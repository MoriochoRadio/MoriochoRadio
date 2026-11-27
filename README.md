# 김태경 — 소프트웨어 개발자

🇰🇷 한국어 · 🇬🇧 [English](README.en.md)

**병원전산 · 의료IT 소프트웨어를 지향하는 개발자**를 준비하고 있습니다. Java · Spring Boot 백엔드가 중심입니다.<br>
건양대학교 의료IT공학과 2027년 2월 졸업 예정 (학점 4.30 / 4.5) · AI와 자바(Spring) 풀스택 과정 7기 수강 중 (2026.06 ~ 12, 952시간)

📧 **kim.taekyoung.dev@gmail.com**

설계 교과 팀 프로젝트 6건(2024 ~ 2026, 5개 학기)에서 개발 · PM · QA를 맡으며 요구사항부터 산출물 · 일정 · 시험까지 팀 개발 과정을 직접 겪었고,
지금은 Java · Spring Boot와 관계형 데이터베이스로 서비스의 백엔드를 만드는 역량을 쌓고 있습니다.

---

## 기술 스택

| 분야 | 기술 | 어디에 썼나 |
|---|---|---|
| **백엔드** | ![Java](https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?logo=springboot&logoColor=white) ![MyBatis](https://img.shields.io/badge/MyBatis-B22222) ![MariaDB](https://img.shields.io/badge/MariaDB-003545?logo=mariadb&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white) | 뉴스톡 백엔드(화면용 API · JWT 로그인 · DB 설계 · Flyway), Docker Compose로 팀 DB 환경 통일, 수업 Spring Boot 게시판 과제 |
| **프론트엔드** | ![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) ![CSS](https://img.shields.io/badge/CSS-1572B6?logo=css&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black) ![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black) | 수업 과제, 뉴스톡 화면 개선 참여 |
| **Python · AI** | ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white) ![Flask](https://img.shields.io/badge/Flask-000000?logo=flask&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white) | SEED 초기 버전(정자 탐지 ~ Flask 웹 서버) · 형태 분석, L-POT CT 영상 전처리 참여 |
| **모바일 · 도구** | ![Android](https://img.shields.io/badge/Android-3DDC84?logo=android&logoColor=white) ![C#](https://img.shields.io/badge/C%23-512BD4?logo=dotnet&logoColor=white) ![Firebase](https://img.shields.io/badge/Firebase-FFCA28?logo=firebase&logoColor=black) ![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-181717?logo=github&logoColor=white) | MedQueue(C# · Xamarin), ElderCaringApp · SchoolbusRFID(Android · Firebase), 뉴스톡 팀 저장소 관리 |

<sub>구현 전반에 AI 코딩 도구를 활용했습니다. 기술을 고르고 구조를 정하고 결과를 검증하는 판단은 제 몫이었고, AI가 만든 코드는 실행 · 테스트로 확인한 뒤에만 반영했습니다.</sub>

---

## 대표 프로젝트

### 1. 뉴스톡 — 뉴스 · 공시로 보는 종목 분석 서비스

| | |
|---|---|
| **기획 의도** | 기사는 너무 많고, 종목 태그만으로는 왜 그 종목인지 알 수 없다는 불편을 풀자 |
| **기간 · 인원 · 역할** | 2026.10.28 ~ 11.18 (3주) · 4인 · AI와 자바(Spring) 풀스택 과정 팀 프로젝트 · **백엔드 담당** · GitHub 관리 · DB 설계 · 화면용 API — AI 수집 · 화면 개선에도 참여 |
| **기술 스택** | Java · Spring Boot · MyBatis · MariaDB · Spring Security(JWT) · Docker · Flyway |
| **주요 특징** | 화면용 API(기사 · 종목 · 회원 · 게시판) · 로그인(JWT). Docker Compose와 Flyway로 팀원 4명의 DB를 한 줄 실행으로 똑같이 맞춤(MariaDB 11.8.9 패치 버전 고정 · 수업용 DB와 겹치지 않게 포트 3308 · 테이블 변경은 번호 파일 V1 ~ V18) |
| **리뷰** | 1차 피드백에서 실무 멘토님이 비용과 판단 기준을 짚어 주셔서, 모든 선택에 근거와 비용을 따져야 함을 배웠습니다. 그 뒤로 결정마다 이유와 대안을 문서로 남겼고, 한계와 다음 단계(수집기 클라우드 이전 · 사람 검수 확대)도 결과보고서와 발표 자료에 정리했습니다. |
| **코드** | **[newstalk](https://github.com/MoriochoRadio/newstalk)** |

### 2. SEED — AI 기반 정자 자동 탐지 및 형태 · 운동성 통합 분석 시스템

| | |
|---|---|
| **기획 의도** | 검사자마다 결과가 다르고 시간이 오래 걸리는 정자 판독을 영상 하나로 자동화하자 |
| **기간 · 인원 · 역할** | 2026.03 ~ 06 (15주) · 5인 · 전공 수업(융합캡스톤디자인) · **정자 탐지부터 웹 서버까지 초기 버전을 먼저 구현**해 팀이 이를 바탕으로 확장 · 팀에서는 형태 분석과 통합(공동) |
| **기술 스택** | Python · PyTorch · YOLO11 · ByteTrack · EfficientNet-B3 · Flask |
| **주요 특징** | 운동성 예측 오차 6.90%p — 같은 공개 데이터를 쓴 기존 논문(7.31%p)보다 낮음 · 실제 영상의 정상 판정 비율 0.5% → 16.3%(WHO 기준 4% 이상 범위로) · 형태 분석을 묶음 처리로 바꿔 53.6초 → 1.3초(결과 동일) · KKITS 2026 학술대회 논문 발표(제1저자) · 설계교과목 성과전시회 우수상(2026-1) |
| **리뷰** | 초기 버전을 먼저 만들어 공유하니 팀원들이 맡은 부분의 고도화에 바로 들어갈 수 있었고, 동작하는 뼈대를 먼저 보여 주면 팀이 빨라진다는 것을 배웠습니다. 실패한 시도와 향후 과제(다기관 임상 데이터 검증)까지 제1저자 논문에 정리해 발표했습니다. |
| **코드** | **[seed-project](https://github.com/MoriochoRadio/seed-project)** · 개인 초기 연구 [sperm-ai](https://github.com/MoriochoRadio/sperm-ai) |

### 3. L-POT — 간 · 폐 CT 이미지의 AI 기반 진단 보조 및 3D 시각화 시스템

| | |
|---|---|
| **기획 의도** | 환자가 자기 CT를 3D로 직접 보고 이해할 수 있게 하자 |
| **기간 · 인원 · 역할** | 2025.03 ~ 11 (두 학기 · 28주) · 1학기 6인 · 2학기 5인 · 전공 수업(융합설계) · **1학기 PM** + CT 데이터 수집 · 전처리 참여 → **2학기 QA**(품질 · 위험 · 시험) |
| **기술 스택** | Python · PyTorch · pydicom · trimesh · PyQt6 · MS Project |
| **주요 특징** | 1학기: MS Project로 일정 · 담당 · 기한 관리, CT 영상(DICOM) → 3D 모델 전처리 참여 · 2학기: 품질관리 · 위험관리 계획서 작성, 화면 기능 12항목 시험, 모델 성능 수치 확인 · 교내 프로젝트 경진대회 대상(2025.12) · 설계교과목 성과전시회 우수상(2025-1, PM을 맡은 학기) |
| **리뷰** | 1학기 PM으로는 시간이 적어 AI 정확도와 처리 로직을 먼저 챙기고 디자인은 뒤로 넘기며 무엇을 미룰지부터 정하는 법을, 2학기 QA로는 쓰는 사람의 눈으로 시험하는 법을 배웠습니다. 1학기 발표에서 밝힌 '결절 없음' 데이터 부족은 팀이 2학기 목표로 삼아 이어 갔습니다. |
| **코드** | **[AILungandLiver](https://github.com/MoriochoRadio/AILungandLiver)** (2025-2) · [LungCT3DNoduleAI](https://github.com/MoriochoRadio/LungCT3DNoduleAI) (2025-1) |

---

## 기타 프로젝트

| 기간 | 프로젝트 | 내용 | 맡은 일 |
|---|---|---|---|
| 2025.05 ~ 12 | **AI 식품 검사 데이터셋** — 정부 R&D 학생연구원 · [food-vision-dataset-design](https://github.com/MoriochoRadio/food-vision-dataset-design) | 중소벤처기업부 R&D 「소규모 식품 제조업체를 위한 보급형 AI 복합식품검사 시스템 개발」의 데이터 파트(건양대학교 연구팀) | 판정 기준 4종 정의(정상 1 · 불량 3) · 건빵 사진 4,266장 라벨링(촬영은 팀원과 공동, Roboflow) · 대한전자공학회 학술대회 논문(제1저자) |
| 2024.03 ~ 06 | **MedQueue** — 병원 대기 순번 앱 · [MedQueue](https://github.com/MoriochoRadio/MedQueue) | 진료실 앞에서 기다리지 않고 휴대폰으로 내 순번을 실시간 확인 (C# · Xamarin.Forms · Firebase) | Xamarin 앱 로직 · Firebase DB 구조 공동 설계 · 대기열 데이터 연동 · 요구사항 분석서 · UML 다이어그램 · 성과전시회 우수상(2024-1) |
| 2024.09 ~ 11 | **ElderCaringApp** — 독거노인 건강 모니터링 · [ElderCaringApp](https://github.com/MoriochoRadio/ElderCaringApp) | 떨어져 사는 보호자가 부모님의 하루를 앱으로 확인 (Java(Android) · ESP32 · Firebase) | 무게 센서(로드셀) 회로 · 펌웨어 · Android 통계 화면 3개 · 중간 · 최종 발표 |
| 2024.08 ~ 09 | **SchoolbusRFID** — 위치 기반 어린이 하차 태그 앱 · [SchoolbusRFID](https://github.com/MoriochoRadio/SchoolbusRFID) | RFID 태그로 통학버스 승하차를 확인 (Java(Android) · ESP8266 · Firebase) · 선배 프로젝트를 분석해 다시 만듦 | Android 앱 로직 · Firebase로 승하차 인원 실시간 집계 |

---

## 논문 · 수상 · 자격

- **논문(제1저자 2편)**
  - KKITS 2026 학술대회 — *Practical Domain Adaptation for Computer-Aided Sperm Analysis: Quality-Aware Video Normalization and Augmentation-Based Morphology Classification* (SEED)
  - 대한전자공학회 2025 추계학술대회 — AI 식품 비전검사기를 위한 데이터 수집 설계와 구현: 건빵 사례 연구
- **수상** — 교내 프로젝트(DYC) 경진대회 **대상**(L-POT, 2025.12) · AI × Design Thinking 캠프 **금상**(2025.06) · 설계교과목 성과전시회 우수상 3회(MedQueue · L-POT · SEED) · 병원임상데이터 AI 기초 교육 장려상(2025.07)
- **자격** — 정보처리기사 · TOEIC 905점 · 네이버클라우드 자격(NCA) · TOPCIT 수준 3 · 빅데이터실무활용능력 1급

---

## 교육 · 학습 기록

**AI와 자바(Spring) 풀스택 과정 7기** (2026.06 ~ 12, 6개월 / 952시간) — Java · Spring Boot · MyBatis · MariaDB · React · Next.js · AI Agent

| 저장소 | 내용 |
|---|---|
| [Spring Boot 게시판](https://github.com/MoriochoRadio/web-study-notes/tree/main/Back_end/web_edu_project/10_login_board_springboot) · [검증 기록](https://github.com/MoriochoRadio/web-study-notes/blob/main/Back_end/sync-validation-2026-10-12.md) | 수업 게시판에 개선 과제 5건(작성자 권한 · 첨부 수정 · 설정 분리 · 생성자 주입 · 로깅)을 AI 코딩 도구와 함께 적용하고, 임시 회원 2명으로 타인 글 수정 · 삭제 차단과 트랜잭션 롤백을 로컬 DB에서 실행해 확인 |
| [web-study-notes](https://github.com/MoriochoRadio/web-study-notes) · [대시보드](https://moriochoradio.github.io/web-study-notes/) | 수업 코드 · 복습 카드 · 코딩테스트 풀이와 검증을 날짜별로 정리한 학습 기록 |
| [java-texas-holdem](https://github.com/MoriochoRadio/java-texas-holdem) | Java 클래스 · 컬렉션 · 인터페이스로 구현한 2인용 텍사스 홀덤. 7장 중 최강 5장 판정 로직, AI 활용 일지, 코드 리뷰 기록 |

그 밖의 교육: 네이버클라우드 아카데미 3기(2025.12, 5일 / 40시간) · GitHub 활용 사물인터넷 프로그래밍 캠프(2025.11, 4일) · 병원임상데이터 활용 AI 기초 교육(2025.07, 5일) · AI × Design Thinking 캠프(2025.06, 4일 / 32시간)

<details>
<summary><b>학습 아카이브</b></summary>

수업 · 독학 과정을 그대로 보존한 저장소입니다.
[study-java](https://github.com/MoriochoRadio/study-java) (Java 기초 → GUI) ·
[study-algorithms](https://github.com/MoriochoRadio/study-algorithms) (알고리즘 C++/C#) ·
[study-windows-programming](https://github.com/MoriochoRadio/study-windows-programming) (WinForms/WPF) ·
[Iot-Github](https://github.com/MoriochoRadio/Iot-Github) (IoT 보드 실습 · Git 기초) ·
[study-web-basics](https://github.com/MoriochoRadio/study-web-basics) · [study-web-funsun](https://github.com/MoriochoRadio/study-web-funsun) (2020, 첫 웹)

</details>

<details>
<summary><b>개인 프로젝트 · 공모전</b></summary>

AI 코딩 도구와 함께 만들어 운영해 온 개인 프로젝트와 공모전 제출물입니다.

| 저장소 | 내용 |
|---|---|
| [nextjs-stock-dashboard](https://github.com/MoriochoRadio/nextjs-stock-dashboard) | Next.js 실시간 주식 대시보드. 직접 찾아 고친 버그 6건의 Before/After 기록 |
| [stock-briefing](https://github.com/MoriochoRadio/stock-briefing) · [사이트](https://moriochoradio.github.io/stock-briefing/) | 매일 아침 미국 · 한국 증시 브리핑 자동 생성 |
| [ai-news-curation](https://github.com/MoriochoRadio/ai-news-curation) · [사이트](https://moriochoradio.github.io/ai-news-curation/) | AI 뉴스 · 논문 · 오픈소스 매일 자동 큐레이션 |
| [ai-daily-trends](https://github.com/MoriochoRadio/ai-daily-trends) · [사이트](https://moriochoradio.github.io/ai-daily-trends/) | GitHub Trending · Hacker News · Reddit의 AI 트렌드 매일 수집 · 요약 |
| [weather-fit](https://github.com/MoriochoRadio/weather-fit) · [사이트](https://moriochoradio.github.io/weather-fit/) | 날씨 기반 코디 추천 PWA — 서버 · API 키 없이 동작 |
| [fit-atlas](https://github.com/MoriochoRadio/fit-atlas) · [사이트](https://moriochoradio.github.io/fit-atlas/) | 운동 990종 · 루틴 · 기록을 담은 로컬 우선 웹앱 |
| [multimodal-bias-vqa](https://github.com/MoriochoRadio/multimodal-bias-vqa) | 멀티모달 AI Bias 챌린지(2026.06) — 근거가 부족하면 "모름"을 고르는 VQA |
| [jump-ai-clinical-agent](https://github.com/MoriochoRadio/jump-ai-clinical-agent) | 제4회 JUMP AI 경진대회(2026.07) — 임상시험 프로토콜 사전 점검 에이전트 제안서 · CLI 프로토타입 |

그 밖에 [tarkov-korean-changes](https://github.com/MoriochoRadio/tarkov-korean-changes) · [tarkov-companion](https://github.com/MoriochoRadio/tarkov-companion) · [sauna-travel-planner](https://github.com/MoriochoRadio/sauna-travel-planner) · [sauna-science-hub](https://github.com/MoriochoRadio/sauna-science-hub) · [fundamental-regime-report](https://github.com/MoriochoRadio/fundamental-regime-report) · [evolution-garden](https://github.com/MoriochoRadio/evolution-garden) · [mindlings](https://github.com/MoriochoRadio/mindlings)

</details>

---

<sub>각 저장소 README에는 팀 구성 · 역할과 함께 <b>제가 직접 한 부분과 하지 않은 부분, 실패한 시도</b>를 적어 두었습니다. 수치는 발표 자료 · 논문 · 코드 기록에서 출처를 확인한 값이며, 측정 조건이 남아 있지 않은 것은 그렇게 밝혀 두었습니다.</sub>
