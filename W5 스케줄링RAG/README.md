# W5 — 스케줄링 + Vector DB 기초

> 🌐 **강의노트**: <https://keerhee.github.io/invest-ax-curriculum/manuals/W5_scheduling_rag.html>
> 🏠 **전체 강의노트 홈**: <https://keerhee.github.io/invest-ax-curriculum/>
> 📦 **GitHub 레포**: <https://github.com/keerhee/invest-ax-curriculum>

**핵심 기술**: Supabase pgvector · 첫 RAG · 멀티 Cron

## 📁 폴더 내 파일

| 파일 | 설명 |
|------|------|
| [`W5.json`](W5.json) | n8n 워크플로우 — 4× Cron + Webhook(/embed,/ask) → OpenAI + Supabase |
| [`W5_스케줄.xlsx`](W5_스케줄.xlsx) | 장 시간대별 4개 스케줄 정의 |

## 🚦 사용 방법

1. [📖 W5 강의노트](https://keerhee.github.io/invest-ax-curriculum/manuals/W5_scheduling_rag.html)에서 흐름 이해
2. `W5.json` 을 n8n에 import (Workflows → Add → Import from file)
3. `W5_스케줄.xlsx` 을 Google Drive에 업로드 → Google Sheets로 변환
4. n8n Sheets Trigger 노드를 본인 시트로 다시 선택
5. 각 노드의 자격증명(`PUT_YOUR_*`) 본인 키로 교체
6. Activate → 출력 검증 → 5개 과제 풀기

## ↔️ 다른 주차로 이동

[← W4 차트Vision](https://github.com/keerhee/invest-ax-curriculum/tree/main/W4%20%EC%B0%A8%ED%8A%B8Vision) · [→ W6 HybridRAG](https://github.com/keerhee/invest-ax-curriculum/tree/main/W6%20HybridRAG)

---

📚 [전체 커리큘럼 README](https://github.com/keerhee/invest-ax-curriculum/blob/main/README.md) · 🌐 [강의노트 홈](https://keerhee.github.io/invest-ax-curriculum/)
