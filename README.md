# 김태경 — 백엔드 개발자 (Java · Spring Boot)

🇰🇷 한국어 · 🇬🇧 [English](README.en.md)

**의료IT · 헬스케어 솔루션을 지향하는 백엔드 개발자**를 준비하고 있습니다.<br>
건양대학교 의료IT공학과 2027년 2월 졸업 예정 (4.30 / 4.5) · 취업아카데미 풀스택 개발자 과정 수강 중 (2026.06~)

📧 **taeral04@gmail.com**

사용자가 보지 못하는 곳에서 데이터가 생성·처리·전달되는 경로를 책임지는 일을 하고 싶습니다.
설계 교과 팀 프로젝트 6건(2024~2026, 5개 학기)에서 ENG → PM → QA를 두루 맡으며 요구사항을 구조로 옮기고 끝까지 검증하는 법을 익혔고,
지금은 Java · Spring Boot와 관계형 데이터베이스로 그 경로를 더 단단하게 만드는 역량을 쌓고 있습니다.

---

## 기술 스택

| 분야 | 기술 | 어디에 썼나 |
|---|---|---|
| **백엔드** | ![Java 21](https://img.shields.io/badge/Java%2021-ED8B00?logo=openjdk&logoColor=white) ![Spring Boot 4.1](https://img.shields.io/badge/Spring%20Boot%204.1-6DB33F?logo=springboot&logoColor=white) ![MyBatis](https://img.shields.io/badge/MyBatis-B22222) ![JSP/Servlet](https://img.shields.io/badge/JSP%20%2F%20Servlet-007396) ![MariaDB](https://img.shields.io/badge/MariaDB-003545?logo=mariadb&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white) ![SQLite](https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=white) | 취업아카데미 — Spring Boot 게시판 개선 과제(첨부 관리 · 작성자 권한 · 설정 분리 · 트랜잭션 롤백)를 로컬 MariaDB에서 실행해 확인, Java 텍사스 홀덤 |
| **프론트엔드** | ![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) ![CSS](https://img.shields.io/badge/CSS-1572B6?logo=css&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white) ![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black) ![Next.js](https://img.shields.io/badge/Next.js-000000?logo=nextdotjs&logoColor=white) | Next.js 16 실시간 주식 대시보드(Finnhub REST/WebSocket · Zustand · Recharts), 서버 없는 정적 웹앱 |
| **Python · AI** | ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white) ![Flask](https://img.shields.io/badge/Flask-000000?logo=flask&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white) ![pydicom](https://img.shields.io/badge/pydicom-4B8BBE) | SEED 4계층 파이프라인 설계(ENG2와 공동)·통합과 Flask 리포트, DICOM → HU → 3D mesh 전처리, 도메인 적응 실험 → 제1저자 논문 |
| **협업 · 인프라** | ![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white) ![Firebase](https://img.shields.io/badge/Firebase-FFCA28?logo=firebase&logoColor=black) ![Linux](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black) ![Android](https://img.shields.io/badge/Android-3DDC84?logo=android&logoColor=white) ![C# · Xamarin](https://img.shields.io/badge/C%23%20%C2%B7%20Xamarin-512BD4?logo=dotnet&logoColor=white) | GitHub Actions로 매일 자동 수집·배포하는 사이트 운영(결손 진단 · 자가복구 전환), Firebase 실시간 동기화 앱 3건, 요구사항 · 설계 · 품질 · 위험 산출물 104쪽 1차 저자(공저 포함) |

<sub>구현 전반에 AI 코딩 도구를 활용했습니다. 기술을 고르고 구조를 정하고 결과를 검증하는 판단은 제 몫이었고, AI가 만든 코드는 실행·테스트로 확인한 뒤에만 반영했습니다.</sub>

---

## 대표 프로젝트

### 1. SEED — AI 정자 자동 탐지 및 형태·운동성 통합 분석 시스템

| | |
|---|---|
| **기획 의도** | 수동 판독은 검사자마다 결과가 다르고, CASA 장비는 비싸며 형태 판독은 여전히 사람이 합니다. 일반 현미경 영상만으로 같은 정자 기준의 형태·운동성 통합 판정을 받을 수 있게 하자는 것이 출발점이었습니다. |
| **기간 · 인원 · 역할** | 2026.03 ~ 06 (15주, 융합캡스톤디자인) · 5인 · **ENG1** — 시스템 구조 설계(ENG2와 공동) · 계층 간 인터페이스 정의 · 4명이 병렬로 개발한 모듈 8개 통합 · 형태 분석 모델 구현 |
| **기술 스택** | Python · PyTorch · YOLO11 · ByteTrack · EfficientNet-B3 · scikit-learn · Flask |
| **주요 특징** | 입력 정규화 → 탐지·추적 → 운동성 회귀·형태 분류 → WHO 판정의 4계층 파이프라인. 착수 전 고정한 목표 3항목 전부 달성 — 운동성 MAE 6.90%p(선행 연구 7.31%p보다 낮음) · 탐지 mAP@50 0.677 · 형태 AUC 0.725 |
| **리뷰** | 벤치마크 1위 모델이 실제 영상에서는 정상형태율 0.5%를 내는 것을 보고, 점수가 아니라 현장에서 쓸 수 있는지로 모델을 골라야 한다는 것을 배웠습니다. 인터페이스를 문서로 먼저 고정해야 병렬 개발이 된다는 것도 이때 체득했습니다. |
| **코드** | **[seed-project](https://github.com/MoriochoRadio/seed-project)** · 개인 베이스라인 [sperm-ai](https://github.com/MoriochoRadio/sperm-ai) |

### 2. L-POT — 간·폐 CT 이미지의 AI 기반 진단 보조 및 3D 시각화 시스템

| | |
|---|---|
| **기획 의도** | 시중의 CT 판독 보조 AI는 전부 의료진용입니다. 환자가 자기 CT를 3D로 보고 이해하도록 돕는 참고용 도구를 목표로 했습니다. |
| **기간 · 인원 · 역할** | 2025.03 ~ 06 · 6인 · **PM** + 데이터 전처리 → 2025.08 ~ 12 · 5인 · **QA**. 같은 시스템을 두 학기 동안 서로 다른 역할로 맡았습니다 |
| **기술 스택** | Python · PyTorch · pydicom · trimesh · Streamlit → PyQt6 데스크탑 앱 · ISO 9126 · MS Project |
| **주요 특징** | DICOM → HU 변환 → 3D mesh 전처리(내 담당). PM 학기 산출물 166쪽 중 143쪽에 이름 기재. QA 학기에 ISO 9126 기반 품질·위험·단위시험 산출물 37쪽 1차 저자. 결절 탐지 정확도 73.1% → 93%(팀 발표 기준). DYC 경진대회 대상 |
| **리뷰** | PM 자리에서 겪은 어려움을 다음 학기 QA 위험 평가표로 옮겼더니 팀이 실제 대비 사항으로 받아들였습니다. 수치를 원본까지 역추적해, 팀 자료가 직전 학기 F1 0.78을 "정확도 78%"로 잘못 인용한 것도 바로잡았습니다. |
| **코드** | **[AILungandLiver](https://github.com/MoriochoRadio/AILungandLiver)** (2025-2) · [LungCT3DNoduleAI](https://github.com/MoriochoRadio/LungCT3DNoduleAI) (2025-1) |

### 3. 정부 R&D — AI 식품 비전검사기 데이터셋 설계 (학생연구원)

| | |
|---|---|
| **과제** | 중소벤처기업부 중소기업 기술개발(R&D) 지원사업 「소규모 식품 제조업체를 위한 보급형 AI 복합식품검사 시스템 개발」 · 주관 (주)동우텍 |
| **기간 · 역할** | 2025.05 ~ 12 (8개월) · 건양대학교 연구팀 학생연구원 · **데이터 파트** |
| **주요 특징** | 불량 4클래스(정상 · 부서짐 · 과도한 익음 · 이물 혼입)를 Codex · UNICEF · MFDS 규범 근거로 정의하고 수치 판정 기준까지 명시. 단일 개체 4,066장 + 집합 200장 = 4,266장 구축. Roboflow 3단계 라벨링 · 버전관리, YOLO · COCO · TFRecord 내보내기 |
| **리뷰** | 모델은 바꾸면 그만이지만 잘못된 라벨은 데이터셋 전체를 다시 만들어야 합니다. 베이스라인 4종이 정확도 1.00을 냈을 때, 통제된 촬영 환경과 무작위 분할로 평가가 쉬워졌을 가능성으로 읽고 일반화 주장을 유보했습니다. |
| **논문 · 기록** | 대한전자공학회 2025 추계학술대회 제1저자 (GEP-0093) · **[food-vision-dataset-design](https://github.com/MoriochoRadio/food-vision-dataset-design)** — 과제 데이터셋과 내부 산출물은 기업 소유라 공개하지 않습니다 |

---

## 백엔드 학습 — 취업아카데미 풀스택 개발자 과정 (2026.06~)

HTML · CSS · JavaScript · React · Next.js → Java · JSP/Servlet · MVC · Spring Boot · MyBatis · MariaDB → AI Agent(Python · FastAPI · LangChain · RAG)

| 저장소 | 내용 |
|---|---|
| [Spring Boot 게시판](https://github.com/MoriochoRadio/web-study-notes/tree/main/Back_end/web_edu_project/10_login_board_springboot) · [검증 기록](https://github.com/MoriochoRadio/web-study-notes/blob/main/Back_end/sync-validation-2026-10-12.md) | Java 21 · Spring Boot 4.1 · Spring Security · MyBatis · MariaDB · Thymeleaf. 수업 게시판에 개선 과제 5건(작성자 권한 · 첨부 수정 · 설정 분리 · 생성자 주입 · 로깅)을 AI 코딩 도구와 함께 적용하고, 임시 회원 2명으로 타인 글 수정·삭제 차단과 트랜잭션 롤백을 로컬 DB에서 실행해 확인 |
| [web-study-notes](https://github.com/MoriochoRadio/web-study-notes) · [대시보드](https://moriochoradio.github.io/web-study-notes/) | 수업 코드 · 복습 카드 · 코딩테스트 풀이와 검증을 날짜별로 정리한 학습 기록 |
| [java-texas-holdem](https://github.com/MoriochoRadio/java-texas-holdem) | Java 클래스 · 컬렉션 · 인터페이스로 구현한 2인용 텍사스 홀덤. 7장 중 최강 5장 판정 로직, AI 활용 일지, 코드 리뷰 기록 |
| [nextjs-stock-dashboard](https://github.com/MoriochoRadio/nextjs-stock-dashboard) | Next.js 16 실시간 주식 대시보드. 직접 찾아 고친 버그 6건의 Before/After 기록 |

---

## 논문 (제1저자 2편)

- **KKITS 2026 학술대회 발표** — *Practical Domain Adaptation for Computer-Aided Sperm Analysis: Quality-Aware Video Normalization and Augmentation-Based Morphology Classification* (지도 허용도 교수)
  벤치마크에서 학습한 형태 분류 모델이 실제 현미경 영상에서 정상형태율 0.5%로 무너지는 문제를, 추론 비용 없이 규격 통일(검출 99.3% 유지)과 학습 시 열화 모사 증강(0.5% → 16.3%, WHO 기준 4% 이상)으로 해결했습니다.
- **대한전자공학회 2025 추계학술대회** — AI 식품 비전검사를 위한 데이터 수집 설계와 구현: 건빵 사례 연구 (논문번호 GEP-0093)

## 수상

2025 DYC 프로젝트 경진대회 **대상**(L-POT) · 2025 충청지역 AI × Design Thinking 캠프 **금상** · 설계교과목 성과전시회 우수상 3회(2024 · 2025 · 2026)

---

## 기타 프로젝트

<details>
<summary><b>학교 팀 프로젝트 2024 · 공모전</b></summary>

| 시기 | 프로젝트 | 내용 | 역할 · 결과 |
|---|---|---|---|
| 2024-1 | [MedQueue](https://github.com/MoriochoRadio/MedQueue) | 병원 실시간 대기정보 앱 (C# · Xamarin · Firebase) | ENG1 — 요구사항분석서 7쪽 단독 + 설계서 33쪽 공저 |
| 2024-2 | [SchoolbusRFID](https://github.com/MoriochoRadio/SchoolbusRFID) | 위치 기반 어린이 하차 태그 앱 (Android · RFID · Firebase) | ENG — Android 로직 · 3역할 분기 |
| 2024-2 | [ElderCaringApp](https://github.com/MoriochoRadio/ElderCaringApp) | 독거노인 건강 모니터링 (Android · ESP32 · Firebase) | ENG — 로드셀 회로·펌웨어 · 통계 화면 |
| 2026-06 | [multimodal-bias-vqa](https://github.com/MoriochoRadio/multimodal-bias-vqa) | 멀티모달 AI Bias 챌린지 — 근거가 부족하면 "모름"을 고르는 VQA | Public Balanced Accuracy 0.883 |
| 2026-07 | [jump-ai-clinical-agent](https://github.com/MoriochoRadio/jump-ai-clinical-agent) | 임상시험 프로토콜 사전 점검 에이전트 — 제4회 JUMP AI 경진대회 | 제안서 · CLI 프로토타입 제출 |

</details>

<details>
<summary><b>개인 프로젝트 — 매일 자동 갱신되는 사이트 · 웹앱</b></summary>

데이터 수집 → LLM 요약 → 정적 사이트 배포를 GitHub Actions 위에서 매일 돌리고, 고장이 나면 원인을 진단해 복구하며 운영해 온 것들입니다.

| 저장소 | 내용 |
|---|---|
| [stock-briefing](https://github.com/MoriochoRadio/stock-briefing) · [사이트](https://moriochoradio.github.io/stock-briefing/) | 매일 아침 미국·한국 증시 브리핑 자동 생성 |
| [ai-news-curation](https://github.com/MoriochoRadio/ai-news-curation) · [사이트](https://moriochoradio.github.io/ai-news-curation/) | AI 뉴스 · 논문 · 오픈소스 매일 자동 큐레이션 |
| [ai-daily-trends](https://github.com/MoriochoRadio/ai-daily-trends) · [사이트](https://moriochoradio.github.io/ai-daily-trends/) | GitHub Trending · Hacker News · Reddit의 AI 트렌드 매일 수집·요약 |
| [tarkov-korean-changes](https://github.com/MoriochoRadio/tarkov-korean-changes) · [사이트](https://moriochoradio.github.io/tarkov-korean-changes/) | 게임 데이터의 사일런트 변경을 매일 수집해 한국어로 해석 |
| [sauna-travel-planner](https://github.com/MoriochoRadio/sauna-travel-planner) · [사이트](https://sauna-travel-planner.vercel.app) | 사우나를 축으로 일자별 여행 코스를 짜 주는 웹앱 (카카오 장소 검색) |
| [weather-fit](https://github.com/MoriochoRadio/weather-fit) · [사이트](https://moriochoradio.github.io/weather-fit/) | 날씨 기반 코디 추천 PWA — 서버 · API 키 없이 동작, 테스트 79개 |
| [fit-atlas](https://github.com/MoriochoRadio/fit-atlas) · [사이트](https://moriochoradio.github.io/fit-atlas/) | 운동 990종 · 루틴 · 기록을 담은 로컬 우선 웹앱 |

그 밖에 [tarkov-companion](https://github.com/MoriochoRadio/tarkov-companion) · [sauna-science-hub](https://github.com/MoriochoRadio/sauna-science-hub) · [fundamental-regime-report](https://github.com/MoriochoRadio/fundamental-regime-report) · [evolution-garden](https://github.com/MoriochoRadio/evolution-garden) · [mindlings](https://github.com/MoriochoRadio/mindlings)

</details>

<details>
<summary><b>학습 아카이브</b></summary>

수업 · 독학 과정을 그대로 보존한 저장소입니다.
[study-java](https://github.com/MoriochoRadio/study-java) (Java 기초 → GUI) ·
[study-algorithms](https://github.com/MoriochoRadio/study-algorithms) (알고리즘 C++/C#) ·
[study-windows-programming](https://github.com/MoriochoRadio/study-windows-programming) (WinForms/WPF) ·
[Iot-Github](https://github.com/MoriochoRadio/Iot-Github) (Zynq 보드 IoT 실습) ·
[study-web-basics](https://github.com/MoriochoRadio/study-web-basics) · [study-web-funsun](https://github.com/MoriochoRadio/study-web-funsun) (2020, 첫 웹)

</details>

---

<sub>각 저장소 README에는 팀 구성 · 역할과 함께 <b>제가 직접 한 부분과 하지 않은 부분, 실패한 시도</b>를 적어 두었습니다. 수치는 발표자료 · 논문 · 코드 기록에서 출처를 확인한 값이며, 측정 조건이 남아 있지 않은 것은 그렇게 밝혀 두었습니다.</sub>
