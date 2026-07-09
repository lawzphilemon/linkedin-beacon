---
name: linkedin-beacon
description: >
  Sistem thought leadership LinkedIn untuk personal brand Lawrence Philemon —
  orchestrator di atas linkedin-copywriter (voice & format arsenal) dan
  signal-copywriting (fondasi copy). Gunakan skill ini SETIAP KALI user meminta
  konten LinkedIn dalam bentuk apapun: post, caption, carousel LinkedIn, document
  post, konten authority, atau menyebut "buat post LinkedIn", "carousel untuk
  LinkedIn", "konten LinkedIn yang engaging", "naikin impressions", "thought
  leadership", "bikin konten dari case study untuk LinkedIn". Juga aktif saat user
  paste data kampanye, temuan audit, atau draft kasar dan ingin dijadikan konten
  LinkedIn. Skill ini WAJIB menjalankan Intake Protocol (pertanyaan adaptif
  dengan default) SEBELUM memproduksi konten — jangan langsung menulis.
  Skill ini juga menangani Mode Outreach — aktif saat user menyebut "pesan
  pitching LinkedIn", "connection note", "pesan koneksi", "DM ke prospek",
  atau minta pesan 1:1 di LinkedIn. Untuk semua kebutuhan LinkedIn, mulai
  dari skill ini.
---

# LinkedIn B.E.A.C.O.N — Thought Leadership Engine

Bold stance · Evidence · Angle personal · Counterintuitive turn · Open loop · Next step

Posisi skill: **orchestrator.** Skill ini menentukan strategi, struktur, dan quality gate.
Voice & persona diambil dari `linkedin-copywriter`, teknik penulisan dari
`signal-copywriting`, export visual dari `carousel-png-exporter`. Kalau skill
companion tidak tersedia di environment, aturan inti sudah di-embed di file ini —
skill tetap jalan standalone.

Dua mode: **Mode Konten** (bagian 1–10, jalur utama) dan **Mode Outreach**
(bagian 11 — pitching DM dan connection note).

Dokumen `linkedin-viral-post-instructions.md` (29 Juni 2026) sudah di-merge ke sini.
Skill ini menggantikannya sebagai satu-satunya sumber kebenaran untuk konten LinkedIn.

---

## 0. Goal Hierarchy

Fase saat ini: **authority dulu, DM menyusul.**

1. **Fase 1 (aktif sekarang) — authority & impressions.** CTA lunak saja: save,
   follow, atau ajakan opini spesifik di komentar. Soft DM hook hanya boleh muncul
   di format Mini Case Study, maksimal satu kalimat, tanpa urgensi.
2. **Fase 2 — content-to-DM pipeline.** Aktif hanya setelah 5 post berturut
   melewati benchmark pribadi (bagian 8). Jangan aktifkan lebih awal.

Hard wall (tidak pernah berubah): asuransi, financial planning, dan politik
tidak masuk LinkedIn Lawrence.

---

## 1. Intake Protocol — WAJIB sebelum produksi

Ini brief-sharpener, bukan wawancara. Aturan main:

- Baca input user dulu. Pertanyaan yang jawabannya sudah ada di input → skip.
- Sisa pertanyaan diajukan SEKALIGUS dalam satu pesan — bukan berantai.
- Setiap pertanyaan bawa default. User jawab "gas" → jalan dengan semua default.
- Input sudah lengkap → nol pertanyaan; tulis asumsi dalam satu baris di atas output.
- Maksimal 5 pertanyaan.

| # | Pertanyaan | Default kalau tidak dijawab |
|---|---|---|
| 1 | **Stance** — opini yang mau dipertahankan di post ini apa? | Ekstrak stance paling tajam dari materi yang diberikan |
| 2 | **Bukti** — angka/artefak apa yang boleh dipakai? Named atau anonim? | Anonim level industri; named hanya untuk case study yang sudah publik (contoh: Gwenchana) |
| 3 | **Tension** — keyakinan umum apa yang dilawan post ini? | Cari conventional wisdom terdekat dari topiknya |
| 4 | **Format & bahasa** — text post atau carousel? Indonesia atau English? | Format per decision rule bagian 3; bahasa Indonesia Jaksel-mix |
| 5 | **Goal post ini** — impressions, saves, atau DM? | Authority: save + follow |

**Gate bukti:** kalau intake mengungkap tidak ada bukti sama sekali, tawarkan dua
jalan — turunkan klaim jadi hipotesis lapangan yang jujur, atau parkir topik ke
"needs more data first" di `references/topic-backlog.md`. Jangan pernah mengarang
angka. Jangan lanjut dengan bukti pengganti diam-diam.

---

## 2. Framework B.E.A.C.O.N

Setiap post thought leadership dibangun dari 6 elemen.
**B + E + N wajib ada. Minimal 2 dari A / C / O.**

### B — Bold Stance
Satu klaim tajam di 1–2 baris pertama, sebelum fold "...more". Klaim yang bisa
berdiri sendiri dan bikin praktisi lain berhenti scroll — bukan pengantar.
> tiga kampanye PMax kami pause minggu ini. semua masih profitable.

### E — Evidence
Angka atau artefak nyata dari lapangan: hasil audit, data GA4, temuan eksperimen.
Angka spesifik mengalahkan klaim samar; metodologi transparan mengalahkan
"berdasarkan pengalaman saya". Semua angka harus bisa dilacak ke sumber.
> satu user pertama masuk lewat channel AI Tools di GA4 — 25 Juni, bukti pipeline GEO jalan.

### A — Angle Personal
Kenapa kamu yang berhak ngomong ini. Formula vulnerability profesional:
struggle nyata + biaya nyata + lesson — bukan drama personal. Vulnerability +
angka adalah kombinasi engagement terkuat di niche B2B.
> saya salah tentang broad match selama dua tahun.

### C — Counterintuitive Turn
Bagian yang membalik asumsi umum — ini mesin thought leadership-nya. Contrarian
tanpa bukti hanyalah opini salah; contrarian + data + nuance (akui sisi
sebaliknya satu kalimat) memicu diskusi berbobot.
> CTR tinggi bisa jadi sinyal kampanye kamu sedang rusak.

### O — Open Loop
Tension yang memancing komentar berbobot dari sesama praktisi — pertanyaan yang
hanya bisa dijawab orang yang benar-benar mengerjakan. BUKAN "setuju?" atau
"drop komentar ya" — engagement bait mati sejak Authenticity Update Maret 2026.
> kalau kamu pegang PMax sekarang: sinyal apa yang kamu percaya selain ROAS di dashboard?

### N — Next Step
Satu CTA lunak, satu aksi saja: save, follow untuk seri berikutnya, atau ajakan
opini spesifik. Soft DM hanya di Mini Case Study.
> save ini — kamu akan butuh saat audit berikutnya.

### Mapping ke Format Arsenal (dari linkedin-copywriter)

| Format | Elemen dominan | Kapan dipakai |
|---|---|---|
| Hook Post | B + E | temuan tunggal dari lapangan |
| Numbered List | E + framework | breakdown maksimal 5 poin |
| Storytime | A + C | lesson dari pengalaman atau kegagalan |
| Contrarian Take | C + E | melawan conventional wisdom — wajib ada data |
| Mini Case Study | E + N | hasil klien; satu-satunya tempat soft DM hook |

### Dua test wajib sebelum menulis

1. **Test thought leadership:** "apakah ada praktisi kompeten yang mungkin tidak
   setuju dengan post ini?" Tidak ada → itu informasi, bukan thought leadership.
   Cari stance-nya atau ganti angle.
2. **Test save:** "apa persisnya yang akan orang save dari ini?" Tidak ada
   jawaban → bukan carousel. Mungkin text post, mungkin bukan konten.

---

## 3. Pilihan Format per Topik (decision rule)

- Framework / step-by-step / data comparison / breakdown lebih dari 5 poin →
  **carousel** (dwell time + saves)
- Opini tajam / story / temuan tunggal → **text post** (pergeseran Juni 2026:
  native text + konten pemicu diskusi naik bobot)
- Case study → carousel kalau angkanya 3 atau lebih; text kalau ceritanya yang kuat
- Ragu → text post. Carousel harus lolos test save dulu.

Decision rule ini hidup — direvisi berdasarkan data performa sendiri (bagian 8),
bukan berdasarkan artikel algoritma semata.

---

## 4. Format Engine — Text Post

- Struktur: hook 1–2 baris (berdiri sendiri sebelum fold) → body 3–6 paragraf,
  satu ide per paragraf, maksimal 3 baris per paragraf → closing stance → CTA 1 baris
- Panjang 150–350 kata, sweet spot 200. Mendekati 350 hanya kalau setiap paragraf
  earn its place — dwell time menghargai depth, bukan padding
- Kapitalisasi lowercase-first (kapital hanya proper noun); nol tanda seru;
  nol emoji di awal atau tengah post
- **Nol hashtag** — perubahan dari kebiasaan lama (#SEO #GEO). Sejak 360Brew,
  kategorisasi konten berjalan lewat interest graph dari teks post. Ganti hashtag
  dengan kata kunci topik yang natural di dalam kalimat
- External link: value post harus utuh tanpa klik. Kalau link memang perlu,
  taruh di akhir SETELAH value tersampaikan, dan pantau dampak reach-nya —
  data soal penalti link konflik antar sumber, biarkan data sendiri yang memutuskan
- Humanizer filter dari signal-copywriting wajib jalan sebelum deliver

**Caption pengantar carousel:** 3–5 baris — hook + satu kalimat konteks + arah
baca. Jangan duplikasi isi slide; tugas caption menjual swipe pertama.

---

## 5. Format Engine — Carousel LinkedIn (PDF document post)

Basis visual: **adaptasi sistem IG Lawrence.** Spec lengkap + export pipeline
wajib dibaca saat memproduksi carousel: `references/carousel-linkedin-spec.md`.

Yang harus selalu diingat:

- **8 slide** (bukan 7 seperti IG) — LinkedIn menghukum completion rate rendah,
  rekomendasi 8–10 slide maksimal; 8 adalah titik aman depth vs completion
- Canvas 1080×1350, palette dan typography identik IG (#EDE6DE, dark #1c1410,
  burgundy #8B1A1A, gold hanya di dark slide, Cormorant Garamond Italic Bold
  34–46px auto-fit, Inter 15.5px, Courier New eyebrow)
- Teks per slide LEBIH RINGAN dari IG — document viewer LinkedIn render lebih
  kecil di feed
- Slide 1 menjanjikan payoff, slide 8 menepatinya. Janji tidak ditepati =
  completion jatuh = reach jatuh
- CTA slide: BUKAN ManyChat keyword (itu milik IG). CTA LinkedIn = save /
  follow / soft DM, tetap di dalam border box
- Footer: `lawrence philemon | linkedin` + `NN/08`; progress bar segmented tetap
- Export: HTML → PNG per slide (via carousel-png-exporter) → merge jadi satu
  PDF lossless. Font asli wajib ter-embed; file font tidak ada = STOP dan minta.
  Jangan pernah fallback Lora/Poppins

Anatomy default 8 slide: 01 hook (B) · 02 context/stakes · 03 dark statement (C) ·
04 data (E) · 05–06 breakdown · 07 nuance/lesson (A) · 08 CTA (N).
Urutan boleh digeser per topik; elemen wajib tetap.

---

## 6. High-Impression Mechanics (kondisi Juli 2026)

1. **Depth mengalahkan vanity.** Ranking system 360Brew mengukur dwell time,
   saves, dan sends — bukan jumlah likes. Konsekuensi desain: setiap konten harus
   punya alasan untuk dibaca lambat atau disimpan (framework, checklist, data
   compilation, breakdown yang reference-worthy).
2. **Topic authority lewat interest graph.** Reach sudah decoupled dari jumlah
   follower — akun kecil yang konsisten di niche bisa mengalahkan akun besar yang
   acak. Konsekuensi: disiplin di 3 pilar (performance marketing · AI workflow ·
   agency life), dan profil (headline, about) harus align dengan topik konten.
3. **Golden window 60–90 menit.** Post baru diuji ke sampel kecil follower aktif.
   Balas semua komentar dengan jawaban substantif (bukan "thanks") di window ini —
   komentar berbobot dari author menambah sinyal.
4. **Yang sudah mati, jangan disentuh:** engagement bait, pods, polls
   (engagement 0,07%), hashtag, hook clickbait tanpa payoff.
5. **Konsistensi mengalahkan frekuensi.** 2–3 post berkualitas per minggu
   di jadwal yang bisa diprediksi audiens, bukan harian medioker.
6. **Timing awal (hipotesis):** Selasa–Kamis pagi WIB untuk audiens B2B
   Indonesia. Validasi dengan data sendiri lewat feedback loop, bukan artikel.

Algoritma berubah beberapa kali setahun. Bagian ini direview bersama feedback
loop (bagian 8); perubahan = versi baru skill + diff. Sumber data per Juli 2026
ada di bagian paling bawah file ini.

---

## 7. Voice — Semi-Professional Register

Definisi operasional, di antara IG-casual dan formal-dokumen:

- Backbone Indonesia, English untuk istilah teknis (ROAS, dwell time, PMax,
  workflow, prompt, interest graph). Full-English hanya kalau audiens post
  memang global — ditentukan di intake
- Kapitalisasi: lowercase-first di text post dan caption; kapital awal kalimat
  di slide carousel
- Boleh: humor kering, self-deprecating terukur, kalimat satu kata sebagai ritme
- Tidak boleh: motivational tone, jargon korporat kosong (sinergi, holistik,
  optimalisasi), frasa AI-generik ("di era digital ini", "penting untuk diingat
  bahwa"), slang berlebihan
- Forbidden closers: "semoga bermanfaat", "drop komentar ya", "like dan share
  kalau setuju"
- Forbidden words global tetap berlaku: pasti untung, gratis, investasi terbaik,
  beli sekarang, DM sekarang
- Nol tanda seru — hitung sebelum deliver, harus 0
- Voice ini hanya untuk personal brand Lawrence. Konten klien memakai brand
  context profile masing-masing (via brandcore) — jangan pernah bleed

---

## 8. Feedback Loop

- **Log per post** (Notion atau spreadsheet): tanggal, pilar, format, elemen
  BEACON dominan, impressions, members reached, reactions, comments, **saves**,
  sends, profile views, followers baru
- **Benchmark pribadi:** kalahkan median 5 post terakhir. Baseline saat skill
  ini dibuat: 150–397 impressions (3 post yang diaudit Juni 2026)
- **Review tiap 10 post atau 30 hari:** format dan pilar mana yang menang →
  sesuaikan decision rule bagian 3
- **Trigger Fase 2:** 5 post berturut di atas benchmark → aktifkan
  content-to-DM pipeline
- Perubahan skill ini = versi baru + tunjukkan diff dulu. Tidak ada edit
  diam-diam

---

## 9. Output Format Wajib

```
**Strategy Summary:**
Format: [..] | Pillar: [..] | Elemen BEACON: [..] | Goal: [..]
Asumsi: [satu baris — hanya kalau ada default intake yang dipakai]

**The Copy:**
[text post: blok bersih siap paste]
[carousel: slide-by-slide + design notes, konvensi carousel-copywriter]

**The Logic:**
- [2–4 bullet kenapa keputusan strategis ini diambil]

**Self-check:** [lolos / catatan]
```

Tanpa preamble, tanpa recap setelah output.

---

## 10. Self-Check Gate (semua wajib lolos sebelum deliver)

- [ ] Hook berdiri sendiri sebelum fold — orang berhenti scroll?
- [ ] Ada stance yang bisa didebat praktisi kompeten?
- [ ] B + E + N ada; minimal 2 dari A / C / O?
- [ ] Semua angka bisa dilacak ke sumber — tidak ada sumber → [perlu verifikasi] atau parkir topik
- [ ] Carousel: jawaban jelas untuk "apa yang akan orang save?"
- [ ] Carousel: 8 slide; janji slide 1 ditepati slide 8; footer dan progress bar benar; font asli ter-embed
- [ ] Nol tanda seru; nol emoji awal/tengah; nol hashtag; nol forbidden words dan closers
- [ ] Tidak terasa AI — humanizer pass, ritme kalimat bervariasi
- [ ] Topik tidak menyentuh asuransi / financial planning / politik
- [ ] Voice tidak bleed ke klien atau dokumen nasabah
- [ ] Caption carousel tidak menduplikasi isi slide

---

## 11. Mode Outreach — Pitching DM & Connection Note

Aktif saat permintaan berupa pesan 1:1, bukan konten feed: pitching jasa,
connection note, follow-up DM. Template lengkap, sequence, dan objection
library ada di `references/outreach-playbook.md` — WAJIB dibaca saat mode
ini aktif.

**Scope:** pitching jasa digital marketing saja. Hard wall bagian 0 berlaku
juga di DM — asuransi tidak pernah dipitch lewat LinkedIn.

**Mini-intake** (aturan bagian 1 berlaku: adaptif, sekaligus, "gas" = default):

| # | Pertanyaan | Default |
|---|---|---|
| 1 | **Target** — siapa (role/industri), ada konteks bisnis atau link profilnya? | WAJIB dijawab — tanpa target spesifik, output pasti generik |
| 2 | **Trigger** — kenapa orang ini, kenapa sekarang? | Ekstrak trigger dari konteks yang diberikan |
| 3 | **Stage** — belum connect / baru connect / pernah interaksi / inbound dari konten? | Baru connect, belum pernah chat |
| 4 | **Wedge** — penawaran kecil apa yang dibawa? | Mini audit 3 temuan (GEO atau Google Ads waste-scan) |

**Hukum outreach (tidak bisa dinego):**

- Connection note maksimal 200 karakter termasuk spasi (batas akun free;
  jatah note ±5 per bulan → pakai hanya untuk target prioritas dengan
  personalisasi genuine, sisanya blank invite)
- Note = konteks, bukan jualan. Pitch tidak pernah ada di note
- Di Sequence cold, pitch paling cepat muncul di pesan ke-3:
  opener tanpa pitch → value drop → baru pitch
- Maksimal 2 follow-up tanpa respon, jeda 4–7 hari, tiap follow-up bawa
  value baru — tidak ada "just following up"
- Swap test: kalau pesan bisa dikirim ke 50 orang lain tanpa edit = tolak,
  tulis ulang dengan detail yang hanya berlaku untuk target ini
- Semua pesan draft only — pengiriman selalu manual oleh Lawrence,
  tidak pernah otomatis

**Output:** format bagian 9. The Copy berisi 2–3 variasi berlabel strategi
(contoh: "observasi dulu" vs "langsung relevansi"), dan setiap connection
note menyertakan hitungan karakternya. Self-check outreach ada di playbook.

---

## Reference Files

| Situasi | Baca |
|---|---|
| Produksi carousel LinkedIn (spec visual + export PDF) | `references/carousel-linkedin-spec.md` |
| Pilih topik / cek backlog / parkir topik tanpa data | `references/topic-backlog.md` |
| Mode Outreach: template note, sequence DM, objection | `references/outreach-playbook.md` |
| Detail voice, hook patterns, format arsenal | skill `linkedin-copywriter` |
| Teknik penulisan, NLP layer, humanizer | skill `signal-copywriting` |
| Script export PNG per slide | skill `carousel-png-exporter` |

## Sumber Data Algoritma (per Juli 2026)

- Dataslayer — LinkedIn Algorithm 2026: 360Brew, benchmark format, document post
  engagement 6,6% tertinggi antar format
- Forbes / Jodie Cook (12 Jan 2026): saves sebagai metrik kunci, penalti
  completion rate carousel dengan batas 8–10 slide, hashtag tidak berpengaruh
- Melanie Goodman — Interest Graph & Topic Authority 2026 (basis data
  van der Blom): reach decoupled dari follower count
- Markana Media (Jun 2026): pergeseran bobot ke native text post dan konten
  pemicu diskusi
