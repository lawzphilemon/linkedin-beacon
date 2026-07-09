# linkedin-beacon

LinkedIn thought leadership engine untuk personal brand Lawrence Philemon.
Orchestrator di atas `linkedin-copywriter` (voice & format arsenal),
`signal-copywriting` (fondasi copy), dan `carousel-png-exporter` (export visual).

## Isi

```
linkedin-beacon/
├── .claude-plugin/
│   └── plugin.json
├── skills/
│   └── linkedin-beacon/
│       ├── SKILL.md                          # core: intake, B.E.A.C.O.N, format engine, self-check
│       └── references/
│           ├── carousel-linkedin-spec.md     # spec visual + export pipeline PDF
│           ├── topic-backlog.md              # backlog topik (migrasi dari doc 29 Juni 2026)
│           └── outreach-playbook.md          # template pitching DM + connection note
└── README.md
```

## Yang dilakukan skill ini

1. **Intake Protocol** — maksimal 5 pertanyaan adaptif (stance, bukti, tension,
   format & bahasa, goal) SEBELUM produksi. Pertanyaan yang sudah terjawab dari
   input di-skip; setiap pertanyaan bawa default; jawab "gas" = jalan dengan
   semua default.
2. **Framework B.E.A.C.O.N** — Bold stance, Evidence, Angle personal,
   Counterintuitive turn, Open loop, Next step. B + E + N wajib, minimal 2 dari
   A/C/O. Dua gate: test thought leadership dan test save.
3. **Format engine** — text post (lowercase-first, nol hashtag, 150–350 kata)
   dan carousel PDF 8 slide dengan design system IG (Cormorant/burgundy) yang
   diadaptasi untuk LinkedIn document post.
4. **High-impression mechanics 2026** — dwell/saves/topic authority, golden
   window 60–90 menit, daftar taktik yang sudah mati.
5. **Feedback loop** — log performa per post, benchmark median 5 post terakhir,
   review tiap 10 post, trigger Fase 2 (DM pipeline).
6. **Mode Outreach** — pitching DM (sequence 3 pesan: opener tanpa pitch →
   value drop → pitch) dan connection note ≤200 karakter, dengan wedge offers,
   objection library, dan self-check terpisah.

## Instalasi

### Via marketplace `lawrence-claude-plugins`

Tambahkan entry ini ke `.claude-plugin/marketplace.json` di root repo
(sesuaikan `source` dengan struktur folder repo):

```json
{
  "name": "linkedin-beacon",
  "source": "./plugins/linkedin-beacon",
  "description": "LinkedIn thought leadership engine — intake adaptif, framework B.E.A.C.O.N, text post + carousel PDF."
}
```

Lalu:

```bash
/plugin install linkedin-beacon@lawrence-claude-plugins
```

### Via claude.ai

Gunakan file `linkedin-beacon.skill` — buka file card dan klik Save skill.

## Relasi dengan skill lain

| Skill | Peran |
|---|---|
| `linkedin-copywriter` | referensi voice, persona, hook patterns, format arsenal |
| `signal-copywriting` | teknik penulisan, NLP layer, humanizer |
| `carousel-png-exporter` | script embed font + export PNG per slide |

Aturan inti sudah di-embed di SKILL.md — skill tetap berfungsi standalone jika
companion tidak tersedia di environment.

## Versioning

Perubahan pada skill ini mengikuti aturan kerja Lawrence: versi baru + diff
ditunjukkan dulu, tidak ada edit diam-diam. Bagian High-Impression Mechanics
direview bersama feedback loop karena algoritma LinkedIn berubah beberapa kali
setahun.

v1.1.0 — Juli 2026. Menambahkan Mode Outreach: pitching DM, connection note,
sequence, wedge offers, objection library (`references/outreach-playbook.md`).

v1.0.0 — Juli 2026. Menggantikan `linkedin-viral-post-instructions.md`
(29 Juni 2026) sebagai satu-satunya sumber kebenaran konten LinkedIn.
