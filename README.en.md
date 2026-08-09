# Kim Taekyoung (김태경)

🇰🇷 [한국어](README.md) · 🇬🇧 English

**Developer aiming for Hospital Information Systems (HIS) and medical IT**
Dept. of Medical IT Engineering, Konyang University · **Expected graduation: Feb 2027**

I solve problems from real medical settings with deep learning and the web.
While still an undergraduate, I published **two conference papers as first author**, and carried the medical-imaging AI topic all the way to working systems — once as a solo research project and once as a graduation team capstone.
In an industry–academia R&D project, I owned the data workstream, designing and building an AI training dataset for food inspection.

- **Interests** — Hospital Information Systems (HIS), medical data, medical imaging AI
- **Contact** — taeral04@gmail.com

---

## Medical Imaging AI — from paper to system

### 1. Conference paper — closing the domain gap in AI sperm analysis (KKITS 2026)

> *Practical Domain Adaptation for Computer-Aided Sperm Analysis: Quality-Aware Video Normalization and Augmentation-Based Morphology Classification*
> **Kim Taekyoung (first author)**, Heo Yongdo (corresponding author) — Dept. of Medical IT Engineering, Konyang University
> Proceedings of KKITS, Vol. 20, No. 1 (2026)

The paper tackles a failure mode of computer-aided sperm analysis (CASA) models: **they work on clean benchmarks but collapse on real clinical footage.**
A morphology classifier trained on the benchmark dataset (MHSMA) saw its normal-morphology rate collapse to 0.5% when applied to real microscope videos (VISEM-Tracking) — and we fixed it using only methods with zero inference-time cost.

| Problem | Approach | Result |
|---|---|---|
| Detection degradation | **No pixel-level correction** (no CLAHE / grayscale); unify only resolution, fps, and clip-length specs | Detection **retained at 99.3%** of原 baseline (pixel correction cost −28.6%p) |
| Morphology collapse | `VisemStyleAugment` — training-time-only augmentation that mimics real-footage degradation | Real-world normal morphology rate **0.5% → 16.3%** (meets WHO ≥4% criterion) |

The conclusion came only after four alternatives — pseudo-labeling, geometric measurement, TTA, and ensembling — were tried first and all failed; the failure log is published in the paper as well.
Validated on footage from 4 real participants (1,824 sperm crops): all met the WHO criterion.

<br/>

### 2. AI-CASA — taking the paper to a web service (solo)

**[sperm-ai](https://github.com/MoriochoRadio/sperm-ai)** · `v1.4.0`

A Flask web system that takes a single microscope video and produces an integrated motility / kinematics / morphology analysis with a WHO 6th-edition report. Planned, modeled, and built end-to-end by myself.

- **Pipeline** — YOLO11 (detection) → ByteTrack (tracking) → ensemble regression (motility) → EfficientNet-B3 (morphology) → explanatory interpretation
- **Results** — On the same dataset (VISEM), motility MAE of **6.9%p** — lower error than the best published result (motilitAI, 7.31%p). YOLO11 mAP@0.5 = 0.677
- **Why it matters** — an assistive analysis tool that needs only a standard microscope video and a browser, no dedicated CASA equipment

<br/>

### 3. SEED — graduation team capstone, system design & integration (2026-1)

**[seed-project](https://github.com/MoriochoRadio/seed-project)** · `Ver 1.0.0`

The solo research above, scaled into a 5-person team system for automatic sperm detection, morphology, and motility analysis. The team set performance targets above the parent paper, met all of them, and completed the final presentation.

- **Role (ENG1)** — system architecture design, module integration, performance improvement, morphology model implementation
- **Tech** — Python · PyTorch · YOLO11 · ByteTrack · Flask
- **Process** — Waterfall methodology with stage-by-stage deliverables and verification documents / Team T.O.P (PM · CM · QA · ENG1 · ENG2)

---

## Industry–Academia R&D — AI food vision inspection (2025)

> **Data Collection Design and Implementation for an AI Food Vision Inspector: A Hardtack Case Study**
> Kim Taekyoung, Kim Minji, Han Juhyeok, Cho Yongseok — IEIE (Institute of Electronics and Information Engineers) 2025 Fall Conference (Nov 2025) · **First author**

In a company-partnered project building an affordable AI inspection system for small food manufacturers, I owned the **data collection and definition** workstream.
The job was not building the model but **defining what the model would learn** — where I learned to design decision criteria from documented grounds.

- **Norm-based defect classes** — defined 4 classes (normal / broken / over-baked / foreign object) against Codex, UNICEF, and Korean MFDS standards plus public-health evidence. No arbitrary splits: every class carries international/domestic regulatory references
- **Quantitative judgment criteria** — numeric rules labelers can't waver on: "broken-minor = outer 10–20%, split = 2 pieces, fragmented = 3+ pieces", "browning area bands at 30%/70%", "foreign objects from 6–8px". Includes exception rules (reflections/shadows are not defects) and class-priority rules for compound defects
- **Dataset construction** — 4,066 single-object 224×224 images (~1,000 per class) + 200 production-line-style multi-object images. Also designed the conveyor shooting protocol (density, arrangement, lighting, motion blur, empty-background shots)
- **Labeling & versioning pipeline** — Roboflow manual + semi-automatic labeling (Box Prompting, Label Assist), with per-version records of splits/preprocessing/augmentation/corrections for reproducibility. Exported to YOLO, COCO, and TFRecord for environment-independent use

📂 The full design record — defect definition grounds, quantitative criteria, shooting protocol — is documented here → **[food-vision-dataset-design](https://github.com/MoriochoRadio/food-vision-dataset-design)**

<sub>※ The project dataset and internal deliverables are company property and are not public.</sub>

---

## Competitions & Challenges

| When | Competition | What I did | Result / Status |
|---|---|---|---|
| 2026-06 | Multimodal AI Bias Challenge (DACON) — [multimodal-bias-vqa](https://github.com/MoriochoRadio/multimodal-bias-vqa) | VQA that answers "unknown" when evidence is insufficient — offline Qwen2.5-VL (4-bit) + balanced chain-of-thought prompt. Built a 600-sample validation set from public BBQ and iterated through 10 logged experiments | Public **Balanced Accuracy 0.883** |
| 2026-07 | 4th JUMP AI Drug-Development Challenge — [jump-ai-clinical-agent](https://github.com/MoriochoRadio/jump-ai-clinical-agent) | Proposed a clinical-trial protocol pre-review agent with a reproducible CLI prototype. Public/synthetic data only, explicit safety boundaries | Proposal submitted (2026-07-08) |

---

## University Team Projects

From hospital-queue and care apps to medical imaging AI and a complete medical AI system — scope grew step by step across five semesters in three years.

| When | Project | Domain | My role |
|---|---|---|---|
| 2024-1 | [MedQueue](https://github.com/MoriochoRadio/MedQueue) | Real-time hospital waiting info | System design |
| 2024-2 | [SchoolbusRFID](https://github.com/MoriochoRadio/SchoolbusRFID) | Location-based child drop-off safety | Android · RFID |
| 2024-2 | [ElderCaringApp](https://github.com/MoriochoRadio/ElderCaringApp) | Health monitoring for seniors living alone | Load-cell HW + statistics SW |
| 2025-1 | [LungCT3DNoduleAI](https://github.com/MoriochoRadio/LungCT3DNoduleAI) | Lung CT nodule detection (accuracy 78%) | PM |
| 2025-2 | [AILungandLiver](https://github.com/MoriochoRadio/AILungandLiver) | Lung + liver CT nodule detection (accuracy 93%) | QA |
| 2026-1 | **[SEED](https://github.com/MoriochoRadio/seed-project)** | Integrated AI sperm detection · morphology · motility | **ENG1** (design · integration · performance) |

The 2025 medical-imaging line (LungCT → AILungandLiver) is one system evolved over two semesters by the same team.
**I deliberately switched roles from PM to QA** to experience both building and verifying.

---

## Personal Projects — experiments in shipping with LLMs and automation

These exist to build the muscle of **wiring LLMs, automation, and the web into products that actually run**.
The backbone pattern is `data collection → LLM analysis → static-site auto-deploy`, running on GitHub Actions with zero servers and zero operating cost, refreshing daily.
I repeated the same pattern across finance, gaming, and healthcare domains to learn where automation holds up and where a human is still needed — plus a few side experiments like a serverless PWA and artificial-life simulations.

| Project | Domain | What it is | Stack |
|---|---|---|---|
| [stock-briefing](https://github.com/MoriochoRadio/stock-briefing) · [demo](https://moriochoradio.github.io/stock-briefing/) | Finance | Daily US/KR market briefing auto-generated and deployed as a dashboard | Actions · Gemini · Astro |
| [ai-daily-trends](https://github.com/MoriochoRadio/ai-daily-trends) · [demo](https://moriochoradio.github.io/ai-daily-trends/) | Data | Daily auto-collection of AI trends from GitHub Trending, HN, Reddit | Python · collection pipeline |
| [tarkov-companion](https://github.com/MoriochoRadio/tarkov-companion) · [demo](https://moriochoradio.github.io/tarkov-companion/) | Web app | Real-time price/value analysis + daily automated briefing | TypeScript · Actions · LLM |
| [sauna-science-hub](https://github.com/MoriochoRadio/sauna-science-hub) · [demo](https://moriochoradio.github.io/sauna-science-hub/) | Healthcare | 90 PubMed papers auto-collected + Korean-translated archive | Python · PubMed API |
| [tarkov-korean-changes](https://github.com/MoriochoRadio/tarkov-korean-changes) · [demo](https://moriochoradio.github.io/tarkov-korean-changes/) | Data | Daily auto-collection and Korean interpretation of silent game-code changes, with automatic stability assessment of recurring events | Python · Actions · LLM |
| [fundamental-regime-report](https://github.com/MoriochoRadio/fundamental-regime-report) | Finance | Corporate fundamentals + market-regime-aware integrated analysis reports | Python · Claude API |
| [weather-fit](https://github.com/MoriochoRadio/weather-fit) · [demo](https://moriochoradio.github.io/weather-fit/) | Web app | Weather-based men's outfit recommendations — 75 outfits by temperature band, static PWA with no server or API keys | TypeScript · PWA |
| [mindlings](https://github.com/MoriochoRadio/mindlings) | Simulation | God-view artificial-life sandbox — observe and intervene with NEAT neural-network creatures | Godot 4 · GDScript |
| [evolution-garden](https://github.com/MoriochoRadio/evolution-garden) · [demo](https://moriochoradio.github.io/evolution-garden/) | Simulation | 137-weight neural networks speciating through mutation and natural selection alone. Single HTML file, no libraries | Vanilla JS · Canvas |

---

## Study Archives

Repositories that preserve coursework and self-study as-is. They show a **learning trajectory** rather than polish.

[study-algorithms](https://github.com/MoriochoRadio/study-algorithms) (algorithms, C++/C#) ·
[study-java](https://github.com/MoriochoRadio/study-java) (Java basics→GUI) ·
[study-windows-programming](https://github.com/MoriochoRadio/study-windows-programming) (WinForms/WPF, 34 chapters) ·
[web-study-notes](https://github.com/MoriochoRadio/web-study-notes) (job-academy front-end/back-end · [progress dashboard](https://moriochoradio.github.io/web-study-notes/)) ·
[Iot-Github](https://github.com/MoriochoRadio/Iot-Github) (Zynq-board IoT practice) ·
[study-web-basics](https://github.com/MoriochoRadio/study-web-basics) · [study-web-funsun](https://github.com/MoriochoRadio/study-web-funsun) (2020, first web)

---

## Tech Stack

| Area | Tech |
|---|---|
| **Primary** | Python · PyTorch · YOLO11 / Ultralytics · ByteTrack · Flask |
| **Web** | TypeScript · JavaScript · Astro · Tailwind CSS · Streamlit |
| **Foundations** | C · C++ · Java · C# · SQL |
| **Data** | Roboflow · dataset design & labeling criteria · versioning |
| **Infra** | GitHub Actions · GitHub Pages · Firebase · Git · Jupyter |
| **LLM** | Claude API · Gemini API · GitHub Models · agent workflows · prompt engineering |

---

<sub>Each repository README documents team composition, roles, and architecture — along with <b>what I personally did and did not do, and the attempts that failed</b>.</sub>
