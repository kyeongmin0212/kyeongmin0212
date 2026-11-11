# 노경민 (Kyeongmin Noh)

AI를 **실제 동작하는 서비스**로 만드는 데 관심이 있습니다.
컴퓨터공학과 4학년.

- 🏆 **학술대회 우수논문상** (1저자) — 2025 한국스마트미디어학회·한국전자거래학회 춘계학술대회
- 📄 **1저자 논문 2편** 
- 🤖 **LLM 애플리케이션** — LangGraph · RAG · Tool Calling · 환각 방지 · 레이트리밋 대응

<br>

## Tech Stack

**LLM · AI**
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Gemini](https://img.shields.io/badge/Vertex_AI_Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)

**Backend**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

**Frontend**
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)

**DevOps · Cloud**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

<br>

## 팀 프로젝트

> 조직 계정 소속이라 아래에 담당 범위를 함께 적었습니다.

### 🔹 [AI's Eye](https://github.com/aivle-b-t24/ai-s-eye) — AICC 모듈 담당
`KT AIVLE School 9기 AI트랙 빅프로젝트` · 2026.7~8 · 팀 6인

매장 CCTV 영상과 주문 정보로 매장 상황을 분석하는 B2B 서비스.
**AI 상담(AICC) 모듈 전체를 담당**했습니다. — 커밋 45건(머지 제외) / +4,980 · −977

- **Gemini Tool Calling** — 질문 유형별 Tool 분기, 자동호출 5회 제한으로 무한루프 차단
- **정책 RAG** — 전체 나열 대신 관련 정책만 검색, 관련도 필터(margin) 적용
- **환각 방지** — 지점명·동이름 고정, evidence 숫자만 사용, 빈 데이터면 분석 생략
- **레이트리밋 대응** — Vertex AI 임베딩 분당 5회 제한 병목을 무료티어 키 분리로 해소
- **멀티턴 대화** — 이전 history 전달로 지시대명사 맥락 유지
- **상권 분석** — SGIS 연동으로 혼잡 원인 추정

`FastAPI` `Vertex AI (Gemini)` `RAG` `PostgreSQL` `Docker` `GCP`

<br>

### 🔹 [CodeTrace](https://github.com/CodeTrace-app/codetrace-backend) — 백엔드 기능 8개 담당
`멋쟁이사자처럼 대학 14기 해커톤` · 2026.8~ · 팀 6인 (백엔드 2명 중 1명)

신입 개발자를 위한 코드 온보딩 도구. 코드가 *왜* 그렇게 작성되었는지와
*수정 시 영향 범위*를 보여줍니다. — PR 8건 / +5,842 · −129

| PR | 기능 |
|---|---|
| #36 | GitHub App 인증 연동 (RS256 JWT) |
| #37 | 레포 등록·재인덱싱·대시보드 API |
| #38 | 커밋·PR 이력 수집 + 심볼 근거 연결 |
| #44 | LLM 배경 요약 + 맥락 API |
| #57 | PR 웹훅 + 경고 코멘트 봇 |
| #58 | 질의 이력 조회 + 90일 보존 정책 |

기능마다 테스트를 동반 작성했습니다 (본인 작성 약 2,800줄).

`FastAPI` `PostgreSQL` `SQLAlchemy` `tree-sitter` `Docker` `pytest`
🔗 [서비스](https://codetrace-frontend.vercel.app)

<br>

### 🔹 [Imagineers-Coin](https://github.com/kyeongmin0212/Imagineers-Coin) — LSTM 암호화폐 자동매매 봇
`SW 전공·융합동아리 AFE → 졸업작품` · 2025.03 ~ · 팀 4인 · **대표학생**
과기정통부 SW중심대학사업 과제 산출물 (2023-0-00028)

동아리 프로젝트로 시작해 졸업작품으로 발전시킨 자동매매 시스템입니다.

- **LSTM 2층(128→64) + Dense 2층**으로 다음날 종가 예측
  (60일 시퀀스 · 피처 4개: 종가·거래량·RSI·MACD)
- 기술지표 6종(Bollinger·RSI·MACD·ADX·ATR·EMA) + 공포탐욕지수 + 뉴스 RSS + OpenAI 시장분석
- **트레일링 스탑**, 오더북 잔량 기반 최적 매수호가 산출, 손실 종목 블랙리스트(24h)
- `RateLimiter`·`FileLock`·지수 백오프 재시도로 24시간 무인 운영
- 텔레그램 알림 + 웹 대시보드
- 실거래 238건 운용 후 **한계를 직접 진단** (폴링 주기 제약, 매매 로직 중복)

`Python` `TensorFlow/Keras` `PyUpbit` `OpenAI API` `Telegram Bot API`

<br>

## 교육 과정

### 🔹 [LKELION-Code](https://github.com/kyeongmin0212/LKELION-Code) — Java 백엔드 PBL (Mission 00~10)
`멋쟁이사자처럼 대학 14기` · 2026.04 ~ 07 · 커밋 28건 · PR 9건

객체지향 → **IoC/DI 직접 구현** → Spring Boot 전환 → REST API → JPA →
연관관계·트랜잭션 → 전역 예외 처리·FE 연동까지 단계적으로 수행.
미션마다 브랜치를 파고 PR로 머지했습니다.

`Java` `Spring Boot` `JPA` `Maven`

<br>

### 🔹 KT AIVLE School 미니프로젝트 1~6차
`2026.04 ~ 06` · 분석형 AI → 생성형 AI → 서비스 개발 → 클라우드

| 차수 | 프로젝트 | 핵심 |
|---|---|---|
| 1차 | 고객 만족도 예측 (**조장**) | 전처리 함수화 · 다지표 비교 후 미세조정 모델 채택 |
| 2차 | **AI 강사 Agent** | LangGraph 10노드 · PPT → 강의 영상 자동 생성 (멀티모달 LLM · TTS · SRT · FFmpeg) |
| 3차 | **리뷰 분석 AI** | LangSmith 파이프라인 모니터링 · ABSA 속성별 감성 분석 |
| 4차 | [BookShelf](https://github.com/owlooo/AIVLE_09_m_4th_22) | OpenAI 이미지 생성·자동 태깅 · 프론트 UI 담당 (9커밋) |
| 5·6차 | 도서관리시스템 | Spring Boot 백엔드 → **K8S 배포 파이프라인** (본인: OpenAI 연동) |

<br>

## 논문

| 제목 | 저자 | 발표 |
|---|---|---|
| 빅데이터 기반 LSTM 예측 모델을 활용한 암호화폐 자동매매 시스템 연구 | **1저자** | 2025 춘계학술대회 · 🏆 **우수논문상** |
| 빅데이터 기반 시계열 예측을 활용한 주식 자동매매 시스템 연구 | **1저자** | 봄철 종합학술대회 |
