# Kim Taewoong (김태웅) — AI / NLP Researcher

**Medical LLM (Generative Medical Record) — research & on-premise serving**
AI/NLP researcher who trains, quantizes, and serves a medical LLM used by **100+ concurrent users**, deployed to **hospital closed networks (on-premise)** where cloud APIs are not allowed. 2019.11–present (6+ yrs).
🏅 **Kaggle Competitions Expert · top 0.7% (1,435 / 210,968)**

---

## Summary
- **On-premise medical LLM serving — 100+ concurrent users inside hospital closed networks (self-hosted GPU).** Cloud APIs are banned in hospitals, so the full train→quantize→serve loop runs on-prem. Core differentiator.
- End-to-end LLM: fine-tuning (SFT·LoRA, RL: DPO/GRPO), quantization (GPTQ/AWQ/W4A16), vLLM serving; multi-GPU training up to H200×8, serving 24B–80B models.
- Kaggle (solo): math-problem classification **3rd / 338**, AIMO Progress Prize 2 **Silver (87 / 2212)**. Competitions Expert (top 0.7%).
- Consistent medical-domain track: Korean medical NLP → precision-medicine R&D → medical LLM.

---

## Experience

### Puzzle AI — AI / NLP Researcher · Nov 2019 – Present (6+ yrs)
Owns training, quantization and **on-premise serving** of a medical LLM (Generative Medical Record) — **100+ concurrent users, deployed inside hospital closed networks** (cloud not allowed).
- On-prem serving — LLM on hospital closed-network / self-hosted GPU, **dual-server round-robin HA for 100+ concurrent users** (key strength)
- Fine-tuning of Gemma 2/3/4 · Qwen · GPT-OSS (LoRA, RL: DPO/GRPO); multi-GPU training up to **H200×8**, served **24B–80B** models to GPU budgets
- Quantization (GPTQ/AWQ/W4A16) for speed & VRAM — solved Gemma-4 AWQ (no official recipe), ~2.5× inference speed
- vLLM serving & reproducibility debugging; stabilized structured (JSON) output via GBNF constrained decoding; serving image build 30 min → 11 s
- GMR backend (FastAPI + vLLM) — multiple clinical-document summarization APIs (surgery / admission / discharge), map-reduce long-document summarization & generation-repetition control, standardized router error-code spec
- Asan / Chungnam Nat'l Univ. hospital pipelines (SOAP · discharge · surgery records); **fine-tuned an LLM on 5 years of surgery records (A6000, on-prem)**; on-site demos
- **Introduced & established vLLM** as the team's LLM serving stack (structured output, serving image, quantized serving); upgraded embedding & reranker models (separate KO/EN embeddings) for retrieval quality
- Earlier (2019.11–2024): Korean medical NLP → precision-medicine R&D (variant / survival analysis, symptom extraction)
- Open source: reported 4 Gemma-related bugs to vLLM · SGLang · llm-compressor

---

## Projects

### Beauty / Health AI Product (side project) · 2024 – present
Drove development of a beauty/health AI product — shipped a real-time voice assistant, scalp/skin-diagnosis CV, and on-device shorts auto-generation; owned spec & review while **AI coding agents** did most of the implementation.
- Real-time **ambient voice assistant** (OpenAI Realtime API, WebSocket) — live STT / translation, sentence-boundary & endpoint tuning
- **Scalp diagnosis CV** — reproduced ScalpVision (macro-F1 **0.744** > paper 0.689)
- **Facial skin diagnosis (8 attributes)** — per-attribute ConvNeXt-Tiny + **CORAL ordinal** models on dermatologist-graded data (AI-Hub, 1,072 subjects / ~14k images); deployment MAE **~0.49**, **~94% within ±1 grade**
- Aligned train/inference crops with MediaPipe landmarks for deployment accuracy → shipped **8 ONNX models on-device**
- **On-device shorts auto-generation & rendering** — generation-progress UI, dynamic editing (fade-out, frozen-frame trim, segment clamping), background music, session persistence
- CRM / admin dashboards, QR login & session management, camera face-warp filters, face-similarity, casual games (Bubble Pop, Beauty Merge)

### Conversational AI Service (side project) · May 2023 – Jan 2024
Sole AI/ML engineer on a multi-modal conversational AI service — designed, built and shipped the entire AI feature set (emotion analysis, voice/video generation, NLP tooling).
- **Emotion classifier** — hand-labeled ~1,500 samples myself, KoELECTRA 7-class, **0.06 s CPU inference**; Optuna search
- **Multi-modal AI** — TTS / voice-cloning, talking-head video, image captioning, speech enhancement, image generation (API integration + tuning)
- **NLP tooling** — repetition avoidance via embedding similarity, profanity / text moderation, sentence splitting
- Multi-stage character-creation prompt engineering; closed beta (27 users) data analysis; end-to-end service QA & release testing

---

## Competitions · Kaggle (solo)
**Competitions Expert — top 0.7% worldwide (1,435 / 210,968)**

### KAChallenges: Classifying Math Problems — 3rd / 338 · May 2025
8-topic math-problem classification (NLP). Reframed generative classification as **constrained decoding** — a Logits Processor restricts output to label tokens, with temperature=0 · max_tokens=1 (single deterministic token) to eliminate format errors. Qwen3-32B / Qwen2.5-32B-AWQ on vLLM + 32B domain fine-tuning. → [Official 3rd-place solution writeup](https://www.kaggle.com/competitions/classification-of-math-problems-by-kasut-academy/writeups/3rd-place-solution)

### AIMO Progress Prize 2 — Silver, 87 / 2212 · Nov 2024 – Mar 2025
Olympiad-level math reasoning. Fine-tuned DeepSeek-R1-Distill-Qwen-7B, then AWQ-quantized; vLLM batch inference. Multi-sample per question → majority-vote self-consistency; token-budget management to maximize samples within the time limit.

*Also: Eedi · Nemotron · Deep Past and other LLM inference-optimization competitions.*
*Official certificates: KAUST Academy (3rd/338), Kaggle (AIMO2 Silver).*

---

## Skills
- **Language:** Python
- **LLM / GenAI:** Fine-tuning & training (SFT·LoRA), RL (DPO/GRPO) experience, quantization (GPTQ/AWQ/W4A16), vLLM serving & on-prem deployment, structured (JSON) output fixes, RAG · retrieval (embedding search · reranking)
- **NLP / CV / Data:** Korean medical text processing/classification · PyTorch image-classification model training & paper reproduction · data analysis (pandas) & labeling
- **Serving / Infra:** vLLM · FastAPI, Docker, Kubernetes / Ceph (rook), on-prem (closed-network) GPU serving, W&B
- **AI agents:** Highly proficient with AI coding agents (Claude, GPT/Codex) — drives large-scale implementation via agents while owning spec, architecture, review & verification. (Puzzle AI early/mid code, Kaggle solutions, data labeling & model training are all done by hand.)

---

## Community · Leadership
**learnup study group — Organizer/Leader** (Somoim app), 2025 – 2026 (1-year milestone Jan 30, 2026). Grew and sustained a 50+ member group for over a year; ran daily in-person meetups (after-work cafe), owning scheduling, venue & facilitation.

## Education
—

## Links
Kaggle [kaggle.com/aleaiest](https://www.kaggle.com/aleaiest) · Hugging Face [huggingface.co/qwertist](https://huggingface.co/qwertist) · Email dxodnd@gmail.com
