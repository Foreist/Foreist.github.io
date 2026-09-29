# Kim Taewoong (김태웅) · AI / NLP Researcher

**Medical LLM training, quantization, and on-prem serving · Puzzle AI, Nov 2019 – Sep 2026**
**Kaggle top 0.2%** · Competition medals 🥇 2 · 🥈 1 · 🥉 1

> 한국어 버전: [resume.md](resume.md)

---

## Summary

- Deployed a medical LLM on GPU servers inside hospital closed networks, serving **100+ concurrent users**
- Full LLM pipeline from fine-tuning 100B+ open-weight models to quantization and vLLM serving
- Built a QR receipt-voucher service solo; **launched commercially in 2026 and in live operation**
- Zindi GeoAI aquaculture-pond detection **gold**
- Kaggle top 0.2%: AI Agent Security **gold**, math-problem classification **3rd**, AIMO Progress Prize 2 **silver**, ARC Prize 2024 **bronze**

---

## Experience

### Puzzle AI · AI / NLP Researcher · Nov 2019 – Sep 2026 (6 yrs 10 mo)

Trained, quantized, and deployed a medical LLM for clinical record generation inside hospitals.

- Deployed LLMs on hospital closed-network GPU servers with a redundant setup for **100+ concurrent users**
- Fine-tuned open-weight LLMs up to **100B+ parameters** (LoRA, DPO/GRPO) with multi-GPU training
- Built an AWQ quantization recipe for a model family with no public recipe, **~2.5× faster inference**
- Moved the team's LLM serving stack to vLLM; stabilized JSON output with grammar-constrained decoding
- Built a long clinical-document summarization backend; improved retrieval by replacing embedding and reranker models
- Built a fine-tuning pipeline on real hospital records; ran on-site hospital demos
- **Lightweight LLM clinical decision support (CDSS)** (Oct 2023 – Dec 2024): training-data generation and labeling, open LLM fine-tuning, on-prem deployment
- **Precision-medicine R&D** (Nov 2020 – Feb 2023, university-hospital collaboration): blood-cancer mutation data collection, preprocessing, analysis, and modeling
- Early (2019 – 2020): Korean medical NLP, symptom extraction and medical text classification

---

## Projects

### QR Receipt Voucher · Own business · 2026 – present

A voucher-refund web service for participating stores. Customers upload a receipt photo through an in-store QR code; the service reads the amount and receipt number, determines eligibility, records issuance, blocks duplicate claims, and provides admin screens.

- **Launched commercially in 2026 and in live use at participating stores**
- Planned, built, deployed, and operate it **solo** (GitHub Actions CI, AWS)

### Beauty / Health AI Product · Sep 2025 – present

AI development lead for a beauty/health AI product. Shipped a real-time voice assistant, scalp and skin diagnosis, and on-device short-video generation.

- Real-time voice assistant: live STT and translation, end-of-speech detection tuning
- Scalp diagnosis: reproduced a public benchmark and reached **macro-F1 0.744** (vs 0.689)
- Facial skin diagnosis across 8 attributes: per-attribute grading models, deployed **MAE ~0.49, ~94% within ±1 grade**
- Aligned training and inference preprocessing to improve deployed accuracy; shipped **8 on-device models**
- On-device short-video generation and rendering (auto-editing, background music, progress UI)

### Conversational AI Service (side project) · May 2023 – Jan 2024

AI/ML engineer on a multimodal conversational AI service. Built and shipped emotion analysis, voice/video generation, and NLP features.

- Emotion classifier: hand-labeled ~1,500 samples, 7 classes, **0.06 s CPU inference**
- Multimodal: TTS and voice cloning, talking-head video, image captioning, speech enhancement, image-generation API integration
- NLP: embedding-similarity repetition control, text moderation, sentence splitting
- Character-creation prompt design, closed-beta (100 users) data analysis, release QA

---

## Competitions (solo)

**Kaggle top 0.2%**

- **AI Agent Security (OpenAI) · Gold** (Sep 2026). LLM-agent red-team benchmark. Split final submissions across two different attack strategies in case the public leaderboard's top attack type was invalidated in final scoring
- **Math-problem classification (KAUST Academy) · 3rd** (May 2025). Reframed generative classification as constrained decoding so the model can only emit label tokens, eliminating format errors. [3rd-place solution writeup](https://www.kaggle.com/competitions/classification-of-math-problems-by-kasut-academy/writeups/3rd-place-solution)
- **AIMO Progress Prize 2 · Silver** (Mar 2025). Fine-tuned and quantized a reasoning model; multi-sample majority vote within a token budget
- **ARC Prize 2024 · Bronze** (Nov 2024). Abstract reasoning on unseen tasks

**Zindi GeoAI aquaculture-pond detection (FAO/ITU) · Gold** (Aug 2026). Large train/test domain gap, so applied test-time self-training: public score 0.916 → 0.941. Chose lower-variance final submissions to hold up in the private ranking

---

## Skills

- **Languages:** Python, TypeScript
- **LLM:** fine-tuning (SFT·LoRA), RL (DPO/GRPO), quantization (GPTQ/AWQ/W4A16), structured output, RAG and retrieval (embeddings, reranking)
- **Serving / Infra:** vLLM, FastAPI, Docker, Kubernetes, on-prem GPU serving, AWS, GitHub Actions, W&B
- **NLP / CV / Data:** Korean medical text processing, PyTorch image models and paper reproduction, pandas analysis, data labeling
- **Workflow:** implement with AI coding agents (Claude, Codex); own design, review, and verification

---

## Community

**learnup study group organizer** (Somoim app) · Feb 2025 – Apr 2026
Ran a 50+ member group for over a year; handled scheduling, venues, and facilitation for weekday evening in-person meetups

## Links

Kaggle [kaggle.com/aleaiest](https://www.kaggle.com/aleaiest) · Zindi [zindi.africa/users/Foreist](https://zindi.africa/users/Foreist) · Hugging Face [huggingface.co/qwertist](https://huggingface.co/qwertist) · Email dxodnd@gmail.com
