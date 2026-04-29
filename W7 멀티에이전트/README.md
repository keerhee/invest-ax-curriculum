# W7 — 멀티 에이전트

> 🌐 **강의노트**: <https://keerhee.github.io/invest-ax-curriculum/manuals/W7_multi_agent.html>
> 🏠 **전체 강의노트 홈**: <https://keerhee.github.io/invest-ax-curriculum/>
> 📦 **GitHub 레포**: <https://github.com/keerhee/invest-ax-curriculum>

**핵심 기술**: Orchestrator + 3 Sub-Agents (Price·News·Chart) · Message Bus

## 📁 폴더 내 파일

| 파일 | 설명 |
|------|------|
| [`W7.json`](W7.json) | n8n 워크플로우 — Webhook → Switch → 3 Sub-Agents → Orchestrator |
| [`W7_의견이력.xlsx`](W7_의견이력.xlsx) | 에이전트 의견이력 시트 (8컬럼) |

## 🚦 사용 방법

1. [📖 W7 강의노트](https://keerhee.github.io/invest-ax-curriculum/manuals/W7_multi_agent.html)에서 흐름 이해
2. `W7.json` 을 n8n에 import (Workflows → Add → Import from file)
3. `W7_의견이력.xlsx` 을 Google Drive에 업로드 → Google Sheets로 변환
4. n8n Sheets Trigger 노드를 본인 시트로 다시 선택
5. 각 노드의 자격증명(`PUT_YOUR_*`) 본인 키로 교체
6. Activate → 출력 검증 → 5개 과제 풀기

## ↔️ 다른 주차로 이동

[← W6 HybridRAG](https://github.com/keerhee/invest-ax-curriculum/tree/main/W6%20HybridRAG) · [→ W8 PaperTrading](https://github.com/keerhee/invest-ax-curriculum/tree/main/W8%20PaperTrading)

---

📚 [전체 커리큘럼 README](https://github.com/keerhee/invest-ax-curriculum/blob/main/README.md) · 🌐 [강의노트 홈](https://keerhee.github.io/invest-ax-curriculum/)
