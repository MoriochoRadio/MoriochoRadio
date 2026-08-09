# 김태경 (Kim Taekyoung)

**병원정보시스템(HIS)·의료IT 분야를 목표로 하는 개발자**
건양대학교 의료IT공학과 재학 · **2027년 2월 졸업 예정**

의료 현장의 문제를 딥러닝과 웹으로 푸는 일을 해왔습니다.
학부 재학 중 **학회 논문 2편을 제1저자로 발표**했고, 그중 의료영상 AI 주제는 1인 연구와 졸업 팀 캡스톤으로 각각 끝까지 구현했습니다.
산학협력 R&D 과제에서는 데이터 파트를 맡아 식품 검사용 AI 학습 데이터셋을 설계·구축했습니다.

- **관심 분야** — 병원정보시스템(HIS), 의료 데이터, 의료영상 AI
- **연락처** — taeral04@gmail.com

---

## 의료영상 AI — 논문에서 시스템까지

### 1. 학회 논문 — AI 정자 분석의 도메인 갭 해결 (KKITS 2026)

> *Practical Domain Adaptation for Computer-Aided Sperm Analysis: Quality-Aware Video Normalization and Augmentation-Based Morphology Classification*
> **김태경(제1저자)**, 허용도(교신저자) — 건양대학교 의료IT공학과
> Proceedings of KKITS, Vol. 20, No. 1 (2026)

컴퓨터 보조 정자 분석(CASA) 모델이 **깨끗한 벤치마크에서는 잘 되지만 실제 임상 영상에서는 무너지는 문제**를 다뤘습니다.
학습 데이터(MHSMA)로 훈련한 형태 분류 모델을 실제 현미경 영상(VISEM-Tracking)에 적용하자 정상 형태율이 0.5%까지 붕괴했고, 이를 추론 비용 없는 방법만으로 해결했습니다.

| 문제 | 접근 | 결과 |
|---|---|---|
| 검출 성능 저하 | CLAHE·그레이스케일 등 픽셀 보정을 **하지 않고**, 해상도·fps·길이 사양만 통일 | 원본 대비 검출 **99.3% 유지** (픽셀 보정 시 −28.6%p) |
| 형태 분류 붕괴 | 학습 시에만 실제 영상 열화를 모사하는 `VisemStyleAugment` 증강 | 실전 정상 형태율 **0.5% → 16.3%** (WHO 기준 ≥4% 충족) |

의사 라벨링 · 기하학적 측정 · TTA · 앙상블 등 4가지 대안을 먼저 시도해 모두 실패한 뒤 얻은 결론이며, 실패 기록도 논문에 함께 실었습니다.
실제 참가자 4명의 영상(정자 크롭 1,824개)에서 전원 WHO 기준을 충족하는 것으로 검증했습니다.

<br/>

### 2. AI-CASA — 논문을 웹 서비스까지 (1인 개발)

**[sperm-ai](https://github.com/MoriochoRadio/sperm-ai)** · `v1.4.0`

현미경 영상 하나로 운동성·키네마틱·형태를 통합 분석하고 WHO 6판 기준 보고서를 출력하는 Flask 웹 시스템입니다. 기획부터 모델·웹까지 전 과정을 혼자 개발했습니다.

- **파이프라인** — YOLO11(검출) → ByteTrack(추적) → 앙상블 회귀(운동성) → EfficientNet-B3(형태 분류) → 설명형 해석
- **성과** — 동일 데이터셋(VISEM)에서 운동성 MAE **6.9%p**로 기존 논문 최고 기록(motilitAI, 7.31%p)을 상회. YOLO11 mAP@0.5 = 0.677
- **의의** — 전용 CASA 장비 없이 일반 현미경 영상과 브라우저만으로 접근 가능한 보조 분석 도구

<br/>

### 3. SEED — 졸업 팀 캡스톤, 시스템 설계·통합 담당 (2026-1)

**[seed-project](https://github.com/MoriochoRadio/seed-project)** · `Ver 1.0.0`

위 1인 연구를 5인 팀 프로젝트로 확장한 정자 자동 탐지·형태·운동성 통합 분석 시스템입니다. 모체 논문보다 높게 설정한 성능 목표를 전부 달성하고 최종 발표를 마쳤습니다.

- **역할 (ENG1)** — 시스템 구조 설계, 모듈 통합 관리, 성능 개선, 형태 분석 모델 구현
- **기술** — Python · PyTorch · YOLO11 · ByteTrack · Flask
- **프로세스** — 폭포수(Waterfall) 방법론, 단계별 산출물·검증 문서화 / Team T.O.P (PM·CM·QA·ENG1·ENG2)

---

## 산학협력 R&D — AI 식품 비전검사기 (2025)

> **AI 식품 비전검사기를 위한 데이터 수집 설계와 구현: 건빵 사례 연구**
> 김태경, 김민지, 한주혁, 조용석 — 대한전자공학회(IEIE) 2025년도 추계학술대회 (2025.11) · **제1저자**

소규모 식품 제조업체를 위한 보급형 AI 검사 시스템을 개발하는 기업 연계 과제에서 **데이터 수집·정의 파트**를 맡았습니다.
모델을 만드는 일이 아니라 **모델이 학습할 대상을 정의하는 일**이었고, 여기서 "판단 기준을 근거로 설계한다"는 것을 배웠습니다.

- **불량 클래스를 규범 기반으로 정의** — 정상·부서짐·과도한 익음·이물 혼입 4종을 Codex·UNICEF·식약처(MFDS) 기준과 공중보건 근거에 맞춰 정의. 임의로 나누지 않고 각 클래스마다 국제·국내 규정 문헌을 근거로 붙였습니다
- **정량 판정 기준 작성** — "부서짐 minor는 외곽 10\~20%, split은 2조각, fragmented는 3조각 이상", "갈변 면적 30%/70% 구간", "이물 6\~8px 이상" 등 라벨러가 흔들리지 않도록 수치화. 반사·그림자는 불량이 아니라는 예외 규칙과, 복합 결함 시 클래스 우선순위 규칙까지 명시
- **데이터셋 구축** — 224×224 단일 개체 이미지 4,066장(클래스별 약 1,000장) + 생산 라인을 모사한 다량 이미지 200장. 컨베이어 촬영 프로토콜(밀도·배치·조명·모션블러·빈 배경 샷 포함)도 함께 설계
- **라벨링·버전관리 파이프라인** — Roboflow 기반 수동 + Box Prompting·Label Assist 반자동 라벨링, 버전별 분할·전처리·증강·수정 이력을 기록해 재현성 확보. YOLO·COCO·TFRecord로 내보내 환경에 관계없이 동일하게 사용 가능하도록 구성

📂 불량 정의 근거, 정량 판정 기준, 촬영 프로토콜까지 설계 과정 전체를 정리해두었습니다 → **[food-vision-dataset-design](https://github.com/MoriochoRadio/food-vision-dataset-design)**

<sub>※ 과제 데이터셋과 내부 산출물은 기업 소유이므로 공개하지 않습니다.</sub>

---

## 공모전·챌린지

| 시기 | 대회 | 한 일 | 결과/상태 |
|---|---|---|---|
| 2026-06 | 멀티모달 AI Bias 챌린지 (DACON) — [multimodal-bias-vqa](https://github.com/MoriochoRadio/multimodal-bias-vqa) | 오프라인 Qwen2.5-VL(4-bit) + 균형 CoT 프롬프트로 "근거가 부족하면 모름"을 판별하는 VQA. 공개 BBQ로 600샘플 자체 검증셋을 만들어 실험 10회를 로그로 남기며 개선 | Public **Balanced Accuracy 0.883** |
| 2026-07 | 제4회 JUMP AI 신약개발 경진대회 — [jump-ai-clinical-agent](https://github.com/MoriochoRadio/jump-ai-clinical-agent) | 임상시험 프로토콜 사전검토(pre-review) 에이전트 제안 + 재현 가능한 CLI 프로토타입. 공개·합성 데이터만 사용, 안전 경계 명시 | 제안서 제출 (2026-07-08) |

---

## 학교 팀 프로젝트 이력

병원 대기·돌봄 앱에서 출발해 의료영상 AI를 거쳐 완성형 의료 AI 시스템까지, 4년에 걸쳐 단계적으로 범위를 넓혀왔습니다.

| 시기 | 프로젝트 | 도메인 | 담당 역할 |
|---|---|---|---|
| 2024-1 | [MedQueue](https://github.com/MoriochoRadio/MedQueue) | 병원 실시간 대기 정보 | 시스템 설계 |
| 2024-2 | [SchoolbusRFID](https://github.com/MoriochoRadio/SchoolbusRFID) | 위치 기반 어린이 하차 안전 | Android · RFID |
| 2024-2 | [ElderCaringApp](https://github.com/MoriochoRadio/ElderCaringApp) | 독거노인 건강 모니터링 | 로드셀 HW + 통계 SW |
| 2025-1 | [LungCT3DNoduleAI](https://github.com/MoriochoRadio/LungCT3DNoduleAI) | 폐 CT 결절 탐지 (정확도 78%) | PM |
| 2025-2 | [AILungandLiver](https://github.com/MoriochoRadio/AILungandLiver) | 폐·간 CT 결절 탐지 (정확도 93%) | QA |
| 2026-1 | **[SEED](https://github.com/MoriochoRadio/seed-project)** | AI 정자 탐지·형태·운동성 통합 분석 | **ENG1** (설계·통합·성능) |

2025년 의료영상 AI 라인(LungCT → AILungandLiver)은 같은 팀으로 한 시스템을 두 학기에 걸쳐 발전시킨 프로젝트입니다.
**PM에서 QA로 역할을 바꿔** 만드는 쪽과 검증하는 쪽을 모두 경험했습니다.

---

## 개인 프로젝트 — AI 활용 역량을 키우기 위한 실험

아래는 **LLM과 AI 에이전트를 실제 제품에 엮어내는 역량**을 기르려고 만든 것들입니다.
공통 구조는 `데이터 수집 → LLM 분석 → 정적 사이트 자동 배포`이며, GitHub Actions 위에 올려 서버·운영비 없이 매일 자동으로 갱신되도록 만들었습니다.
같은 구조를 도메인만 바꿔 반복 적용하면서, 어디까지 자동화가 버티고 어디서 사람이 필요한지를 확인했습니다.

| 프로젝트 | 분야 | 내용 | 스택 |
|---|---|---|---|
| [stock-briefing](https://github.com/MoriochoRadio/stock-briefing) · [데모](https://moriochoradio.github.io/stock-briefing/) | 금융 | 매일 아침 미·한 증시 브리핑을 자동 생성해 대시보드로 배포 | Actions · Gemini · Astro |
| [ai-daily-trends](https://github.com/MoriochoRadio/ai-daily-trends) · [데모](https://moriochoradio.github.io/ai-daily-trends/) | 데이터 | GitHub Trending·HN·Reddit의 AI 트렌드 매일 자동 수집·정리 | Python · 수집 파이프라인 |
| [tarkov-companion](https://github.com/MoriochoRadio/tarkov-companion) · [데모](https://moriochoradio.github.io/tarkov-companion/) | 웹앱 | 실시간 시세·가성비 분석 + 매일 자동 브리핑 | TypeScript · Actions · LLM |
| [sauna-science-hub](https://github.com/MoriochoRadio/sauna-science-hub) | 헬스케어 | PubMed 논문 90편 자동 수집 + 한글 번역 아카이브 | Python · PubMed API |
| [tarkov-korean-changes](https://github.com/MoriochoRadio/tarkov-korean-changes) | 데이터 | 게임 코드의 사일런트 변경을 매일 자동 수집·한글 해석, 반복 이벤트 안정성 자동 판정 | Python · Actions · LLM |
| [fundamental-regime-report](https://github.com/MoriochoRadio/fundamental-regime-report) | 금융 | 기업 펀더멘털 + 시장 국면(regime) 인지형 통합 분석 리포트 | Python · Claude API |
| [weather-fit](https://github.com/MoriochoRadio/weather-fit) | 웹앱 | 날씨 기반 남성 코디 추천 — 기온대별 75벌, 서버·API 키 없는 정적 PWA | TypeScript · PWA |
| [mindlings](https://github.com/MoriochoRadio/mindlings) | 시뮬레이션 | NEAT 신경망 생명체를 관찰·간섭하는 신 시점 인공생명 샌드박스 | Godot 4 · GDScript |
| [evolution-garden](https://github.com/MoriochoRadio/evolution-garden) · [데모](https://moriochoradio.github.io/evolution-garden/) | 시뮬레이션 | 137개 가중치 신경망이 돌연변이·자연선택만으로 종 분화하는 인공생명. 라이브러리 없이 단일 HTML | Vanilla JS · Canvas |
| [web-study-notes](https://github.com/MoriochoRadio/web-study-notes) · [데모](https://moriochoradio.github.io/web-study-notes/) | 학습 | 프론트엔드 수업 실습 아카이브 + 진도 대시보드 | HTML · CSS · JS |

---

## 학습 아카이브

수업·독학 과정을 그대로 보존한 저장소들입니다. 완성도보다 **학습 궤적**을 보여주는 기록입니다.

[study-algorithms](https://github.com/MoriochoRadio/study-algorithms) (알고리즘 C++/C#) ·
[study-java](https://github.com/MoriochoRadio/study-java) (Java 기초→GUI) ·
[study-windows-programming](https://github.com/MoriochoRadio/study-windows-programming) (WinForms/WPF 34챕터) ·
[web-study-notes](https://github.com/MoriochoRadio/web-study-notes) (취업아카데미 프론트/백엔드) ·
[study-web-basics](https://github.com/MoriochoRadio/study-web-basics) · [study-web-funsun](https://github.com/MoriochoRadio/study-web-funsun) (2020, 첫 웹)

---

## 기술 스택

| 구분 | 기술 |
|---|---|
| **주력** | Python · PyTorch · YOLO11 / Ultralytics · ByteTrack · Flask |
| **웹** | TypeScript · JavaScript · Astro · Tailwind CSS · Streamlit |
| **기반** | C · C++ · Java · C# · SQL |
| **데이터** | Roboflow · 데이터셋 설계 및 라벨링 기준 수립 · 버전관리 |
| **인프라** | GitHub Actions · GitHub Pages · Firebase · Git · Jupyter |
| **LLM 활용** | Claude API · Gemini API · 에이전트 워크플로우 · 프롬프트 엔지니어링 |

---

<sub>각 저장소 README에는 팀 구성·역할·아키텍처와 함께 <b>제가 직접 한 부분과 하지 않은 부분, 실패한 시도</b>를 함께 적어두었습니다.</sub>
