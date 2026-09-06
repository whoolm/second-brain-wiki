---
title: "Transkrip Harvard Gabungan — Failed Extraction Catalog"
type: "source"
tags:
  - "education"
  - "data-quality"
sources:
  - "raw/Transkrip_Harvard_Gabungan_Total.md"
sub_categories:
  - "Katalog Pendidikan"
  - "Kualitas Data & Pipeline"
  - "Topik Menunggu Ekstraksi"
entities:
  - "harvard-online"
updated: "2026-09-05"
---

# Transkrip Harvard Gabungan — Failed Extraction Catalog

> 284 entri Harvard Online; 283 gagal diekstrak (error format yt-dlp, pesan 227 char identik) + 1 kosong. Nol klaim substantif. Nilai wiki: (a) katalog topik penawaran Harvard Online, (b) studi kasus kegagalan pipeline. Relevan ke [[overview]] sebagai peringatan kualitas korpus.

## Key Claims (cited)

- Ekstraksi gagal massal: pola `[GAGAL PIPELINE AI: ERROR: [youtube] <id>: Requested format is not...]` pada ~283/284 video [raw/Transkrip_Harvard_Gabungan_Total.md]
- Katalog topik (judul + link valid meski materi gagal): Justice (Sandel), Happiness, AI generatif, kepemimpinan, strategi kesehatan, piramida Giza, kota, memasak/ilmu pangan, kontrak, syariah kitab suci dunia, opioid, saraf, iklim, dan puluhan lagi [raw/Transkrip_Harvard_Gabungan_Total.md]

## Concepts & Entities Touched

- [[pipeline-data-quality]] — mode kegagalan ekstraksi massal; judul-terekstrak vs materi-gagal
- [[harvard-online]] — lanskap penawaran (katalog saja, tanpa isi)

## Open Questions

- Re-ekstrak dengan format fallback (audio-only/whisper) untuk 283 video?
- Apakah pola "Requested format" spesifik channel Harvard (DRM/age-gate)?

## Data Quality

> [!warning] Jangan kutip klaim substantif dari sumber ini — tidak ada materi transkrip yang berhasil diekstrak.

## References

[^1]: raw/Transkrip_Harvard_Gabungan_Total.md
