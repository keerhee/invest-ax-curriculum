# W3 — 뉴스 센티먼트 분석

> 🌐 **강의노트**: <https://keerhee.github.io/invest-ax-curriculum/manuals/W3_news_sentiment.html>
> 🏠 **전체 강의노트 홈**: <https://keerhee.github.io/invest-ax-curriculum/>
> 📦 **GitHub 레포**: <https://github.com/keerhee/invest-ax-curriculum>

**핵심 기술**: Alpha Vantage · Claude Haiku · 2차원 (감정 × 영향도)

## 📁 폴더 내 파일

| 파일 | 설명 |
|------|------|
| [`W3.json`](W3.json) | n8n 워크플로우 — Cron → Alpha Vantage → Claude Haiku → Sheets/Slack |
| [`W3_뉴스이력.xlsx`](W3_뉴스이력.xlsx) | 출력 시트 헤더 (10컬럼) — 워크플로우가 채움 |

## 🚦 사용 방법

1. [📖 W3 강의노트](https://keerhee.github.io/invest-ax-curriculum/manuals/W3_news_sentiment.html)에서 흐름 이해
2. `W3.json` 을 n8n에 import (Workflows → Add → Import from file)
3. `W3_뉴스이력.xlsx` 을 Google Drive에 업로드 → Google Sheets로 변환
4. n8n Sheets Trigger 노드를 본인 시트로 다시 선택
5. 각 노드의 자격증명(`PUT_YOUR_*`) 본인 키로 교체
6. Activate → 출력 검증 → 5개 과제 풀기

## ↔️ 다른 주차로 이동

[← W2 기술적지표](https://github.com/keerhee/invest-ax-curriculum/tree/main/W2%20%EA%B8%B0%EC%88%A0%EC%A0%81%EC%A7%80%ED%91%9C) · [→ W4 차트Vision](https://github.com/keerhee/invest-ax-curriculum/tree/main/W4%20%EC%B0%A8%ED%8A%B8Vision)

---

📚 [전체 커리큘럼 README](https://github.com/keerhee/invest-ax-curriculum/blob/main/README.md) · 🌐 [강의노트 홈](https://keerhee.github.io/invest-ax-curriculum/)
