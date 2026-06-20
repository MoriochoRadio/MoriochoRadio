<!-- ============================================================
  MoriochoRadio (KimTaeKyoung) — GitHub Profile README
  파일 위치: github.com/MoriochoRadio/MoriochoRadio 레포의 README.md
============================================================ -->

<h1 align="center">안녕하세요, 김태경입니다 👋</h1>

<p align="center">
  <b>병원·의료IT를 진로로 두고, AI를 도구로 다뤄 문제를 푸는 개발자 지망생</b><br/>
  <sub>의료 현장의 문제를 앱·IoT·의료영상 AI로 풀어왔고, 곁가지로 1인 프로젝트도 꾸준히 배포합니다.</sub>
</p>

<p align="center">
  <a href="https://github.com/MoriochoRadio?tab=repositories"><img src="https://img.shields.io/badge/Repos-24-2b3137?style=flat-square&logo=github&logoColor=white"></a>
  <img src="https://img.shields.io/badge/주_진로-병원정보시스템·의료IT-0a7d6b?style=flat-square">
  <img src="https://img.shields.io/badge/강점-의료영상_AI·LLM_활용·배포-7c3aed?style=flat-square">
  <img src="https://komarev.com/ghpvc/?username=MoriochoRadio&style=flat-square&color=blue&label=Profile+views">
</p>

---

건양대학교 **의료IT공학과** 재학 중이며, 졸업 후 **병원·병원정보시스템(HIS)의 개발·유지보수·관리, 의료IT** 분야에서 일하는 것을 목표로 합니다.
환자 대기 시간, 어린이 안전, 독거노인 모니터링, CT 결절 탐지, 정자 형태·운동성 분석까지 — *"의료진뿐 아니라 사람(환자) 본인을 위한 도구"* 를 4년간 학교 팀 프로젝트로 하나씩 만들어 왔습니다.

문제를 푸는 방식으로 **AI(딥러닝·생성형 AI)를 일상적인 도구**로 사용하며, 학교 프로젝트 밖에서도 **혼자서 여러 분야의 제품을 만들어 배포**해 왔습니다.

```
🏥 주 진로     병원 · 병원정보시스템(HIS) · 의료IT 개발/유지보수/관리
🔬 핵심 경험   의료영상·의료 AI 시스템 (객체탐지·추적·3D 영상, 팀 캡스톤)
🧠 도구로서의 AI   딥러닝(YOLO/PyTorch) · LLM(Claude/Gemini) · 자동화 배포
🧱 기반        소프트웨어공학(C/C++/Java/C#) · 앱/데스크탑/웹 · 데이터 파이프라인
```

---

## 🏥 의료IT공학 — 케어 앱에서 의료 AI 시스템까지

진로와 직결되는 **학교 팀 프로젝트** 흐름입니다. 병원 대기·돌봄 앱에서 출발해 → 의료영상 AI → **완성형 의료 AI 시스템**으로 단계적으로 성장했습니다.

| 시기 | 프로젝트 | 도메인 | 본인 역할 |
|---|---|---|---|
| 2024-1 | [MedQueue](https://github.com/MoriochoRadio/MedQueue) | **병원 실시간 대기 정보** (HIS 성격) | 시스템 설계 |
| 2024-2 | [SchoolbusRFID](https://github.com/MoriochoRadio/SchoolbusRFID) | 위치 기반 어린이 하차 안전 | Android · RFID |
| 2024-2 | [ElderCaringApp](https://github.com/MoriochoRadio/ElderCaringApp) | 독거노인 건강 모니터링 | 로드셀 HW + 통계 SW |
| 2025-1 | [LungCT3DNoduleAI](https://github.com/MoriochoRadio/LungCT3DNoduleAI) | 폐 CT 결절 탐지 (78%) | PM |
| 2025-2 | [AILungandLiver](https://github.com/MoriochoRadio/AILungandLiver) | 폐+간 CT 결절 탐지 (93%) | QA |
| **2026-1** | **[🌱 SEED](https://github.com/MoriochoRadio/seed-project)** | **AI 정자 탐지·형태·운동성 통합 분석** | **ENG1 (시스템 설계·통합·성능)** |

<sub>성장 메모: 2025년 의료영상 AI 라인(LungCT → AILungandLiver)에서는 같은 팀으로 한 시스템을 두 학기에 걸쳐 발전시키며 **PM → QA** 로 역할을 바꿔, 만드는 쪽과 검증하는 쪽을 모두 경험했습니다. (정확도 78% → 93%)</sub>

### 🌱 대표작 — SEED · AI 기반 정자 자동 탐지 및 형태·운동성 통합 분석 시스템

> **모체논문보다 높게 설정한 성능목표를 전부 달성한 캡스톤 프로젝트.** 2026-1 융합캡스톤디자인 I 최종발표 완료 (`Ver 1.0.0`).

- **무엇** — 현미경 영상 속 정자를 AI가 **자동 검출·추적**하고, **형태·운동성(키네마틱 지표)을 정량 평가**하는 시스템 (WHO 기준 참고)
- **내 역할 (ENG1)** — 시스템 구조 설계·제작, 모듈 **통합 관리**, **성능 개선**, 그리고 **형태 분석 모델 구현**
- **기술** — `Python` · `PyTorch` · `YOLO11(Ultralytics)` · `ByteTrack(추적)` · `Flask` / 폭포수(Waterfall) 방법론으로 단계별 산출물·검증
- **팀** — Team **T.O.P** (PM·CM·QA·ENG1·ENG2 5인 분산형 구성)
- 📂 발표 슬라이드 흐름을 그대로 옮긴 상세 README · 산출물 · Quick Start 포함 → **[저장소 보기](https://github.com/MoriochoRadio/seed-project)**

<sub>※ 각 학교 프로젝트 README에는 팀 구성·역할·아키텍처·산출물과 함께, 내가 한 부분/못한 부분을 정직하게 적어 두었습니다.</sub>

---

## 🚀 1인 프로젝트 — 의료 AI 단독 연구부터 다양한 분야까지

학교 밖에서도 **혼자서** 기획·구현·배포까지 끝냅니다. 의료 AI를 단독으로 연구하며, 그 외에도 여러 분야의 제품을 **AI·자동화로 실제 동작하게** 만들어 왔습니다.

### 🔬 대표 솔로작 — AI-CASA · AI 기반 정자 종합 분석 시스템 ([sperm-ai](https://github.com/MoriochoRadio/sperm-ai))

> **SEED 팀 캡스톤의 베이스라인으로 시도한, 혼자서 웹까지 완성한 의료 AI 프로젝트.**

- **무엇** — 정자 현미경 영상 하나로 **운동성·키네마틱(VCL/VSL/LIN 등)·형태를 통합 분석**하고 WHO 6판 기준 설명형 보고서를 출력하는, 누구나 영상을 올려 쓰는 **Flask 웹 시스템** (`v1.4.0`, 전 과정 1인 개발)
- **파이프라인** — `YOLO11`(탐지) → `ByteTrack`(추적) → 앙상블 회귀(운동성) → `EfficientNet-B3`(형태 분류) → 설명형 해석
- **성과** — 동일 데이터셋(VISEM)에서 운동성 MAE **6.9%p** 로 기존 논문 최고(motilitAI 7.31%p) **초과 달성**, YOLO11 mAP50 0.677
- **의의** — 수천만 원 전용 장비 없이 **일반 현미경 영상 + 웹 브라우저**만으로 접근 가능 (병원 방문 전 보조 분석)

<sub>※ 이 솔로 연구 경험이 이후 졸업 팀 캡스톤 <b><a href="https://github.com/MoriochoRadio/seed-project">SEED</a></b> 로 이어졌습니다.</sub>

### 그 외 — 다른 분야도 혼자, 끝까지 배포

아래는 모두 **라이브로 동작**하며, 데이터 수집·LLM 분석·배포가 사람 손 없이 자동으로 돌아갑니다.

| 프로젝트 | 분야 | 한 줄 소개 | 핵심 스택 | 링크 |
|---|---|---|---|---|
| 📈 **[stock-briefing](https://github.com/MoriochoRadio/stock-briefing)** | 금융·자동화 | 매일 아침 미·한 증시 브리핑을 **AI가 작성**해 대시보드로 자동 배포 (서버·비용 0원) | GitHub Actions · Gemini · Astro · Tailwind | [▶ 데모](https://moriochoradio.github.io/stock-briefing/) |
| 📊 **[fundamental-regime-report](https://github.com/MoriochoRadio/fundamental-regime-report)** | 금융·ML | KOSPI200 321개 기업(상폐 포함) 펀더멘털 + 시장 국면을 **ML + LLM**으로 통합 분석 | Python · ML · Claude · Streamlit | [코드](https://github.com/MoriochoRadio/fundamental-regime-report) |
| 🧬 **[evolution-garden](https://github.com/MoriochoRadio/evolution-garden)** | 시뮬레이션 | 137개 가중치 신경망 뇌가 **돌연변이·자연선택만으로 종 분화**하는 인공생명 (단일 HTML, 무의존성) | Vanilla JS · Canvas · 신경망 직접 구현 | [▶ 데모](https://moriochoradio.github.io/evolution-garden/) |
| 🎯 **[tarkov-companion](https://github.com/MoriochoRadio/tarkov-companion)** | 웹앱 | 실시간 시세·가성비 분석 + **매일 AI 자동 작성 브리핑** 게임 컴패니언 웹 | TypeScript · GitHub Actions · LLM | [▶ 데모](https://moriochoradio.github.io/tarkov-companion/) |
| 📰 **[ai-daily-trends](https://github.com/MoriochoRadio/ai-daily-trends)** | 데이터·자동화 | GitHub Trending·HN·Reddit·SNS의 **AI 트렌드를 매일 자동 수집·정리** | Python · 수집 파이프라인 · Actions | [▶ 데모](https://moriochoradio.github.io/ai-daily-trends/) |
| 🛠️ **[tarkov-korean-changes](https://github.com/MoriochoRadio/tarkov-korean-changes)** | 자동화 | 변경사항을 **매일 한글로 자동 번역·해석**하고 안정성까지 자동 판정 | Python · LLM 번역 · 규칙 판정 | [▶ 데모](https://moriochoradio.github.io/tarkov-korean-changes/) |

<sub>👉 분야는 달라도 공통으로 보여주는 것: <b>혼자 기획→구현→배포까지 끝내는 실행력</b>, 그리고 <b>AI를 한 번 써보는 수준이 아니라 운영되는 제품으로 엮어내는</b> 능력.</sub>

---

## 🛠️ 기술 스택

**언어**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white)

**의료·AI**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![YOLO](https://img.shields.io/badge/YOLO11-00FFFF?style=flat-square&logo=ultralytics&logoColor=black)
![Claude](https://img.shields.io/badge/Claude_API-D97757?style=flat-square&logo=anthropic&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini_API-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)

**웹 · 앱 · 인프라**

![Astro](https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![PyQt](https://img.shields.io/badge/PyQt6-41CD52?style=flat-square&logo=qt&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

---

## 📊 GitHub at a glance

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=MoriochoRadio&show_icons=true&hide_border=true&include_all_commits=true&count_private=true&theme=default" alt="GitHub Stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MoriochoRadio&layout=compact&hide_border=true&langs_count=8&theme=default" alt="Top Languages" />
</p>

---

## 📫 연락

GitHub: [@MoriochoRadio](https://github.com/MoriochoRadio) · Email: taeral04@gmail.com

<sub>각 레포의 README 에는 *"5년 뒤의 내가 봐도 떳떳하도록"* 내가 한 부분과 안 한 부분, 잘된 것과 부족했던 것을 정직하게 적어 두었습니다. 학습 과정의 흔적(오타 포함)도 일부러 남겨 두었습니다.</sub>
