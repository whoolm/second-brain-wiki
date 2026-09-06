---
title: "Generative AI Methods"
type: "concept"
tags: ["research", "ai", "llm", "diffusion"]
sources: ["raw/1_Artificial_Intelligence_and_Machine_Learning.md", "raw/10_Generative_AI__Adapting_LLMs_with_Parameter-Eff.md", "raw/11_Generative_AI__Text-to-Image_Models.md"]
updated: 2026-09-05
---

# Generative AI Methods

> Dari taksonomi (supervised/unsupervised/RL) ke AR-LM + RAG + LoRA hingga diffusion teks-bersyarat — stack teknis yang menjelaskan mengapa CapEx dan adopsi meledak.

## Core Claims

- Fondasi: supervised/unsupervised/RL; reward = poin; sukses = data + compute + algoritma [raw/1_Artificial_Intelligence_and_Machine_Learning.md]
- AR-LM: linear+softmax atas vocab ~50k; GPT-1/2/3 beda skala, bukan arsitektur [raw/10_Generative_AI__Adapting_LLMs_with_Parameter-Eff.md]
- RAG: embed FAQ + pertanyaan, top-k pack ke context-window (moving-window/summarize-outside) [raw/10_Generative_AI__Adapting_LLMs_with_Parameter-Eff.md]
- LoRA: delta ≈ thin×thin (~0,02%); 1–2 GPU cukup untuk 7/13B [raw/10_Generative_AI__Adapting_LLMs_with_Parameter-Eff.md]
- Diffusion: text-conditional + transformer (Sora); joint embedding teks-gambar → denoise; demo HuggingFace deteksi/segmentasi [raw/11_Generative_AI__Text-to-Image_Models.md]

## Links

- [[ai-ml-accelerator-overview]], [[generative-ai-adapting-llms]], [[generative-ai-text-to-image]]
- [[ai-supercycle-economics]], [[ai-in-education]], [[pipeline-data-quality]]

## Open Questions

- Hyperparameter LoRA (rank), retriever, dan sampler diffusion — butuh slide/lab.

## Tension 6 — Efficiency vs Concentration

> [!warning]
> LoRA/RAG (adaptasi murah 1–2 GPU, ~0,02% params) mendemokratisasi *adaptasi* sementara [[ai-supercycle-economics]] menunjukkan *training* terpusat di hyperscaler (CapEx, AI factories). Rekonsiliasi sementara: training-centralized vs adaptation-distributed. Perlu angka biaya training vs fine-tune + peta siapa menangkap nilai.
