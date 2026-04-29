# W8 — Paper Trading + 수료

> 🌐 **강의노트**: <https://keerhee.github.io/invest-ax-curriculum/manuals/W8_paper_trading.html>
> 🏠 **전체 강의노트 홈**: <https://keerhee.github.io/invest-ax-curriculum/>
> 📦 **GitHub 레포**: <https://github.com/keerhee/invest-ax-curriculum>

**핵심 기술**: Alpaca Paper · 4 Risk Guards · Bracket Order

## 📁 폴더 내 파일

| 파일 | 설명 |
|------|------|
| [`W8.json`](W8.json) | n8n 워크플로우 — Webhook → Account+Positions → 4 Risk Guards → Bracket |
| [`W8_주문이력.xlsx`](W8_주문이력.xlsx) | Paper 주문이력 시트 (10컬럼) |

## 🚦 사용 방법

1. [📖 W8 강의노트](https://keerhee.github.io/invest-ax-curriculum/manuals/W8_paper_trading.html)에서 흐름 이해
2. `W8.json` 을 n8n에 import (Workflows → Add → Import from file)
3. `W8_주문이력.xlsx` 을 Google Drive에 업로드 → Google Sheets로 변환
4. n8n Sheets Trigger 노드를 본인 시트로 다시 선택
5. 각 노드의 자격증명(`PUT_YOUR_*`) 본인 키로 교체
6. Activate → 출력 검증 → 5개 과제 풀기

## ↔️ 다른 주차로 이동

[← W7 멀티에이전트](https://github.com/keerhee/invest-ax-curriculum/tree/main/W7%20%EB%A9%80%ED%8B%B0%EC%97%90%EC%9D%B4%EC%A0%84%ED%8A%B8) · [→ SP KIS모의투자](https://github.com/keerhee/invest-ax-curriculum/tree/main/SP%20KIS%EB%AA%A8%EC%9D%98%ED%88%AC%EC%9E%90)

---

📚 [전체 커리큘럼 README](https://github.com/keerhee/invest-ax-curriculum/blob/main/README.md) · 🌐 [강의노트 홈](https://keerhee.github.io/invest-ax-curriculum/)
