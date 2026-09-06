---
title: "Pipeline Data Quality"
type: "concept"
tags: ["research", "meta", "data-quality"]
sources: ["raw/Transkrip_Harvard_Gabungan_Total.md", "raw/Transkrip_TED_Gabungan_Total.md", "raw/Transkrip_TEDx_Gabungan_Total.md", "raw/1_Artificial_Intelligence_and_Machine_Learning.md", "raw/10_Generative_AI__Adapting_LLMs_with_Parameter-Eff.md", "raw/11_Generative_AI__Text-to-Image_Models.md", "raw/12_Intelligence_How_Do_We_Know_You_Are_Smart_audio.md"]
updated: 2026-09-05
---

# Pipeline Data Quality

> Korpus ini membawa artefaknya sendiri: ekstraksi massal yang gagal total (Harvard), truncasi 100KB/file, dan loop caption 3x di hampir semua video narasi.

## Core Claims

- Harvard: 283/284 gagal (error format yt-dlp identik) — judul valid, materi nol [raw/Transkrip_Harvard_Gabungan_Total.md]
- Truncasi: tiap gabungan terpotong ~100KB (limit max_text_length pipeline) [raw/Transkrip_TED_Gabungan_Total.md]
- Duplikasi caption: frasa berulang 3x (kemungkinan stack multi-bahasa/subtitle) + entitas HTML + `[Music]` [raw/Transkrip_TEDx_Gabungan_Total.md]
- Batch AI 2026-09-05: 3 file kuliah 40–45k kata terkompresi ~35% via dedup 2–3x (mis. 40952→14490; 44942→15440; 40567→14094; 35616→12364); angka arsitektur (vocab 50k, matriks 8000) ilustratif [raw/1_Artificial_Intelligence_and_Machine_Learning.md] [raw/10_Generative_AI__Adapting_LLMs_with_Parameter-Eff.md] [raw/11_Generative_AI__Text-to-Image_Models.md] [raw/12_Intelligence_How_Do_We_Know_You_Are_Smart_audio.md]
- 2 TED talks bersih (2–3k kata, tanpa loop): Russell + Graylin — prioritas kutipan presisi [raw/3_principles_for_creating_safer_AI__Stuart_Russell.md] [raw/3_Possible_Futures_for_AI__Which_Will_We_Choose__A.md]

## Links

- [[transkrip-harvard]]
- [[harvard-online]]

## Open Questions

- Pipeline perbaikan: dedup pra-ingest, fallback whisper untuk Harvard, naikkan/split batas truncasi.
