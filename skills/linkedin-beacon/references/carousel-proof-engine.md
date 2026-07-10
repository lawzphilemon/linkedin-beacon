# LINKEDIN CAROUSEL ENGINE — Design System P.R.O.O.F
## v1.0 · Juli 2026 · reference file untuk linkedin-beacon ≥ v1.2.0

**Posisi dokumen:** engine carousel yang dirujuk section 5 SKILL.md. Dokumen ini TIDAK mengubah Intake Protocol, framework B.E.A.C.O.N, goal hierarchy, high-impression mechanics, voice semi-professional, feedback loop dasar, Mode Outreach, maupun hard wall (asuransi · financial planning · politik tidak pernah masuk LinkedIn) — semuanya milik SKILL.md. Dokumen ini menang untuk semua keputusan visual dan produksi carousel; menggantikan `carousel-linkedin-spec.md` (deprecated sejak v1.2.0) — semua produksi carousel LinkedIn memakai design system P.R.O.O.F, bukan adaptasi sistem IG.

**Kalibrasi (keputusan Lawrence, Juli 2026):**
- Prioritas engagement, urut: **Saves > Comments berbobot > Sends > Follow/profile visit** — DM diparkir sampai Fase 2 beacon aktif
- Arah design: **editorial-tech light** — paper, sans geometris besar, evidence-first
- Font: **Space Grotesk** (display) · **Inter** (body) · **JetBrains Mono** (eyebrow/label/footer)
- Canvas 1080×1350 (4:5), **8 slide**, bahasa default **English**
- Level provokasi default: provokatif terukur (sama dengan skala IG)

**Pipeline lengkap:**

```
Fase 0 Intake (beacon §1) → Fase 1 Angle Scoring → Fase 2 Copy (B.E.A.C.O.N → 8 slide)
→ Fase 3 Build & Export PDF → Fase 4 Caption → Fase 5 Self-Check
→ deliver → Fase 6 Feedback Loop
```

Skill yang dibaca saat eksekusi: `linkedin-beacon` (strategi + gate), `signal-copywriting` (fondasi copy + humanizer), `carousel-png-exporter` (mekanika export).

---

## FASE 0 — INTAKE

Pakai Intake Protocol beacon §1 apa adanya: maksimal 5 pertanyaan adaptif, semua batched satu pesan, setiap pertanyaan bawa default, "gas" = semua default, input lengkap = nol pertanyaan + asumsi satu baris. Gate bukti beacon berlaku penuh — tanpa bukti, turunkan klaim jadi hipotesis jujur atau parkir ke topic-backlog.

Dua penyesuaian khusus carousel:

1. Pertanyaan #4 beacon (format & bahasa) — format sudah carousel; **default bahasa berubah jadi English.** Indonesia Jaksel-mix tetap bisa dipilih per post di intake.
2. Tambahan cek wajib: **save artifact** — apa persisnya yang akan orang simpan (framework bernama, checklist, benchmark, workflow). Materi tidak menghasilkan jawaban → kembali ke decision rule beacon §3; kemungkinan ini text post, bukan carousel.

---

## FASE 1 — ANGLE SCORING (bobot LinkedIn)

Generate 3 kandidat angle internal, skor 1–5 per dimensi:

| Dimensi | Bobot | Pertanyaan penilaian |
|---|---|---|
| Save-ability | 35% | Ada artefak yang praktisi simpan buat dipakai kerja? |
| Discussion trigger | 30% | Ada open loop yang hanya bisa dijawab orang yang benar-benar mengerjakan? |
| Send-ability | 20% | Layak dikirim ke rekan satu tim atau klien tanpa malu? |
| Authority compound | 15% | Memperkuat salah satu dari 3 pilar (performance marketing · AI workflow · agency life)? |

Output ke Lawrence: **satu angle terpilih** + alasan 1–2 baris + dua kandidat kalah disebut sekilas. Bukan menu pro/cons.

**Skala provokasi** — identik dengan sistem IG: Level 1 data shock halus · **Level 2 contrarian terukur (DEFAULT)** · Level 3 reframe keras, konfirmasi satu kali. Tambahan LinkedIn: setiap elemen C (counterintuitive) wajib bawa nuance — akui sisi sebaliknya satu kalimat (aturan beacon §2, contrarian tanpa nuance = opini murahan).

**Batas absolut:** hard wall beacon berlaku (asuransi, financial planning, politik). Platform (Meta, Google, TikTok) boleh disebut faktual — itu materi kerja; yang dikritik adalah praktik, setting default, dan pola — bukan menyerang vendor, agency lain, atau individu.

---

## FASE 2 — B.E.A.C.O.N → 8 SLIDE

Elemen wajib: **B + E + N. Minimal 2 dari A / C / O** (O boleh hidup di slide 7 atau di caption). Urutan slide boleh digeser per topik; elemen wajib tidak.

| Slide | Beat | Fungsi | Treatment default |
|---|---|---|---|
| 01 | **B** — Bold stance | Hook: klaim yang bikin praktisi berhenti scroll | Statement centered, accent 1–2 kata |
| 02 | Pacing | Context/stakes: kenapa ini penting sekarang | Fleksibel |
| 03 | **C** — Counterintuitive | Statement yang membalik asumsi | **Dark slide**, highlight accent-on-dark |
| 04 | **E** — Evidence | Bukti lapangan: angka, chart, screenshot | Stat hero / chart / screenshot beranotasi |
| 05 | Breakdown 1 | Framework/langkah, bagian pertama | List top-aligned |
| 06 | Breakdown 2 | Framework/langkah, bagian kedua | List top-aligned |
| 07 | **A** — Angle personal | Nuance, lesson, biaya nyata | Fleksibel; O boleh ditanam di sini |
| 08 | **N** — Next step | Menepati janji slide 1 + satu CTA | Centered, CTA box |

### Word budget (turun satu tingkat dari IG — viewer document LinkedIn render kecil di feed)

- Hook slide 1: **≤ 12 kata**
- Slide body: target **≤ 25 kata**, ceiling absolut **35 kata**
- Slide list: maksimal **4 item** — lebih = pecah dua slide
- Slide data: angka hero + **≤ 15 kata** konteks
- Satu ide per slide, tanpa pengecualian

### Aturan beat

- **Slide 1:** statement, **tanpa tanda tanya** — pertanyaan hidupnya di O (slide 7 atau caption). Wajib lolos feed test: terbaca dan menimbulkan tension pada render kecil (±350px) dalam < 1 detik. Janji slide 1 = utang; catat di Strategy Summary beserta slide pelunasnya.
- **Slide 3 (dark):** satu-satunya dark slide. Statement paling tajam di carousel — pattern break visual sekaligus puncak C.
- **Slide 4 (evidence):** setiap angka = nilai spesifik + sumber + periode. Kontras dua angka lebih kuat dari satu angka. Metodologi transparan mengalahkan "in my experience".
- **Slide 8:** utang slide 1 lunas paling lambat di sini — completion rate rendah dihukum algoritma, janji tidak ditepati = reach jatuh. Satu aksi saja.

---

## FASE 3 — DESIGN SYSTEM P.R.O.O.F

**P**aper · **R**ules · **O**versized type · **O**ne accent · **F**ooter system.

Identitas visual: **annotated dashboard** — bukti lapangan yang dianotasi seperti audit, bukan dekorasi. Ini bahasa visual pilar digital marketing + AI; sistem IG (Cormorant/burgundy = premium advisor) adalah identitas terpisah — **jangan pernah campur elemen antar dua sistem.**

### Canvas

- 1080×1350 px (4:5), preview CSS 420×525 px, `device_scale_factor = 1080/420`
- 8 slide per carousel

### Palette (CSS custom properties di `:root` — satu sumber kebenaran)

| Token | Nilai | Pakai untuk |
|---|---|---|
| `--paper` | `#F4F4F1` | Background slide light |
| `--ink` | `#161616` | Teks utama |
| `--ink-soft` | `#5A5852` | Teks sekunder, subline |
| `--hairline` | `rgba(22,22,22,.16)` | Rules, divider, border screenshot |
| `--accent` | `#E8500A` | SATU-SATUNYA accent di slide light |
| `--dark` | `#101010` | Background dark slide (slide 3) |
| `--paper-on-dark` | `#F4F4F1` | Teks di dark slide |
| `--accent-on-dark` | `#FF7A33` | Highlight di dark slide |
| `--bar-muted` | `rgba(22,22,22,.16)` | Bar chart non-poin |

Aturan warna: accent menandai **yang penting** — 1–2 kata di headline, satu bar utama di chart, delta, rule anotasi. Lebih dari itu = bukan accent lagi. Burgundy `#8B1A1A` dan gold `#C9A84C` **tidak ada** di sistem ini.

Semantik accent: orange sinyal = warna flag di dashboard — konsisten dengan framing waste-first Lawrence. Sengaja jauh dari biru UI LinkedIn (supaya tidak tenggelam di chrome platform) dan dari burgundy IG (supaya dua identitas tidak silang).

### Typography (ukuran pada preview 420px; export ×2.571)

| Peran | Font | Ukuran | Aturan |
|---|---|---|---|
| Display/headline | **Space Grotesk 700** | auto-fit 32–44px | pendek → 44, panjang → 32; line-height 1.08; letter-spacing −1px |
| Stat hero | **Space Grotesk 700** | 64–84px | letter-spacing −2px; angka sebagai headline |
| Body | **Inter 400** | 15.5px | line-height 1.6; **floor** — sempit = potong kata, bukan kecilkan font |
| Emphasis body | **Inter 600** | 15.5px | maksimal satu frasa per slide |
| List item | **Inter 400** | 14.5px | divider hairline antar item |
| Marker list | **JetBrains Mono 500** | 10.5px | index `01 02 03` warna accent bila urutan bermakna; `+` accent bila bukan sequence |
| Eyebrow | **JetBrains Mono 500** | 10.5px caps | letter-spacing 2.5px; SATU tema seragam semua slide |
| Label/anotasi data | **JetBrains Mono 400** | 9.5px caps | letter-spacing 1px |
| Footer baris 1 — nama | **JetBrains Mono 500** | 8.5px caps | letter-spacing 1px |
| Footer baris 2 — headline | **JetBrains Mono 400** | 7.5px caps | letter-spacing 0.8px |

Dramatic gap dipertahankan sebagai identitas: **tidak ada ukuran perantara** antara body 15.5 dan display 32. Kapitalisasi slide: kapital di awal setiap kalimat (aturan lama tetap).

### Layout

- Padding sisi 32px (preview); content area clear **top 78px / bottom 78px** (footer dua baris) — selalu bebas dari footer, termasuk chart dan screenshot
- Struktur dari **rules dan whitespace, bukan card**: hairline full-width di bawah zona eyebrow dan di atas footer. Tanpa inner card floating (itu identitas IG). Radius 0–2px, flat, tanpa shadow
- Slide statement (1, 3, 8) centered; slide list/data (4–6) top-aligned; slide 2 dan 7 fleksibel
- **Signature device — annotated number:** stat hero + rule accent pendek (24px) + satu baris anotasi mono di bawahnya. Persis seperti callout di dashboard. Maksimal 2× per carousel supaya tetap signature
- Swipe cue `→` JetBrains Mono kanan-bawah slide 1–7; slide 8 tanpa
- Footer semua slide, dua baris: baris 1 `LAWRENCE PHILEMON` (kiri) + `NN/08` (kanan); baris 2 `AI-ASSISTED GROWTH MARKETER | GEO & PAID PERFORMANCE` — caps mono mengikuti sistem, tagline sedikit lebih kecil (7.5px) supaya hierarki nama tetap jelas
- Progress bar 2px segmented di bawah footer, 8 segmen, terisi accent sesuai posisi slide

### Treatment per jenis konten

- **Dark slide:** hanya slide 3 (default). Background `--dark`, teks `--paper-on-dark`, highlight `--accent-on-dark` pada 1–2 kata. Satu per carousel — dua dark slide = pattern break-nya mati.
- **Chart:** bar fine-line. Semua bar `--bar-muted`, **satu** bar accent (bar yang jadi poin). Angka di atas bar, label mono di bawah. Tanpa gridline, axis minimal. Data chart mengikuti aturan bukti — proporsi tidak boleh dikarang.
- **Screenshot evidence** (GA4, ads manager, terminal): border hairline 1px, radius 2px, tanpa shadow; tinggi maksimal 55% content area; anotasi mono + rule/underline accent menunjuk bagian penting. Screenshot harus asli dari Lawrence — tidak ada screenshot → pakai chart atau stat hero; jangan pernah mock-up UI vendor seolah-olah asli.
- **CTA slide 8:** satu baris payoff (menepati janji slide 1) + **CTA box** border 1px accent, isi JetBrains Mono caps **≤ 6 kata**. Menu CTA per goal hierarchy beacon: `SAVE THIS FOR YOUR NEXT AUDIT` · `FOLLOW FOR THE NEXT TEARDOWN` · soft DM satu kalimat hanya di Mini Case Study.
- **Foto personal:** bukan bagian v1.0. Topik butuh foto → minta foto asli dari Lawrence; tanpa stock/AI-generated diam-diam.

### Anti-bleed — beda vs sistem IG

| Aspek | IG (B.E.D.A.H) | LinkedIn (P.R.O.O.F) |
|---|---|---|
| Display | Cormorant Garamond Italic Bold | Space Grotesk 700 |
| Mono | Courier New | JetBrains Mono |
| Palette | #EDE6DE · burgundy · gold | #F4F4F1 · ink · orange #E8500A |
| Dark slide | #1c1410 (warm) | #101010 (neutral) |
| Struktur | Inner card floating | Full-bleed + hairline rules |
| Marker list | Arrow `→` burgundy | Index mono / `+` accent |
| Slide count | 7 | 8 |
| Footer | Handle IG, satu baris | Nama + headline profesional, dua baris |
| CTA akhir | ManyChat keyword | Save / follow / soft DM |
| Bahasa default | Indonesia | English |
| Engine strategi | B.E.D.A.H | B.E.A.C.O.N (beacon) |
| Bobot angle | DM 35 · Save 30 · Comment 20 · Share 15 | Save 35 · Comment 30 · Send 20 · Follow 15 |

---

## FASE 2b — HOOK LIBRARY (10 formula, English)

Statement, nol tanda tanya, nol tanda seru. Placeholder `[X]` wajib diganti angka bersumber saat produksi. Rotasi wajib: formula ≠ formula post sebelumnya. Setiap curiosity gap = utang, dicatat di Strategy Summary + slide pelunasnya. Utang tidak lunas = clickbait = rewrite.

1. **Naked number.** Satu angka + tension. — *"[X] campaigns paused this week. All of them still profitable."*
2. **Quiet proof.** Understatement yang memaksa swipe. — *"1 user. 25 days. That's the entire proof of concept."*
3. **Contrarian terukur.** Balikkan metrik kebanggaan. — *"High CTR can mean your campaign is quietly broken."*
4. **Cost of the default.** Setting bawaan sebagai musuh. — *"The default attribution window costs more than most agency fees."*
5. **Two accounts.** Dua realita, satu variabel. — *"Same budget. Same audience. One scaled, one bled — the gap was one decision."*
6. **Insider pattern.** Otoritas dari repetisi lapangan. — *"Every broken account I audit starts with the same mistake."*
7. **Time collapse.** Sebelum vs sesudah workflow. — *"This audit took 6 hours. Now it takes 40 minutes."*
8. **Dated best practice.** Nasihat benar di tahun yang salah. — *"'[Received wisdom]' was great advice. In [year]."*
9. **Framework reveal.** Sistem bernama sebagai janji. — *"I run every account through the same [N] checks before touching budget."*
10. **Receipt on the table.** Eksperimen + hasil. — *"We turned [tactic] off for 30 days. Here's what the data did."*

---

## FASE 4 — CAPTION (English default, lowercase-first)

Caption beacon: 3–5 baris, tugasnya menjual swipe pertama — bukan meringkas slide.

1. **Baris 1 — hook caption.** WAJIB beda dari headline slide 1; keduanya tampil bersamaan di feed
2. **1–2 baris konteks** — kenapa sekarang, apa yang dipertaruhkan
3. **Pointer baca** — arahkan ke slide bernilai: *"slide 4 is the one to save"*
4. **Penutup:** open loop question untuk praktisi (satu-satunya tempat tanda tanya) ATAU soft CTA — pilih satu

Nol hashtag (aturan beacon — interest graph baca kata kunci natural di kalimat). Kata kunci topik masuk natural di 1–2 kalimat pertama. Lowercase-first, nol tanda seru, forbidden words dan closers nol, humanizer pass.

**Filename = judul dokumen di feed.** Beri nama hook pendek layak tampil: `pmax-audit-checklist.pdf`, `geo-pipeline-proof.pdf` — bukan `carousel_final_v3.pdf`.

---

## TRIGGER ENGAGEMENT (Save > Comment > Send > Follow)

- **Save (utama).** Minimal satu slide save-worthy per carousel: framework bernama, checklist, benchmark, workflow. Tidak muncul natural dari angle → angle lemah, kembali ke Fase 1. Ini gate "test save" beacon — gagal = bukan carousel.
- **Comment.** Open loop praktisi di slide 7 atau caption — pertanyaan yang hanya bisa dijawab orang yang mengerjakan. "Agree?" dan sejenisnya = engagement bait = mati.
- **Send.** Bila topik cocok, framing "send this to whoever runs your account" — bonus, bukan target.
- **Follow.** Label seri + disiplin pilar = alasan follow. CTA follow menjanjikan edisi berikutnya yang spesifik.
- **DM.** Parkir sampai Fase 2 beacon (5 post berturut di atas benchmark). Soft DM hanya di Mini Case Study, satu kalimat, tanpa urgensi.

---

## FASE 3b — BUILD & EXPORT (PDF document post)

1. **Build HTML** single file 8 slide, semua token lewat CSS custom properties di `:root`.
2. **Embed font base64 — tiga font wajib ter-embed:** Space Grotesk, Inter, JetBrains Mono.
   - Sumber primer: file .ttf di uploads/knowledge base Lawrence.
   - Sumber sekunder (terverifikasi Juli 2026, lisensi OFL): repo GitHub `google/fonts` — `ofl/spacegrotesk/SpaceGrotesk[wght].ttf`, `ofl/jetbrainsmono/JetBrainsMono[wght].ttf`, `ofl/inter/Inter[opsz,wght].ttf` (variable font, embed sebagai `format('truetype-variations')`).
   - Sumber tersier: `embed_fonts.py` dari `carousel-png-exporter` dengan `GOOGLE_FONTS_URL` diganti ke tiga family ini.
   - **Semua jalur gagal = STOP dan minta file font.** Tanpa fallback system font — font berbeda = sistem berbeda.
3. **Export PNG per slide** via `export_slides.py`: `TOTAL_SLIDES = 8`, `element.screenshot()`, `device_scale_factor = 1080/420`. Verifikasi tiap PNG tepat 1080×1350.
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

5. **Verifikasi PDF:** 8 halaman, urutan benar, Space Grotesk render asli (cek huruf khasnya: `a`, `g`, angka `1`), warna token benar, tanpa clipping.
6. **Deliver PDF ke Lawrence.** Upload manual. Buffer hanya draft/idea — tidak pernah create_post atau schedule tanpa approve eksplisit.

Default eksekusi: lanjut sampai PDF dalam satu run (execute-first) — kecuali Lawrence bilang "copy dulu".

---

## FASE 5 — SELF-CHECK (pre-export; menggantikan poin carousel di gate beacon §10)

- [ ] Feed test: slide 1 terbaca + menimbulkan tension pada render kecil dalam < 1 detik
- [ ] Slide 1 = statement, tanpa tanda tanya, ≤ 12 kata
- [ ] B + E + N ada; minimal 2 dari A / C / O
- [ ] Utang curiosity slide 1 lunas paling lambat slide 8
- [ ] Minimal satu slide save-worthy — jawaban jelas untuk "apa yang di-save"
- [ ] Word budget: ≤ 25 target / 35 ceiling per slide; list ≤ 4 item; satu ide per slide
- [ ] Satu accent; dark slide hanya satu; tidak ada elemen sistem IG (burgundy/gold/Cormorant/card)
- [ ] Semua angka: nilai + sumber + periode, atau [perlu verifikasi]; proporsi chart tidak dikarang
- [ ] Nol tanda seru; nol emoji; nol hashtag; nol forbidden words dan closers
- [ ] Bahasa konsisten dengan keputusan intake (default English)
- [ ] Hook caption ≠ headline slide 1; caption tidak menduplikasi isi slide
- [ ] Formula hook ≠ formula post sebelumnya
- [ ] Filename layak tampil sebagai judul dokumen
- [ ] Font asli ter-embed (tiga-tiganya); footer + progress bar benar
- [ ] Topik tidak menyentuh asuransi / financial planning / politik; voice tidak bleed
- [ ] Humanizer pass — tidak terasa AI, ritme kalimat bervariasi

Gagal satu poin = perbaiki dulu, jangan deliver draft mentah.

---

## FASE 6 — FEEDBACK LOOP (extend beacon §8)

Log per carousel, tambahan di atas log beacon: **formula hook · angle + skor · level provokasi · design version (P.R.O.O.F v1.0) · filename**.

- **Metrik utama: saves per 1.000 impressions** — sesuai bobot kalibrasi. Sekunder: comments berbobot (dari praktisi, bukan basa-basi), sends, followers baru per post.
- **Baseline design baru:** 5 carousel pertama P.R.O.O.F membentuk baseline sendiri; bandingkan vs carousel era Cormorant sebagai A/B kasar — log design version yang bikin ini mungkin.
- Benchmark berjalan: kalahkan median 5 carousel terakhir.
- Diagnosis wajib format **[aksi] + [objek] + [angka]**. Contoh: "pensiunkan formula hook #7 — dua carousel terakhir saves/1k = 2,1 vs median 4,8."
- Pola konsisten ≥ 3 post → usulkan revisi dokumen ini sebagai v1.x, tunjukkan diff dulu (aturan approval Lawrence).

---

## REKOMENDASI SERI (opsional, bisa dimatikan per carousel)

Eyebrow sebagai label seri: `FIELD NOTES — [TOPIC]` (JetBrains Mono caps). Seri bernama = alasan follow + recall antar post. Konsisten dengan aturan eyebrow satu tema seragam per carousel.

---

## OUTPUT FORMAT PER PRODUKSI

1. **Strategy Summary:** angle terpilih + skor, pilar, elemen B.E.A.C.O.N yang aktif, level provokasi, formula hook, utang curiosity + slide pelunas, save artifact, bahasa, filename usulan.
2. **The Copy:** per slide — nomor, beat, treatment, teks final, design notes pakai marker `[ACCENT]` `[DARK SLIDE]` `[STAT HERO]` `[CHART]` `[SCREENSHOT]` `[EYEBROW:]` `[CTA BOX:]`.
3. **Caption** lengkap, lowercase-first, struktur Fase 4 + usulan filename.
4. **The Logic:** 4–6 bullet — teknik per beat + kenapa angle ini menang.
5. Lanjut Fase 3b build & export dalam run yang sama.

---

## PRECEDENCE (kalau ada konflik antar-dokumen)

- **Visual carousel LinkedIn:** dokumen ini menang — `carousel-linkedin-spec.md` deprecated untuk spec visual; mekanika export-nya sudah diserap ke Fase 3b.
- **Strategi & mekanika LinkedIn:** `linkedin-beacon` menang — intake, B.E.A.C.O.N, goal hierarchy, high-impression mechanics, feedback loop dasar, Mode Outreach.
- **Copy rules:** `signal-copywriting` fondasi; word budget carousel LinkedIn mengikuti Fase 2 dokumen ini.
- **Sistem IG** (B.E.D.A.H + Cormorant/burgundy) tidak tersentuh — platform terpisah, tidak pernah silang elemen.
- **Hard rules Lawrence** (angka bersumber, forbidden words, nol tanda seru, approval gates, no publish otomatis): tidak pernah di-override oleh dokumen manapun.

---

## SUMBER

- Mekanika algoritma LinkedIn 2026 (dwell/saves/sends, batas 8–10 slide, interest graph, engagement bait mati): sumber tercatat di `linkedin-beacon` SKILL.md — Dataslayer LinkedIn Algorithm 2026; Forbes/Jodie Cook, Jan 2026; Melanie Goodman, Interest Graph & Topic Authority 2026; Markana Media, Jun 2026.
- Font (lisensi SIL OFL, verified Juli 2026 via repo `google/fonts`): Space Grotesk © Florian Karsten; JetBrains Mono © JetBrains; Inter © Rasmus Andersson.

---

*v1.0 — Juli 2026. Kalibrasi: saves-first (35/30/20/15), editorial-tech light, Space Grotesk + Inter + JetBrains Mono, English default, 8 slide 4:5. Menggantikan carousel-linkedin-spec.md untuk visual; beacon tetap sumber kebenaran strategi.*
