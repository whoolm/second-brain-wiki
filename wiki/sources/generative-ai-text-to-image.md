---
title: "Generative AI — Text-to-Image Models (Diffusion)"
type: "source"
tags: ["research", "ai", "diffusion"]
sources: ["raw/11_Generative_AI__Text-to-Image_Models.md"]
entities: []
updated: 2026-09-05
sub_categories: []
---

# Generative AI — Text-to-Image Models (Diffusion)

> Kuliah penutup: diffusion teks-bersyarat + transformer (Sora), intuisi joint embedding teks-gambar, dan demo HuggingFace (deteksi/segmentasi). Fondasi untuk [[generative-ai-methods]].

## Key Claims (cited)

- Demo: ChatGPT photorealistic grad-students (minus instruktur), Midjourney desa Italia ala Monet; Sora (15 Feb, OpenAI) teks→video 1-menit, contoh tidal-wave + surfers di aula historis [raw/11_Generative_AI__Text-to-Image_Models.md]
- Sora tech report: text-conditional diffusion + transformer architecture [raw/11_Generative_AI__Text-to-Image_Models.md]
- Intuisi: embedding prompt ≈ embedding gambar-gambar yang cocok (satu ruang); denoise embedding → gambar final [raw/11_Generative_AI__Text-to-Image_Models.md]
- Pipeline HuggingFace: object-detection (bounding-box: cat/remote/couch) → image-segmentation (mask per-objek) [raw/11_Generative_AI__Text-to-Image_Models.md]
- Kualitas data: loop 3x (dedup 40567→14094 kata); prompt persis dan tanggal rilis perlu verifikasi slide [raw/11_Generative_AI__Text-to-Image_Models.md]

## Concepts & Entities Touched

- [[generative-ai-methods]] — diffusion + joint embedding
- [[ai-in-education]] — demo sebagai pedagogi

## Open Questions

- Detail arsitektur diffusion (schedule, sampler, CLIP vs lain) tidak di transkrip — butuh slide.

## References

[^1]: raw/11_Generative_AI__Text-to-Image_Models.md
