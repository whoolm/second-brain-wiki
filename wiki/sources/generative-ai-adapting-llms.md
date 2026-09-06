---
title: "Generative AI — Adapting LLMs with Parameter-Efficient Methods"
type: "source"
tags: ["research", "ai", "llm"]
sources: ["raw/10_Generative_AI__Adapting_LLMs_with_Parameter-Eff.md"]
entities: []
updated: 2026-09-05
sub_categories: []
---

# Generative AI — Adapting LLMs with Parameter-Efficient Methods

> Kuliah lanjutan LLM (kausal/AR): koreksi arsitektur GPT-3, skala vs data, context-window + RAG, dan LoRA sebagai adaptasi murah. Fondasi teknis untuk [[generative-ai-methods]].

## Key Claims (cited)

- Kausal LM ≠ BERT: embedding kontekstual → single dense linear + softmax atas vocab ~50k untuk next-word prediction [raw/10_Generative_AI__Adapting_LLMs_with_Parameter-Eff.md]
- GPT-1/2/3 sama secara arsitektur (transformer stack); GPT-3 terkenal karena scale network + scale data [raw/10_Generative_AI__Adapting_LLMs_with_Parameter-Eff.md]
- Context-window: moving-window baseline; ringkas-di-luar-window via LLM lain, lalu attach ke prompt [raw/10_Generative_AI__Adapting_LLMs_with_Parameter-Eff.md]
- RAG: embed FAQ (mis. via BERT), embed pertanyaan baru, ambil top-k (mis. 5 dari 10.000) yang paling mirip, pack ke prompt [raw/10_Generative_AI__Adapting_LLMs_with_Parameter-Eff.md]
- LoRA: delta-W (mis. 8000×8000=64M) ≈ perkalian dua matriks kurus (8000×2); ~16.192 params ≈0,02%; freeze base, latih adapter di 1–2 GPU (LLaMA 7/13B di single Colab GPU) [raw/10_Generative_AI__Adapting_LLMs_with_Parameter-Eff.md]
- Kualitas data: loop caption 2–3x (dedup 44942→15440 kata) — angka 8000/64M ilustratif, bukan spesifikasi model rilis [raw/10_Generative_AI__Adapting_LLMs_with_Parameter-Eff.md]

## Concepts & Entities Touched

- [[generative-ai-methods]] — AR-LM, RAG, LoRA
- [[ai-supercycle-economics]] — efisiensi fine-tune menurunkan biaya adopsi (sisi permintaan CapEx)
- [[pipeline-data-quality]] — loop caption

## Open Questions

- Versi GPT/LLaMA tepat dan tahun kuliah tak disebut di transkrip — cek silabus.

## References

[^1]: raw/10_Generative_AI__Adapting_LLMs_with_Parameter-Eff.md
