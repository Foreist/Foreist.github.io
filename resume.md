# Kim Taewoong (김태웅) — AI / NLP Researcher

**Medical LLM (Generative Medical Record) — research & on-premise serving**
AI/NLP researcher who trains, quantizes, and serves a medical LLM used by **100+ concurrent users**, deployed to **hospital closed networks (on-premise)** where cloud APIs are not allowed. 2019.11–present (6+ yrs).
🏅 **Kaggle Competitions Expert · top 0.7% worldwide**

---

## Summary
- **On-premise medical LLM serving — 100+ concurrent users inside hospital closed networks (self-hosted GPU).** Cloud APIs are banned in hospitals, so the full train→quantize→serve loop runs on-prem. Core differentiator.
- End-to-end LLM: fine-tuning (SFT·LoRA, RL: DPO/GRPO), quantization (GPTQ/AWQ/W4A16), vLLM serving; fine-tuned open-weight LLMs up to 100B+ parameters.
- Kaggle Competitions Expert (**top 0.7%** worldwide) — math-problem classification **3rd**, AIMO Progress Prize 2 **Silver**, ARC Prize 2024 **Bronze**. Zindi · FAO/ITU satellite pond detection **13th**.
- Consistent medical-domain track: Korean medical NLP → precision-medicine R&D → medical LLM.

---

## Experience

### Puzzle AI — AI / NLP Researcher · Nov 2019 – Present (6+ yrs)
Owns training, quantization and **on-premise serving** of a medical LLM (Generative Medical Record) — **100+ concurrent users, deployed inside hospital closed networks** (cloud not allowed).
- On-prem serving — LLM on hospital closed-network / self-hosted GPU, **redundant dual-server setup for 100+ concurrent users** (key strength)
- Fine-tuning open-weight LLMs up to **100B+ parameters** (LoRA, RL: DPO/GRPO); multi-GPU distributed training, serving sized to GPU budgets
- Quantization (GPTQ/AWQ/W4A16) for speed & VRAM — built an AWQ recipe for a model family with no official support, ~2.5× inference speed
- vLLM serving & reproducibility debugging; stabilized structured (JSON) output via GBNF constrained decoding; serving image build 30 min → 11 s
- GMR backend (FastAPI + vLLM) — multiple clinical-document summarization APIs (surgery / admission / discharge), map-reduce long-document summarization & generation-repetition control, standardized router error-code spec
- Tertiary-hospital record pipelines (SOAP · discharge · surgery records); **fine-tuned an LLM on multi-year surgery-record corpora, on-prem**; on-site demos
- **Introduced & established vLLM** as the team's LLM serving stack (structured output, serving image, quantized serving); upgraded embedding & reranker models (separate KO/EN embeddings) for retrieval quality
- **CDSS with a small LLM** (2023.10–2024.12) — clinical decision support for hospital use: generated & labeled training data with GPT, fine-tuned an open LLM, converted for on-prem deployment
- **Precision-medicine R&D** (2020.11–2023.02, university-hospital collaboration) — blood-cancer mutation research: literature survey, data collection, preprocessing, analysis and modeling
- Earlier (2019.11–2020): Korean medical NLP — symptom extraction and medical text classification
- Open source: reported 4 upstream bugs to vLLM · SGLang · llm-compressor

---

## Projects

### Beauty / Health AI Product (side project) · Sep 2025 – present
Drove development of a beauty/health AI product — shipped a real-time voice assistant, scalp/skin-diagnosis CV, and on-device shorts auto-generation; owned spec & review while **AI coding agents** did most of the implementation.
- Real-time **ambient voice assistant** — live STT / translation, sentence-boundary & endpoint tuning
- **Scalp diagnosis CV** — reproduced a published benchmark and beat it (macro-F1 **0.744** vs 0.689)
- **Facial skin diagnosis (8 attributes)** — per-attribute ordinal-grading models; deployment MAE **~0.49**, **~94% within ±1 grade**
- Tuned train/inference preprocessing for deployment accuracy → shipped **8 models on-device**
- **On-device shorts auto-generation & rendering** — generation-progress UI, dynamic editing (fade-out, frozen-frame trim, segment clamping), background music, session persistence

### Conversational AI Service (side project) · May 2023 – Jan 2024
AI/ML engineer on a multi-modal conversational AI service — built and shipped AI features (emotion analysis, voice/video generation, NLP tooling).
- **Emotion classifier** — hand-labeled ~1,500 samples myself, 7-class, **0.06 s CPU inference**; hyperparameter search
- **Multi-modal AI** — TTS / voice-cloning, talking-head video, image captioning, speech enhancement, image generation (API integration + tuning)
- **NLP tooling** — repetition avoidance via embedding similarity, profanity / text moderation, sentence splitting
- Multi-stage character-creation prompt engineering; closed beta (100 users) data analysis; end-to-end service QA & release testing

---

## Competitions (solo)

- **Kaggle Competitions Expert · top 0.7% worldwide**
  - **Kaggle math-problem classification — 3rd place** (May 2025). Reframed generative classification as **constrained decoding** — a Logits Processor restricts output to label tokens, temperature=0 · max_tokens=1, eliminating format errors. → [Official 3rd-place solution writeup](https://www.kaggle.com/competitions/classification-of-math-problems-by-kasut-academy/writeups/3rd-place-solution)
  - **Kaggle AIMO Progress Prize 2 — Silver medal** (Mar 2025). Fine-tuned and quantized a reasoning model for batch inference; multi-sample majority-vote self-consistency under a strict token budget.
  - **Kaggle ARC Prize 2024 — Bronze medal** (Nov 2024). Abstract reasoning on unseen tasks.
- **Zindi · FAO/ITU satellite aquaculture-pond detection — 13th place** (Aug 2026). Heavy domain shift between train and test, so I validated directly on the leaderboard: **test-time self-training** raised the public score **0.916 → 0.941**, and picking final submissions for variance rather than rank survived the private shakeup.

*Also: Eedi · Nemotron · Deep Past and other LLM inference-optimization competitions.*

---

## Skills
- **Language:** Python
- **LLM / GenAI:** Fine-tuning & training (SFT·LoRA), RL (DPO/GRPO) experience, quantization (GPTQ/AWQ/W4A16), vLLM serving & on-prem deployment, structured (JSON) output fixes, RAG · retrieval (embedding search · reranking)
- **NLP / CV / Data:** Korean medical text processing/classification · PyTorch image-classification model training & paper reproduction · data analysis (pandas) & labeling
- **Serving / Infra:** vLLM · FastAPI, Docker, Kubernetes, on-prem (closed-network) GPU serving, W&B
- **AI agents:** Highly proficient with AI coding agents (Claude, GPT/Codex) — drives large-scale implementation via agents while owning spec, architecture, review & verification. (Puzzle AI early/mid code, Kaggle solutions, data labeling & model training are all done by hand.)

---

## Community · Leadership
**learnup study group — Organizer/Leader** (Somoim app), Feb 2025 – Apr 2026 (1-year milestone Jan 30, 2026). Grew and sustained a 50+ member group for over a year; ran daily in-person meetups (after-work cafe), owning scheduling, venue & facilitation.

## Education
—

## Links
Kaggle [kaggle.com/aleaiest](https://www.kaggle.com/aleaiest) · Zindi [zindi.africa/users/Foreist](https://zindi.africa/users/Foreist) · Hugging Face [huggingface.co/qwertist](https://huggingface.co/qwertist) · Email dxodnd@gmail.com
