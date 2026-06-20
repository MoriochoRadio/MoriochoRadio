<!-- ============================================================
  MoriochoRadio (KimTaeKyoung) — GitHub Profile README
  파일 위치: github.com/MoriochoRadio/MoriochoRadio 레포의 README.md
============================================================ -->

<h1 align="center">안녕하세요, 김태경입니다 👋</h1>

<p align="center">
  <b>의료IT를 중심에 두고, 생성형 AI를 '매일 쓰는 도구'로 다루는 개발자 지망생</b><br/>
  <sub>아이디어를 며칠 안에 <b>배포된 실제 제품</b>으로 만들고, AI·자동화로 굴러가게 합니다.</sub>
</p>

<p align="center">
  <a href="https://github.com/MoriochoRadio?tab=repositories"><img src="https://img.shields.io/badge/Repos-24-2b3137?style=flat-square&logo=github&logoColor=white"></a>
  <img src="https://img.shields.io/badge/도메인-의료IT·의료영상_AI-0a7d6b?style=flat-square">
  <img src="https://img.shields.io/badge/강점-LLM_활용·자동화_배포-7c3aed?style=flat-square">
  <img src="https://komarev.com/ghpvc/?username=MoriochoRadio&style=flat-square&color=blue&label=Profile+views">
</p>

---

건양대학교 **의료IT공학과** 에서 의료와 기술이 만나는 지점을 공부하고 있습니다.
환자 대기 시간, 어린이 안전, 독거노인 모니터링, 폐·간 CT 결절 탐지까지 — *"의료진뿐 아니라 사람(환자) 본인을 위한 도구"* 를 만드는 데 관심이 있습니다.

그 관심을 푸는 방식으로 **생성형 AI(Claude·Gemini)와 자동화 파이프라인**을 일상적으로 사용합니다.
최근 한 달 동안 데이터 수집 → LLM 분석 → 정적 사이트 빌드 → 자동 배포까지 **서버·비용 0원으로 매일 스스로 돌아가는 제품**을 여러 개 만들어 공개했습니다.

```
🏥 주 진로     의료IT · 병원정보시스템(HIS) · 의료영상 AI
🧠 핵심 역량   LLM(Claude/Gemini) 오케스트레이션 · GitHub Actions 자동화 · 웹 배포
🧱 기반        소프트웨어공학(C/C++/Java/C#) · 데이터 파이프라인 · 데스크탑/모바일 앱
```

---

## 🚀 대표 작업 — "AI를 도구로 굴린다"의 증거

> 모두 **라이브로 동작하는** 프로젝트입니다. 데이터 수집·LLM 분석·배포가 사람 손 없이 매일 자동으로 돌아갑니다.

| 프로젝트 | 한 줄 소개 | 핵심 스택 | 링크 |
|---|---|---|---|
| 📈 **[stock-briefing](https://github.com/MoriochoRadio/stock-briefing)** | 매일 아침 7시 미·한 증시 맞춤 브리핑을 **AI가 작성**해 대시보드로 자동 배포. 서버·비용 0원 | GitHub Actions · **Gemini API** · Astro 5 · Tailwind · yfinance | [▶ 데모](https://moriochoradio.github.io/stock-briefing/) |
| 🎯 **[tarkov-companion](https://github.com/MoriochoRadio/tarkov-companion)** | 실시간 시세·가성비 분석 + **매일 AI 자동 작성 일일 브리핑**을 더한 게임 컴패니언 웹 | TypeScript · GitHub Actions · LLM · GitHub Pages | [▶ 데모](https://moriochoradio.github.io/tarkov-companion/) |
| 🧬 **[evolution-garden](https://github.com/MoriochoRadio/evolution-garden)** | 137개 가중치의 신경망 뇌가 **돌연변이·자연선택만으로 종 분화**하는 인공생명 시뮬레이터 (단일 HTML, 무의존성) | Vanilla JS · Canvas 2D · 신경망 직접 구현 | [▶ 데모](https://moriochoradio.github.io/evolution-garden/) |
| 📊 **[fundamental-regime-report](https://github.com/MoriochoRadio/fundamental-regime-report)** | KOSPI200 321개 기업(상폐 포함)의 펀더멘털 + 시장 국면을 **ML + LLM**으로 통합 분석 | Python · ML · **Claude** · Streamlit | [코드](https://github.com/MoriochoRadio/fundamental-regime-report) |
| 📰 **[ai-daily-trends](https://github.com/MoriochoRadio/ai-daily-trends)** | GitHub Trending·HN·Reddit·SNS의 **AI 트렌드를 매일 자동 수집·정리**하는 정적 사이트 | Python · 자동 수집 파이프라인 · GitHub Actions | [▶ 데모](https://moriochoradio.github.io/ai-daily-trends/) |
| 🛠️ **[tarkov-korean-changes](https://github.com/MoriochoRadio/tarkov-korean-changes)** | 게임 변경사항을 **매일 한글로 자동 번역·해석**하고 안정성까지 자동 판정하는 정적 웹 | Python · LLM 번역 · 규칙 기반 판정 | [▶ 데모](https://moriochoradio.github.io/tarkov-korean-changes/) |

<sub>👉 이 프로젝트들이 공통으로 보여주는 것: <b>LLM API 오케스트레이션 · GitHub Actions(cron) 자동화 · 데이터 수집/가공 · 무료 풀스택 배포(Astro/Tailwind/GitHub Pages)</b> — 즉, AI를 한 번 써보는 수준이 아니라 <b>운영 가능한 제품으로 엮어내는</b> 능력.</sub>

---

## 🔬 의료영상 AI 라인 — 한 시스템을 두 학기, 두 역할로

가장 깊게 파고든 흐름은 **CT 결절 탐지 AI** 입니다. 같은 팀(**T.O.P**)에서 한 시스템을 두 학기에 걸쳐 발전시켰고, 그 과정에서 서로 다른 역할을 맡아 봤습니다.

```
        2025-1  LungCT3DNoduleAI          2025-2  AILungandLiver (L-POT)
        ────────────────────────         ──────────────────────────────
도메인   폐 CT 결절                  →     폐 + 간 CT 결절  (다중 부위 확장)
모델     3D Voxel CNN (4-branch)     →     SpiralNet+PointNet+Transformer+MeshCNN
정확도   78%                         →     93%  (+15%p)
인프라   Jupyter/Colab + Streamlit   →     PyQt6 데스크탑 앱 + exe 배포
내 역할  PM (일정·진척도·전처리)      →     QA (품질·위험·시험)
```

- **PM 으로** 6명 팀의 일정·산출물을 책임지며 *"AI 모델 지식 부족"* 같은 어려움을 직접 겪었고,
- 다음 학기 **QA 로** 그 경험을 위험 관리 계획서의 *"치명적 위험"* 으로 박아 넣었습니다.
- *안 해본 역할을 일부러 골라* 한 시스템을 다른 관점에서 바라보는 경험을 쌓았습니다.

지금은 마지막 학기 캡스톤 **[seed-project](https://github.com/MoriochoRadio/seed-project)** ·**[sperm-ai](https://github.com/MoriochoRadio/sperm-ai)** (AI 정자 운동성 분석)으로 의료영상 AI 경험을 이어가고 있습니다. → [▶ seed-project 데모](https://moriochoradio.github.io/seed-project/)

---

## 🩺 학부 프로젝트 타임라인 — 헬스케어·케어 도메인

앱·IoT 에서 시작해 의료영상 AI 로 이어지는 흐름입니다.

| 시기 | 프로젝트 | 도메인 | 본인 역할 |
|---|---|---|---|
| 2024-1 | [MedQueue](https://github.com/MoriochoRadio/MedQueue) | 병원 실시간 대기 정보 | 시스템 설계 |
| 2024-2 | [SchoolbusRFID](https://github.com/MoriochoRadio/SchoolbusRFID) | 위치 기반 어린이 하차 안전 | Android·RFID |
| 2024-2 | [ElderCaringApp](https://github.com/MoriochoRadio/ElderCaringApp) | 독거노인 건강 모니터링 | 로드셀 HW + 통계 SW |
| **2025-1** | [LungCT3DNoduleAI](https://github.com/MoriochoRadio/LungCT3DNoduleAI) | 폐 CT 결절 탐지 (78%) | **PM** |
| **2025-2** | [AILungandLiver](https://github.com/MoriochoRadio/AILungandLiver) | 폐+간 CT 결절 탐지 (93%) | **QA** |

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

**AI · 자동화**

![Claude](https://img.shields.io/badge/Claude_API-D97757?style=flat-square&logo=anthropic&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini_API-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)

**웹 · 앱 · 데이터**

![Astro](https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![PyQt](https://img.shields.io/badge/PyQt6-41CD52?style=flat-square&logo=qt&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-222222?style=flat-square&logo=githubpages&logoColor=white)

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
