# 투자 AX 업무혁신 — 개인 투자자 자동화 학습과정

> 🌐 **온라인 강의노트**: <https://keerhee.github.io/invest-ax-curriculum/>
> 📦 **GitHub 레포**: <https://github.com/keerhee/invest-ax-curriculum>

> "남이 만든 시그널을 사는 게 아니라, **내 손으로 데이터·지표·뉴스·차트·RAG를 엮어
> 자기만의 자동 매매 리서치 시스템을 직접 구축한다.**"

8주 + 특별세션(SP) 구성. 각 주차마다 5개 과제, 총 **45개 과제 / 60~70시간 학습**.
참고 커리큘럼: <https://github.com/keerhee/invest-automation-curriculum>

## 📚 커리큘럼 한눈에

각 주차의 가이드(HTML)는 **강의노트 페이지**에서 클릭하여 보거나, GitHub에서는 [manuals/](manuals) 폴더의 HTML 파일을 직접 엽니다.
실습 폴더는 워크플로우 JSON과 시트가 들어 있습니다.

| 주차 | 주제 | 핵심 기술 | 강의노트 | 실습 폴더 |
|------|------|---------|---------|---------|
| **W1** | 데이터 수집 자동화 | CoinGecko · Yahoo Finance · FRED · Google Sheets | [📖 가이드](https://keerhee.github.io/invest-ax-curriculum/manuals/W1_data_collection.html) | [📂 W1 데이터수집](W1%20데이터수집) |
| **W2** | 기술적 지표 계산 | RSI · MA · 볼린저 밴드 · MACD · 수식 직접 구현 | [📖 가이드](https://keerhee.github.io/invest-ax-curriculum/manuals/W2_technical_indicators.html) | [📂 W2 기술적지표](W2%20기술적지표) |
| **W3** | 뉴스 센티먼트 분석 | Alpha Vantage · Claude Haiku · 2차원 분석 | [📖 가이드](https://keerhee.github.io/invest-ax-curriculum/manuals/W3_news_sentiment.html) | [📂 W3 뉴스센티먼트](W3%20뉴스센티먼트) |
| **W4** | 차트 Vision + 3D Verdict | Chart-IMG · Claude Vision · AI Agent | [📖 가이드](https://keerhee.github.io/invest-ax-curriculum/manuals/W4_chart_vision.html) | [📂 W4 차트Vision](W4%20차트Vision) |
| **W5** | 스케줄링 + Vector DB 기초 | Supabase pgvector · 첫 RAG · 멀티 스케줄 | [📖 가이드](https://keerhee.github.io/invest-ax-curriculum/manuals/W5_scheduling_rag.html) | [📂 W5 스케줄링RAG](W5%20스케줄링RAG) |
| **W6** | Hybrid RAG 실전 | PDF 임베딩 · Cohere Rerank · 출처 인용 Q&A | [📖 가이드](https://keerhee.github.io/invest-ax-curriculum/manuals/W6_hybrid_rag.html) | [📂 W6 HybridRAG](W6%20HybridRAG) |
| **W7** | 멀티 에이전트 | Orchestrator + 3 Sub-Agents · Message Bus | [📖 가이드](https://keerhee.github.io/invest-ax-curriculum/manuals/W7_multi_agent.html) | [📂 W7 멀티에이전트](W7%20멀티에이전트) |
| **W8** | Paper Trading + 수료 | Alpaca · Risk Guards · Bracket Order · 발표 | [📖 가이드](https://keerhee.github.io/invest-ax-curriculum/manuals/W8_paper_trading.html) | [📂 W8 PaperTrading](W8%20PaperTrading) |
| **SP** | KIS 모의투자 | OAuth · HashKey · 한국 주식 · 호가 단위 | [📖 가이드](https://keerhee.github.io/invest-ax-curriculum/manuals/SP_kis_korea.html) | [📂 SP KIS모의투자](SP%20KIS모의투자) |

## 🎯 학습 목표 (수강 후)

- **데이터 손에 잡기** — 무료 API만으로 글로벌·한국 시세, 매크로 지표, 뉴스 데이터를 매일 자동 수집
- **숫자 직접 계산** — RSI/MA/MACD를 라이브러리 없이 수식으로 구현 → 의미 이해
- **AI를 의사결정 도구로** — 뉴스 센티먼트, 차트 Vision, 멀티 에이전트로 3차원 의견 도출
- **지식 검색 시스템** — 사업보고서·공시 PDF를 Hybrid RAG로 인용 답변
- **Paper Trading 실전** — Risk Guards 통과한 시그널만 모의계좌에 자동 발주
- **한국 주식 대응** — KIS OpenAPI 모의투자로 KOSPI 종목 호가단위·HashKey 처리

## 📂 디렉터리 구조

```
invest-ax-curriculum/
├── index.html                      # 다크 테마 강의노트 진입점
├── README.md                       # 이 파일
├── manuals/                        # HTML 가이드 11종
│   ├── 00_main.html                # 본 매뉴얼 (커리큘럼 개요)
│   ├── 01_prereq.html              # 사전 준비 (계정·키·툴)
│   ├── W1_data_collection.html ~ W8_paper_trading.html
│   ├── SP_kis_korea.html
│   └── _style.css                  # 공통 스타일
├── W1 데이터수집/                   # 각 주차 폴더 — n8n JSON + 실습 xlsx
│   ├── W1.json
│   ├── W1_종목마스터.xlsx
│   └── README.md                   # 강의노트로 돌아가는 안내
└── ...
```

### 매뉴얼 (HTML로 직접 열어도 동작)

| 파일 | 강의노트 | 비고 |
|------|---------|------|
| [manuals/00_main.html](manuals/00_main.html) | [📖 보기](https://keerhee.github.io/invest-ax-curriculum/manuals/00_main.html) | 본 매뉴얼 |
| [manuals/01_prereq.html](manuals/01_prereq.html) | [📖 보기](https://keerhee.github.io/invest-ax-curriculum/manuals/01_prereq.html) | 사전 준비 |

## 🛠️ 사용 도구 (모두 무료 또는 무료 한도)

- **자동화**: n8n (Cloud 또는 Self-host Docker)
- **시세 데이터**: Yahoo Finance (무료) · CoinGecko (무료) · FRED (키 발급)
- **뉴스**: Alpha Vantage NEWS_SENTIMENT (5 req/min 무료)
- **AI**: Claude Haiku (저비용) · Claude Sonnet (Vision/Agent용) · OpenAI Embeddings
- **벡터 DB**: Supabase pgvector (무료 500MB) — RAG 주차
- **Reranking**: Cohere Rerank (무료 1000 req/month)
- **차트 이미지**: Chart-IMG API (무료 한도)
- **Paper Trading**: Alpaca Paper (무료) · 한국투자증권 모의투자 (무료)

**예상 API 비용**: 학습 전 과정 $10~$20 (대부분 무료 크레딧으로 커버)

## 🚦 사용 방법

1. **온라인** — [강의노트 메인](https://keerhee.github.io/invest-ax-curriculum/)에서 본 매뉴얼·사전 준비를 먼저 정독
2. **로컬** — 또는 `index.html` 더블클릭으로 동일하게 열람
3. W1부터 순서대로:
   1. 매뉴얼 HTML로 흐름 이해
   2. 해당 폴더 `W*.json` 을 n8n에 import
   3. 동봉 xlsx를 Google Sheets에 업로드 → Sheets Trigger 노드에서 선택
   4. Activate → 출력 검증 → 5개 과제 풀기
4. W8 종료 시점에 본인의 자동 매매 리서치 시스템 1세트 보유

## ⚠️ 안전 가이드 (꼭 읽기)

> **본 과정은 교육 목적입니다.** 8주 학습으로 실계좌 자동매매를 그대로 운용하지 마세요.

- W7까지의 모든 시그널 노드는 **출력만**합니다 (실 발주 없음)
- W8 Paper Trading은 **반드시 paper 자격증명**만 사용 — 실거래 키 절대 금지
- SP KIS는 **모의투자 계좌**만 연결 (실거래 신청 X)
- API 키는 GitHub 등 공개 저장소에 commit 금지 — n8n credential에 저장
- 실거래 적용은 별도의 백테스트·Position Sizing·DDL(Daily Drawdown Limit)·심리 학습이 필수
