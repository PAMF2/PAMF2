<div align="center">
<img src="./assets/banner.svg" width="900" alt="Pedro Afonso"/>
</div>

<div align="center">

![Profile Views](https://komarev.com/ghpvc/?username=PAMF2&color=3b82f6&style=flat&label=profile+views)

</div>

I build systems that **learn to act, not just predict.** My focus is on objective-driven learning — training models through execution feedback instead of imitation, designing multi-agent pipelines that reason through explicit intermediate state, and building causally-aware memory that scales linearly without quadratic attention blowup. I ship end-to-end: from reward pipeline design and inference-time planning to production deployment in resource-constrained clinical environments.

Currently co-founding [MIOSA](https://miosa.ai) (self-learning agent platform, 7k downloads in 3 days) and leading AI at [Veredictos](https://www.veredictos.com/) (retinal disease screening, active pilots in public healthcare). Also building [PaymentsLine](https://www.paymentsline.com/), a payments layer for AI-native businesses. Senior AI/ML Engineer at Lunivate. Started consulting at 15.

### Achievements

| Achievement | Details |
|-------------|---------|
| 1st Place — CrewAI Agentic AI Challenge 2025 | Built DiabetesEye with Gabriel Maia. Only Brazilian team in the global top 10. Judges cited the combination of agentic AI with classical ML and low-level API control as the differentiator. |
| AWS Machine Learning Specialty Certified | Amazon Web Services, 2024 |
| Finalist — Brazilian Nuclear Olympiad 2025 | IRRAD[IA]: AI-controlled food irradiation with YOLOv8, dose optimization, and industrial safety loop |
| Participant — Arc × Circle Hackathon 2026 | BaaS Arc: autonomous 4-division banking syndicate with 110 production functions, DeFi, and sub-second settlement |
| MIOSA — 7k downloads in 3 days | Word of mouth only. Built on OSA, a local-first Elixir/OTP agent runtime |

### Currently Building

**[Veredictos](https://www.veredictos.com/)** — A retinal AI platform that screens for diabetic retinopathy, glaucoma, and hypertensive retinopathy from fundus images. The model (86.8M params, ViT + MedGemma) reached 94%+ sensitivity across all three diseases (GATE 1 passed) on 24K images from 18 datasets. Currently in integration pilots with Prefeitura do Rio de Janeiro (SUS) and Centro Carioca do Olho. Backed by NVIDIA Inception and Google for Startups.

**[PaymentsLine](https://www.paymentsline.com/)** — Payments infrastructure for AI-native businesses, built alongside Veredictos to support clinical billing and agentic transaction flows.

**[MIOSA](https://miosa.ai) / [OSA](https://github.com/PAMF2/OSA)** — OSA is a production local AI orchestrator in Elixir/OTP with hot-reload skills, PubSub event routing, Rust NIFs, and SQLite persistence. MIOSA is the commercial platform built on top of it — a self-learning agent that improves through usage.

### Research & Projects

**Medical AI**

| Project | Stack | Description |
|---------|-------|-------------|
| [Veredictos](https://www.veredictos.com/) | PyTorch · ViT · MedGemma | 86.8M parameter model — DR sensitivity 94.1%, glaucoma 94.3%, hypertensive retinopathy 95.3%, DR grading Kappa 0.775. Trained on 24K images from 18 datasets. CFM 2.454/2026 compliant. |
| [DiabetesEye](https://github.com/PAMF2/DiabetesEye) | CrewAI · Gemini · OpenCV | 1st place globally. Multi-agent pipeline that grades diabetic retinopathy from fundus images, outputs ETDRS classification and 6/12/24-month progression risk in under 30 seconds. Fully offline — built for underserved clinics. |
| [IRRAD[IA]](https://github.com/PAMF2/irrad-IA-) | YOLOv8 | Detects food type and geometry from camera, computes optimal Cobalt-60 irradiation dose per category, and blocks any out-of-range recommendation before processing. Built for industrial deployment. |

**RL & Research**

| Project | Stack | Description |
|---------|-------|-------------|
| [CodeForge ASM](https://github.com/PAMF2/codeforgefinal) | PyTorch · TRL · GRPO | Qwen3.5-2B trained from zero supervised labels to write correct x86-64 NASM assembly, using pure execution signal (nasm + ld + run). Two-phase GRPO on Kaggle T4x2. MCTS over candidate instruction sequences at inference time improves pass@k on out-of-distribution patterns. |
| [hackaton-claw](https://github.com/PAMF2/hackaton-claw) | Python · Claude | Dual-loop autonomous scientific analysis system. A strategic loop (Orchestrator + Plan Reviewer) decomposes goals into steps; a tactical loop (Code Planner + Executor + Reviewer) implements each step with retry on failure. All agents run on Claude. |
| MCU | Python | Linear-time causal memory architecture — O(N) scaling with built-in causal coherence, no quadratic attention. Proved epsilon-causal consistency with memory bounds M = O(D log N) via instrumental variable-based causal distance estimation. |

**Agent Infrastructure & Finance**

| Project | Stack | Description |
|---------|-------|-------------|
| [AEG](https://github.com/PAMF2/AEG) | Elixir · OTP | Production agent runtime with a full guard → plan → memory → model → eval → persistence pipeline. Agents plan multi-step sequences against a learnable world model before executing. Q-learning RL layer with epsilon-greedy policy. Adapters for OpenAI, Anthropic, Gemini, Ollama. |
| [OSA](https://github.com/PAMF2/OSA) | Elixir · OTP · SQLite | Local-first AI orchestrator — PubSub event routing, hot-reload skills, Rust NIFs, file system watcher. Open-source alternative to OpenClaw. Powers MIOSA. |
| [BaaS Arc](https://github.com/PAMF2/ARC) | Python · Gemini | Autonomous 4-division banking syndicate (Front Office, Risk, Treasury, Clearing). 110 production functions. Every transaction cleared through all four agents before settling. Gemini-powered fraud detection, OFAC/PEP screening, DeFi yield farming, sub-second RTP/FedNow settlement. |
| [ASP](https://github.com/PAMF2/asp) | Python | Adversarial Semantic Protection — LLM prompt injection detection engine using 3D Gaussian probability fields and morphological intent detection. Minimal dependencies by design. |

### Stack

<div align="center">

[![Stack](https://skillicons.dev/icons?i=python,pytorch,cpp,elixir,rust,typescript,aws,docker)](https://skillicons.dev)

</div>

**RL & Training** — GRPO · PPO · MCTS · TRL · LoRA/QLoRA · reward modeling · DQN  
**Vision & Medical** — YOLOv8 · OpenCV · TransUNet · EfficientNet-B3 · UNet++ · MedGemma  
**Agents** — CrewAI · LangChain · LlamaIndex · Elixir/OTP · MoE · RAG · world-model loops  
**Infra** — AWS · Docker · Kubernetes · FastAPI · PostgreSQL · Redis · Vector DBs · MLOps

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=PAMF2&show_icons=true&theme=github_dark&hide_border=true&count_private=true&bg_color=0d1117&title_color=3b82f6&icon_color=3b82f6)
&nbsp;
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=PAMF2&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=3b82f6)

</div>

<div align="center">
<img src="https://raw.githubusercontent.com/PAMF2/PAMF2/output/github-contribution-grid-snake-dark.svg" alt="snake"/>
</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:1d2d44&height=60&section=footer" width="100%"/>
