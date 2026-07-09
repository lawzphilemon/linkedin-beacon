# Carousel LinkedIn — Spec Visual & Export Pipeline

Adaptasi dari design system Instagram Lawrence Philemon untuk format document
post LinkedIn (satu file PDF). Baca file ini setiap kali memproduksi carousel
LinkedIn — jangan mengerjakan dari memori.

---

## Perbedaan vs sistem IG (baca ini dulu)

| Aspek | Instagram | LinkedIn |
|---|---|---|
| Jumlah slide | 7 | **8** |
| Format upload | PNG per slide | **1 file PDF** (document post) |
| CTA slide akhir | ManyChat keyword | save / follow / soft DM |
| Footer kiri | `lawrence philemon \| ig: @lawrencephilemon_` | `lawrence philemon \| linkedin` |
| Hashtag di caption | sesuai aturan IG | **nol** |
| Densitas teks per slide | standar | lebih ringan — viewer LinkedIn render kecil di feed |
| Kapitalisasi slide | kapital awal kalimat | kapital awal kalimat (sama) |

Kenapa 8 slide: LinkedIn menghukum completion rate rendah pada document post;
rekomendasi 2026 adalah 8–10 slide maksimal. 8 = titik aman antara depth
(dwell time) dan completion.

---

## Canvas & Warna (identik IG)

- 1080×1350 px (rasio 4:5), preview CSS 420×525 px, `device_scale_factor = 1080/420`
- Background light: `#EDE6DE`
- Dark slide: `#1c1410` — dipakai untuk slide statement/quote di tengah carousel
- Accent burgundy: `#8B1A1A` (satu-satunya accent di slide light)
- Gold: `#C9A84C` — HANYA untuk highlight italic di dark slide
- Accent pada 1–2 kata kunci per headline (burgundy di light, gold di dark)
- Inner card floating: border 0.5px `rgba(139,26,26,0.2)`, radius 3px
- Semua nilai lewat CSS custom properties di `:root` — satu sumber kebenaran,
  konsistensi antar slide dijamin

## Typography (identik IG)

- Headline: **Cormorant Garamond Italic Bold**, auto-fit 34–46px berdasar
  panjang teks (pendek → 46, panjang → 34), line-height 1.1, letter-spacing -0.5px.
  Tidak ada ukuran perantara antara body dan display — dramatic gap adalah
  identitas visual
- Body: **Inter 400** 15.5px, line-height 1.6 — JANGAN turun di bawah 15.5px
- List item: Inter 14.5px, arrow burgundy `→`, divider tipis antar item
- Eyebrow: **Courier New** 10.5px caps, letter-spacing 2.5px — SATU tema
  seragam di semua slide (bukan judul berbeda per slide)
- Kapitalisasi slide: kapital di awal setiap kalimat

## Layout

- Content area: clear top 78px / bottom 64px — selalu bebas dari footer,
  termasuk diagram
- Slide statement / hook / CTA: centered. Slide list: top-aligned
- Swipe arrow Courier New bottom-right di semua slide non-final;
  slide 8 tanpa arrow
- Footer semua slide: `lawrence philemon | linkedin` (kiri) + `NN/08` (kanan),
  Courier New 8.5px caps
- Progress bar 2px segmented di bawah footer, segmen terisi sesuai posisi slide
- Diagram piramida/segitiga via CSS clip-path, tier stacked, label mono di
  bawah tiap tier, wajib clearance dari footer

## Anatomy Default 8 Slide

| Slide | Peran | Elemen BEACON |
|---|---|---|
| 01 | Hook — menjanjikan payoff | B |
| 02 | Context / stakes — kenapa ini penting sekarang | — |
| 03 | Dark statement (background #1c1410, gold highlight) | C |
| 04 | Data / chart | E |
| 05 | Breakdown 1 | framework |
| 06 | Breakdown 2 | framework |
| 07 | Nuance / lesson | A |
| 08 | CTA — menepati janji slide 01 | N |

Urutan boleh digeser per topik. Elemen wajib (B, E, N) tidak boleh hilang.

## Copy Rules per Slide

- Maksimal ±30 kata per slide; satu ide per slide (aturan carousel-copywriter
  tetap berlaku, dengan densitas lebih ringan dari IG)
- Slide 01: di bawah 15 kata, tanpa tanda tanya, klaim yang bikin berhenti scroll
- Slide 08: satu aksi saja, keyword CTA dalam border box (burgundy di light,
  gold di dark)
- Setiap slide harus masuk akal berdiri sendiri DAN mengalir ke slide berikutnya

---

## Export Pipeline (wajib berurutan)

1. **Build HTML** single file berisi 8 slide, CSS custom properties di `:root`
   sebagai satu sumber kebenaran ukuran/warna.
2. **Embed font base64.** Pakai `embed_fonts.py` dari skill
   `carousel-png-exporter` (sudah dikonfigurasi Cormorant Garamond + Inter).
   File font asli tidak tersedia dan embed gagal → STOP dan minta file font.
   Jangan pernah export dengan fallback Lora/Poppins atau system font.
3. **Export PNG per slide.** Pakai `export_slides.py`
   (`element.screenshot()`, `TOTAL_SLIDES = 8`, `device_scale_factor = 1080/420`).
   Verifikasi tiap PNG tepat 1080×1350.
4. **Merge jadi satu PDF lossless:**

```bash
pip install img2pdf --break-system-packages
python3 - <<'PY'
import img2pdf, glob
pngs = sorted(glob.glob('outputs/slides/slide_*.png'))
assert len(pngs) == 8, f"harus 8 slide, ketemu {len(pngs)}"
with open('outputs/carousel-linkedin.pdf', 'wb') as f:
    f.write(img2pdf.convert(pngs))
print('ok:', 'outputs/carousel-linkedin.pdf')
PY
```

`img2pdf` menyimpan PNG apa adanya tanpa re-kompresi — kualitas identik
dengan export.

5. **Verifikasi PDF:** 8 halaman, urutan benar, font render asli (cek huruf
   a/g/k), tidak ada clipping di tepi, warna brand benar.
6. **Penamaan file:** LinkedIn menampilkan nama file sebagai judul dokumen di
   feed. Beri nama dengan hook pendek yang layak tampil, contoh:
   `geo-audit-workflow.pdf` — bukan `carousel_final_v3.pdf`.
7. **Deliver PDF ke user.** Upload ke LinkedIn dilakukan manual oleh Lawrence.
   Jangan pernah schedule atau publish otomatis (termasuk via Buffer) — draft
   dan file saja; keputusan posting selalu di tangan Lawrence.
