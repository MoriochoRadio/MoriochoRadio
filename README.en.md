# Kim Taekyoung (김태경) — Backend Developer (Java · Spring Boot)

🇰🇷 [한국어](README.md) · 🇬🇧 English

Preparing to work as a **backend developer focused on medical IT and healthcare solutions**.
Dept. of Medical IT Engineering, Konyang University — expected graduation Feb 2027 (GPA 4.30 / 4.5) · currently in a full-stack developer bootcamp (since Jun 2026)

📧 **taeral04@gmail.com**

I want to own the path along which data is created, processed and delivered — the part users never see.
Across six team design projects (2024–2026, five semesters) I worked as engineer, PM and QA, learning to turn requirements into structure and verify it end to end.
Now I am building the skills to make that path more solid with Java, Spring Boot and relational databases.

---

## Tech stack

| Area | Tools | Where I used them |
|---|---|---|
| **Backend** | ![Java](https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?logo=springboot&logoColor=white) ![MyBatis](https://img.shields.io/badge/MyBatis-B22222) ![JSP/Servlet](https://img.shields.io/badge/JSP%20%2F%20Servlet-007396) ![MariaDB](https://img.shields.io/badge/MariaDB-003545?logo=mariadb&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white) ![SQLite](https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=white) | Bootcamp — Spring Boot board improvement assignment (attachments, author permissions, config separation, transaction rollback) run and verified on a local MariaDB; Java Texas Hold'em |
| **Frontend** | ![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) ![CSS](https://img.shields.io/badge/CSS-1572B6?logo=css&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white) ![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black) ![Next.js](https://img.shields.io/badge/Next.js-000000?logo=nextdotjs&logoColor=white) | Next.js 16 real-time stock dashboard (Finnhub REST/WebSocket · Zustand · Recharts), serverless static web apps |
| **Python · AI** | ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white) ![Flask](https://img.shields.io/badge/Flask-000000?logo=flask&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white) ![pydicom](https://img.shields.io/badge/pydicom-4B8BBE) | SEED four-layer pipeline (co-designed with ENG2) and integration with a Flask report, DICOM → HU → 3D mesh preprocessing, domain-adaptation experiments → first-author paper |
| **Collaboration · infra** | ![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white) ![Firebase](https://img.shields.io/badge/Firebase-FFCA28?logo=firebase&logoColor=black) ![Linux](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black) ![Android](https://img.shields.io/badge/Android-3DDC84?logo=android&logoColor=white) ![C# · Xamarin](https://img.shields.io/badge/C%23%20%C2%B7%20Xamarin-512BD4?logo=dotnet&logoColor=white) | Daily auto-collecting sites on GitHub Actions (failure diagnosis, self-recovery), three Firebase real-time sync apps, 104 pages of requirements/design/quality/risk documents as lead author (incl. co-authored) |

<sub>I use AI coding tools throughout. Choosing the technology, deciding the structure and verifying the result are my job; AI-written code goes in only after I have run and tested it.</sub>

---

## Featured projects

### 1. SEED — AI sperm detection with integrated morphology and motility analysis

| | |
|---|---|
| **Why** | Manual reading varies by examiner, CASA equipment is expensive, and morphology is still read by hand. The goal: integrated morphology and motility judgments on the same sperm from ordinary microscope video. |
| **Period · team · role** | Mar–Jun 2026 (15 weeks, capstone) · 5 people · **ENG1** — system architecture (co-designed with ENG2), inter-layer interface definitions, integration of 8 modules built in parallel by 4 people, morphology model |
| **Stack** | Python · PyTorch · YOLO11 · ByteTrack · EfficientNet-B3 · scikit-learn · Flask |
| **Highlights** | Four-layer pipeline: input normalization → detection/tracking → motility regression and morphology classification → WHO judgment. All three targets fixed before kickoff were met — motility MAE 6.90%p (below the prior study's 7.31%p), detection mAP@50 0.677, morphology AUC 0.725 |
| **Review** | The benchmark's best model produced a 0.5% normal-morphology rate on real footage; models must be chosen by whether they work in the field, not by score. Fixing interfaces in documents first is what made parallel development possible. |
| **Code** | **[seed-project](https://github.com/MoriochoRadio/seed-project)** · solo baseline [sperm-ai](https://github.com/MoriochoRadio/sperm-ai) |

### 2. L-POT — AI diagnostic aid and 3D visualization for liver and lung CT

| | |
|---|---|
| **Why** | Commercial CT reading aids are all built for clinicians. We aimed at a reference tool that helps patients see and understand their own CT in 3D. |
| **Period · team · role** | Mar–Jun 2025 · 6 people · **PM** + data preprocessing → Aug–Dec 2025 · 5 people · **QA**. The same system over two semesters in two different roles |
| **Stack** | Python · PyTorch · pydicom · trimesh · Streamlit → PyQt6 desktop app · ISO 9126 · MS Project |
| **Highlights** | DICOM → HU → 3D mesh preprocessing (mine). PM semester: named on 143 of 166 deliverable pages. QA semester: lead author of 37 pages of ISO 9126-based quality, risk and unit-test documents. Nodule detection accuracy 73.1% → 93% (as presented by the team). Grand prize, DYC project competition |
| **Review** | Difficulties I hit as PM went into the next semester's QA risk register, and the team adopted them as real countermeasures. Tracing figures back to the originals, I also corrected a team slide that cited the previous semester's F1 of 0.78 as "78% accuracy". |
| **Code** | **[AILungandLiver](https://github.com/MoriochoRadio/AILungandLiver)** (2025-2) · [LungCT3DNoduleAI](https://github.com/MoriochoRadio/LungCT3DNoduleAI) (2025-1) |

### 3. Government R&D — dataset design for an AI food vision inspector (student researcher)

| | |
|---|---|
| **Project** | Ministry of SMEs and Startups R&D program, "Affordable AI food inspection system for small food manufacturers" · lead company Dongwoo Tech |
| **Period · role** | May–Dec 2025 (8 months) · Konyang University research team, student researcher · **data workstream** |
| **Highlights** | Four classes (normal, broken, over-baked, foreign matter) defined on Codex, UNICEF and MFDS standards, with numeric judgment criteria. 4,066 single-item + 200 multi-item images = 4,266. Three-stage Roboflow labeling and versioning, exported to YOLO, COCO and TFRecord |
| **Review** | A model can be swapped; a wrong label means rebuilding the dataset. When four baselines scored 1.00 accuracy, I read it as a possible artifact of controlled capture and random splits and withheld any generalization claim. |
| **Paper · record** | IEIE 2025 Fall Conference, first author (GEP-0093) · **[food-vision-dataset-design](https://github.com/MoriochoRadio/food-vision-dataset-design)** — the dataset and internal deliverables belong to the company and are not public |

---

## Backend training — full-stack developer bootcamp (since Jun 2026)

HTML · CSS · JavaScript · React · Next.js → Java · JSP/Servlet · MVC · Spring Boot · MyBatis · MariaDB → AI Agent (Python · FastAPI · LangChain · RAG)

| Repository | What it is |
|---|---|
| [web-study-notes](https://github.com/MoriochoRadio/web-study-notes) · [dashboard](https://moriochoradio.github.io/web-study-notes/) | Class code, review cards and verified coding-test solutions, organized by date |
| [java-texas-holdem](https://github.com/MoriochoRadio/java-texas-holdem) | Two-player Texas Hold'em built with Java classes, collections and interfaces; best-5-of-7 hand evaluation, AI usage log, code review notes |
| [nextjs-stock-dashboard](https://github.com/MoriochoRadio/nextjs-stock-dashboard) | Next.js 16 real-time stock dashboard; before/after notes on 6 bugs I found and fixed |

---

## Papers (first author, 2)

- **KKITS 2026 conference** — *Practical Domain Adaptation for Computer-Aided Sperm Analysis: Quality-Aware Video Normalization and Augmentation-Based Morphology Classification* (advisor: Prof. Heo Yongdo)
  A morphology classifier trained on a benchmark collapsed to a 0.5% normal rate on real microscope video; spec-only normalization (99.3% detection retained) and training-time degradation augmentation (0.5% → 16.3%, meeting WHO ≥4%) fixed it at zero inference cost.
- **IEIE 2025 Fall Conference** — Data collection design and implementation for an AI food vision inspector: a hardtack case study (GEP-0093)

## Awards

Grand prize, 2025 DYC project competition (L-POT) · Gold, 2025 Chungcheong AI × Design Thinking Camp · Excellence award at the design-course showcase three times (2024, 2025, 2026)

---

## Other projects

<details>
<summary><b>2024 school team projects · competitions</b></summary>

| When | Project | What | Role · result |
|---|---|---|---|
| 2024-1 | [MedQueue](https://github.com/MoriochoRadio/MedQueue) | Real-time hospital waiting-status app (C# · Xamarin · Firebase) | ENG1 — requirements spec 7 pp. solo + design docs 33 pp. co-authored |
| 2024-2 | [SchoolbusRFID](https://github.com/MoriochoRadio/SchoolbusRFID) | Location-based child drop-off tagging app (Android · RFID · Firebase) | ENG — Android logic, three-role branching |
| 2024-2 | [ElderCaringApp](https://github.com/MoriochoRadio/ElderCaringApp) | Health monitoring for seniors living alone (Android · ESP32 · Firebase) | ENG — load-cell circuit and firmware, statistics screens |
| 2026-06 | [multimodal-bias-vqa](https://github.com/MoriochoRadio/multimodal-bias-vqa) | Multimodal AI bias challenge — VQA that answers "unknown" when evidence is insufficient | Public balanced accuracy 0.883 |
| 2026-07 | [jump-ai-clinical-agent](https://github.com/MoriochoRadio/jump-ai-clinical-agent) | Pre-review agent for clinical-trial protocol drafts — 4th JUMP AI competition | Proposal and CLI prototype submitted |

</details>

<details>
<summary><b>Personal projects — daily auto-updating sites and web apps</b></summary>

Collect → summarize with an LLM → deploy a static site, run daily on GitHub Actions and kept alive by diagnosing and fixing failures.

| Repository | What it is |
|---|---|
| [stock-briefing](https://github.com/MoriochoRadio/stock-briefing) · [site](https://moriochoradio.github.io/stock-briefing/) | Daily US and Korean market briefing |
| [ai-news-curation](https://github.com/MoriochoRadio/ai-news-curation) · [site](https://moriochoradio.github.io/ai-news-curation/) | Daily curation of AI news, papers and open source |
| [ai-daily-trends](https://github.com/MoriochoRadio/ai-daily-trends) · [site](https://moriochoradio.github.io/ai-daily-trends/) | Daily AI trends from GitHub Trending, Hacker News and Reddit |
| [tarkov-korean-changes](https://github.com/MoriochoRadio/tarkov-korean-changes) · [site](https://moriochoradio.github.io/tarkov-korean-changes/) | Daily collection and Korean interpretation of silent game-data changes |
| [sauna-travel-planner](https://github.com/MoriochoRadio/sauna-travel-planner) · [site](https://sauna-travel-planner.vercel.app) | Day-by-day travel planner built around saunas (Kakao place search) |
| [weather-fit](https://github.com/MoriochoRadio/weather-fit) · [site](https://moriochoradio.github.io/weather-fit/) | Weather-based outfit PWA with no server or API key, 79 tests |
| [fit-atlas](https://github.com/MoriochoRadio/fit-atlas) · [site](https://moriochoradio.github.io/fit-atlas/) | Local-first workout app with 990 exercises, routines and logs |

Also [tarkov-companion](https://github.com/MoriochoRadio/tarkov-companion) · [sauna-science-hub](https://github.com/MoriochoRadio/sauna-science-hub) · [fundamental-regime-report](https://github.com/MoriochoRadio/fundamental-regime-report) · [evolution-garden](https://github.com/MoriochoRadio/evolution-garden) · [mindlings](https://github.com/MoriochoRadio/mindlings)

</details>

<details>
<summary><b>Learning archive</b></summary>

Course and self-study work kept as it was:
[study-java](https://github.com/MoriochoRadio/study-java) ·
[study-algorithms](https://github.com/MoriochoRadio/study-algorithms) ·
[study-windows-programming](https://github.com/MoriochoRadio/study-windows-programming) ·
[Iot-Github](https://github.com/MoriochoRadio/Iot-Github) ·
[study-web-basics](https://github.com/MoriochoRadio/study-web-basics) · [study-web-funsun](https://github.com/MoriochoRadio/study-web-funsun)

</details>

---

<sub>Each repository README lists the team, the roles, <b>what I did and did not do, and the attempts that failed</b>. Figures are traced to slides, papers or code records; where measurement conditions were not preserved, I say so.</sub>
