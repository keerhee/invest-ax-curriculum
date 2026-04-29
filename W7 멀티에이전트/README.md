# W7 — 멀티 에이전트

> 🌐 **강의노트**: <https://keerhee.github.io/invest-ax-curriculum/manuals/W7_multi_agent.html>
> 🏠 **전체 강의노트 홈**: <https://keerhee.github.io/invest-ax-curriculum/>
> 📦 **GitHub 레포**: <https://github.com/keerhee/invest-ax-curriculum>

**핵심 기술**: Orchestrator + 3 Sub-Agents (Price·News·Chart) · Message Bus

## 📁 폴더 내 파일

| 파일 | 설명 |
|------|------|
| [`W7.json`](W7.json) | n8n 워크플로우 본편 — Webhook → Switch → 3 Sub-Agents → Orchestrator |
| [`W7_의견이력.xlsx`](W7_의견이력.xlsx) | 에이전트 의견이력 시트 (8컬럼) |
| 💎 [`W7_BONUS_종합분석.json`](W7_BONUS_%EC%A2%85%ED%95%A9%EB%B6%84%EC%84%9D.json) | **보너스** — NotebookLM 8차원 종합 분석 → Gmail+Slack (매일 평일 08:00 자동) |
| 💎 [`W7_BONUS_분석큐.xlsx`](W7_BONUS_%EB%B6%84%EC%84%9D%ED%81%90.xlsx) | **보너스** — 라운드로빈 분석 큐 (5종목 샘플) |
| 💎 [`W7_BONUS_보고서이력.xlsx`](W7_BONUS_%EB%B3%B4%EA%B3%A0%EC%84%9C%EC%9D%B4%EB%A0%A5.xlsx) | **보너스** — 일일 발송 이력 (10컬럼) |

## 🚦 사용 방법 (본편)

1. [📖 W7 강의노트](https://keerhee.github.io/invest-ax-curriculum/manuals/W7_multi_agent.html)에서 흐름 이해 (본편 + 💎 보너스)
2. `W7.json` 을 n8n에 import (Workflows → Add → Import from file)
3. `W7_의견이력.xlsx` 을 Google Drive에 업로드 → Google Sheets로 변환
4. n8n Sheets Trigger 노드를 본인 시트로 다시 선택
5. 각 노드의 자격증명(`PUT_YOUR_*`) 본인 키로 교체
6. Activate → 출력 검증 → 5개 과제 풀기

## 💎 보너스 — 매일 종합 투자 보고서 (NotebookLM 8차원)

**프롬프트 출처**: 타민더마켓 © 2025 — "노트북LM 전용 주식 분석 프롬프트 모음"
([유튜브 '타민더마켓'](https://www.youtube.com/@타민더마켓))

본편의 3 Sub-Agent를 **8개 분석 차원**으로 확장하고, 매일 평일 08:00에 분석큐의 다음 ticker 1개를 자동 분석해 종합 HTML 보고서를 운용팀 메일과 Slack #research-daily 로 발송합니다.

### 8 Sub-Agent
1. **재무 트렌드** — 매출/마진/FCF + 변곡점
2. **세그먼트** — 사업부별 매출/마진 + 믹스
3. **경제적 해자** — Moat Grade(A/B/C/D)
4. **Risk Factors** — 새로운/강화/완화된 리스크
5. **CEO 말바뀜** — 약속 적중률 %
6. **약속 이행** — 정직성 등급(A/B/C/D)
7. **Bear Case** — 반대 논리 12개
8. **소스 갭** — 누락 데이터

### 보너스 셋업 절차
1. `W7_BONUS_종합분석.json` 을 n8n에 import (23 노드)
2. **W6 BONUS Qdrant Hybrid 워크플로우가 먼저 활성화돼 있어야 함** (이 워크플로우가 `/qdrant-hybrid` webhook 호출)
3. `W7_BONUS_분석큐.xlsx` + `W7_BONUS_보고서이력.xlsx` 를 Google Drive에 업로드 → Sheets 변환
4. 분석큐에 본인 관심종목 5~10개 등록 (active=TRUE)
5. n8n credential: Anthropic Claude API + Gmail OAuth + Slack Webhook
6. Cron Trigger Activate → 다음 평일 08:00 KST에 자동 발송 시작

### 비용
8 Sub-Agent (Haiku) + 1 Orchestrator (Sonnet) ≈ **$0.05/종목 · 1회**
매일 평일 1종목 × 22일 = 약 **$1.1/월**

### 라운드로빈 순환
큐의 `last_analyzed`가 가장 오래된 ticker를 매일 1개 pick → 발송 후 갱신.
5종목이면 5영업일 주기, 7종목이면 7영업일 주기로 분석.

## ↔️ 다른 주차로 이동

[← W6 HybridRAG](https://github.com/keerhee/invest-ax-curriculum/tree/main/W6%20HybridRAG) · [→ W8 PaperTrading](https://github.com/keerhee/invest-ax-curriculum/tree/main/W8%20PaperTrading)

---

📚 [전체 커리큘럼 README](https://github.com/keerhee/invest-ax-curriculum/blob/main/README.md) · 🌐 [강의노트 홈](https://keerhee.github.io/invest-ax-curriculum/)
