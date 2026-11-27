# Kim Taekyoung (김태경) — Software Developer

🇰🇷 [한국어](README.md) · 🇬🇧 English

Preparing to work as a **software developer for hospital information systems and medical IT**, with Java · Spring Boot backend as my core.<br>
Dept. of Medical IT Engineering, Konyang University — expected graduation Feb 2027 (GPA 4.30 / 4.5) · AI & Java (Spring) Full-Stack Course, 7th cohort (Jun–Dec 2026, 952 hours)

📧 **kim.taekyoung.dev@gmail.com**

Across six team design projects (2024–2026, five semesters) I worked as developer, PM and QA and went through the whole team process myself — from requirements to deliverables, schedules and testing.
Now I am building the skills to make service backends with Java, Spring Boot and relational databases.

---

## Tech stack

| Area | Tools | Where I used them |
|---|---|---|
| **Backend** | ![Java](https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?logo=springboot&logoColor=white) ![MyBatis](https://img.shields.io/badge/MyBatis-B22222) ![MariaDB](https://img.shields.io/badge/MariaDB-003545?logo=mariadb&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white) | NewsTalk backend (screen APIs, JWT login, DB design, Flyway), one-command team DB setup with Docker Compose, Spring Boot board assignment in class |
| **Frontend** | ![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) ![CSS](https://img.shields.io/badge/CSS-1572B6?logo=css&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black) ![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black) | Class assignments, helped improve NewsTalk screens |
| **Python · AI** | ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white) ![Flask](https://img.shields.io/badge/Flask-000000?logo=flask&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white) | SEED first version (sperm detection to Flask web server) and morphology analysis, helped with L-POT CT preprocessing |
| **Mobile · tools** | ![Android](https://img.shields.io/badge/Android-3DDC84?logo=android&logoColor=white) ![C#](https://img.shields.io/badge/C%23-512BD4?logo=dotnet&logoColor=white) ![Firebase](https://img.shields.io/badge/Firebase-FFCA28?logo=firebase&logoColor=black) ![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-181717?logo=github&logoColor=white) | MedQueue (C# · Xamarin), ElderCaringApp · SchoolbusRFID (Android · Firebase), managed the NewsTalk team repository |

<sub>I use AI coding tools throughout. Choosing the technology, deciding the structure and verifying the result are my job; AI-written code goes in only after I have run and tested it.</sub>

---

## Featured projects

### 1. NewsTalk — stock analysis through news and disclosures

| | |
|---|---|
| **Why** | There are too many articles, and a stock tag alone does not tell you why an article is about that stock |
| **Period · team · role** | Oct 28 – Nov 18, 2026 (3 weeks) · 4 people · team project of the AI & Java (Spring) Full-Stack Course · **backend lead**, GitHub management, DB design, screen APIs — also helped with AI collection and screens |
| **Stack** | Java · Spring Boot · MyBatis · MariaDB · Spring Security (JWT) · Docker · Flyway |
| **Highlights** | Screen APIs (articles, stocks, members, board) · login (JWT). With Docker Compose and Flyway, all four members get the same DB with one command (MariaDB 11.8.9 pinned to the patch version, port 3308 to avoid the class DB, table changes as numbered files V1–V18) |
| **Review** | After the first review, our industry mentor pointed out cost and decision criteria, and I learned that every choice needs evidence and a cost check. From then on I recorded the reason and alternatives for each decision, and put the limits and next steps (moving the collector to the cloud, more human review) in the final report and presentation. |
| **Code** | **[newstalk](https://github.com/MoriochoRadio/newstalk)** |

### 2. SEED — AI sperm detection with integrated morphology and motility analysis

| | |
|---|---|
| **Why** | Automate sperm reading, which varies by examiner and takes a long time, from a single video |
| **Period · team · role** | Mar–Jun 2026 (15 weeks) · 5 people · capstone course · **built the first version from sperm detection to the web server**, which the team then extended · in the team: morphology analysis and integration (shared) |
| **Stack** | Python · PyTorch · YOLO11 · ByteTrack · EfficientNet-B3 · Flask |
| **Highlights** | Motility prediction error 6.90%p — lower than the prior paper on the same public data (7.31%p) · normal rate on real footage 0.5% → 16.3% (into the WHO ≥4% range) · morphology batched, 53.6 s → 1.3 s (same results) · KKITS 2026 paper (first author) · excellence award, design-course showcase (2026-1) |
| **Review** | Sharing a first version early let teammates go straight to improving their parts, and I learned that showing a working skeleton first makes a team faster. The failed attempts and future work (multi-site clinical validation) went into my first-author paper. |
| **Code** | **[seed-project](https://github.com/MoriochoRadio/seed-project)** · my earlier solo research [sperm-ai](https://github.com/MoriochoRadio/sperm-ai) |

### 3. L-POT — AI diagnostic aid and 3D visualization for liver and lung CT

| | |
|---|---|
| **Why** | Let patients see and understand their own CT in 3D |
| **Period · team · role** | Mar–Nov 2025 (two semesters, 28 weeks) · 6 people, then 5 · major course · **semester 1: PM** + CT data collection, helped with preprocessing → **semester 2: QA** (quality, risk, testing) |
| **Stack** | Python · PyTorch · pydicom · trimesh · PyQt6 · MS Project |
| **Highlights** | Semester 1: schedule, assignments and deadlines in MS Project; helped turn CT (DICOM) into 3D models · Semester 2: wrote the quality and risk management plans, tested 12 screen functions, checked the model's reported figures · grand prize, campus project competition (Dec 2025) · excellence award, design-course showcase (2025-1, my PM semester) |
| **Review** | As PM with little time, I put AI accuracy and processing logic first and pushed design back — learning to decide first what to postpone; as QA I learned to test through the user's eyes. The lack of "no nodule" data, reported in the semester-1 presentation, became the team's goal for semester 2. |
| **Code** | **[AILungandLiver](https://github.com/MoriochoRadio/AILungandLiver)** (2025-2) · [LungCT3DNoduleAI](https://github.com/MoriochoRadio/LungCT3DNoduleAI) (2025-1) |

---

## Other projects

| When | Project | What | My part |
|---|---|---|---|
| May–Dec 2025 | **AI food inspection dataset** — government R&D student researcher · [food-vision-dataset-design](https://github.com/MoriochoRadio/food-vision-dataset-design) | Data workstream (Konyang University team) of the Ministry of SMEs and Startups R&D project "Affordable AI food inspection system for small food manufacturers" | Defined 4 judgment classes (1 normal, 3 defect) · labeled 4,266 hardtack images (photographed with a teammate, Roboflow) · IEIE conference paper (first author) |
| Mar–Jun 2024 | **MedQueue** — hospital queue app · [MedQueue](https://github.com/MoriochoRadio/MedQueue) | Check your queue number on your phone instead of waiting at the clinic door (C# · Xamarin.Forms · Firebase) | Xamarin app logic · co-designed the Firebase DB structure · queue data integration · requirements spec · UML diagrams · excellence award (2024-1) |
| Sep–Nov 2024 | **ElderCaringApp** — health monitoring for seniors living alone · [ElderCaringApp](https://github.com/MoriochoRadio/ElderCaringApp) | Lets family far away follow a parent's day in an app (Java (Android) · ESP32 · Firebase) | Load-cell circuit and firmware · three Android statistics screens · midterm and final presentations |
| Aug–Sep 2024 | **SchoolbusRFID** — location-based child drop-off tagging app · [SchoolbusRFID](https://github.com/MoriochoRadio/SchoolbusRFID) | Checks school-bus boarding with RFID tags (Java (Android) · ESP8266 · Firebase) · rebuilt from a senior team's project | Android app logic · real-time boarding counts with Firebase |

---

## Papers · awards · certifications

- **Papers (first author, 2)**
  - KKITS 2026 conference — *Practical Domain Adaptation for Computer-Aided Sperm Analysis: Quality-Aware Video Normalization and Augmentation-Based Morphology Classification* (SEED)
  - IEIE 2025 Fall Conference — Data collection design and implementation for an AI food vision inspector: a hardtack case study
- **Awards** — Grand prize, campus (DYC) project competition (L-POT, Dec 2025) · Gold, AI × Design Thinking Camp (Jun 2025) · excellence award at the design-course showcase three times (MedQueue, L-POT, SEED) · encouragement award, hospital clinical data AI basics course (Jul 2025)
- **Certifications** — Engineer Information Processing · TOEIC 905 · NAVER Cloud Platform Certified Associate · TOPCIT level 3 · Big Data Practical Skills level 1

---

## Training · learning records

**AI & Java (Spring) Full-Stack Course, 7th cohort** (Jun–Dec 2026, 6 months / 952 hours) — Java · Spring Boot · MyBatis · MariaDB · React · Next.js · AI Agent

| Repository | What it is |
|---|---|
| [Spring Boot board](https://github.com/MoriochoRadio/web-study-notes/tree/main/Back_end/web_edu_project/10_login_board_springboot) · [verification notes](https://github.com/MoriochoRadio/web-study-notes/blob/main/Back_end/sync-validation-2026-10-12.md) | Applied a five-item improvement assignment (author permissions, attachment edits, config separation, constructor injection, logging) to the class board with an AI coding assistant, and verified with two test accounts on a local DB that others' posts cannot be edited or deleted and that transactions roll back |
| [web-study-notes](https://github.com/MoriochoRadio/web-study-notes) · [dashboard](https://moriochoradio.github.io/web-study-notes/) | Class code, review cards and verified coding-test solutions, organized by date |
| [java-texas-holdem](https://github.com/MoriochoRadio/java-texas-holdem) | Two-player Texas Hold'em with Java classes, collections and interfaces; best-5-of-7 hand evaluation, AI usage log, code review notes |

Other training: NAVER Cloud Academy, 3rd cohort (Dec 2025, 5 days / 40 h) · GitHub IoT programming camp (Nov 2025, 4 days) · hospital clinical data AI basics (Jul 2025, 5 days) · AI × Design Thinking Camp (Jun 2025, 4 days / 32 h)

<details>
<summary><b>Learning archive</b></summary>

Course and self-study work kept as it was:
[study-java](https://github.com/MoriochoRadio/study-java) ·
[study-algorithms](https://github.com/MoriochoRadio/study-algorithms) ·
[study-windows-programming](https://github.com/MoriochoRadio/study-windows-programming) ·
[Iot-Github](https://github.com/MoriochoRadio/Iot-Github) ·
[study-web-basics](https://github.com/MoriochoRadio/study-web-basics) · [study-web-funsun](https://github.com/MoriochoRadio/study-web-funsun)

</details>

<details>
<summary><b>Personal projects · competitions</b></summary>

Personal projects built and run with AI coding tools, and competition submissions.

| Repository | What it is |
|---|---|
| [nextjs-stock-dashboard](https://github.com/MoriochoRadio/nextjs-stock-dashboard) | Next.js real-time stock dashboard; before/after notes on 6 bugs I found and fixed |
| [stock-briefing](https://github.com/MoriochoRadio/stock-briefing) · [site](https://moriochoradio.github.io/stock-briefing/) | Daily US and Korean market briefing |
| [ai-news-curation](https://github.com/MoriochoRadio/ai-news-curation) · [site](https://moriochoradio.github.io/ai-news-curation/) | Daily curation of AI news, papers and open source |
| [ai-daily-trends](https://github.com/MoriochoRadio/ai-daily-trends) · [site](https://moriochoradio.github.io/ai-daily-trends/) | Daily AI trends from GitHub Trending, Hacker News and Reddit |
| [weather-fit](https://github.com/MoriochoRadio/weather-fit) · [site](https://moriochoradio.github.io/weather-fit/) | Weather-based outfit PWA with no server or API key |
| [fit-atlas](https://github.com/MoriochoRadio/fit-atlas) · [site](https://moriochoradio.github.io/fit-atlas/) | Local-first workout app with 990 exercises, routines and logs |
| [multimodal-bias-vqa](https://github.com/MoriochoRadio/multimodal-bias-vqa) | Multimodal AI bias challenge (Jun 2026) — VQA that answers "unknown" when evidence is insufficient |
| [jump-ai-clinical-agent](https://github.com/MoriochoRadio/jump-ai-clinical-agent) | 4th JUMP AI competition (Jul 2026) — proposal and CLI prototype of a clinical-trial protocol pre-check agent |

Also [tarkov-korean-changes](https://github.com/MoriochoRadio/tarkov-korean-changes) · [tarkov-companion](https://github.com/MoriochoRadio/tarkov-companion) · [sauna-travel-planner](https://github.com/MoriochoRadio/sauna-travel-planner) · [sauna-science-hub](https://github.com/MoriochoRadio/sauna-science-hub) · [fundamental-regime-report](https://github.com/MoriochoRadio/fundamental-regime-report) · [evolution-garden](https://github.com/MoriochoRadio/evolution-garden) · [mindlings](https://github.com/MoriochoRadio/mindlings)

</details>

---

<sub>Each repository README lists the team, the roles, <b>what I did and did not do, and the attempts that failed</b>. Figures are traced to slides, papers or code records; where measurement conditions were not preserved, I say so.</sub>
