# W4 — 차트 Vision + 3D Verdict

> 🌐 **강의노트**: <https://keerhee.github.io/invest-ax-curriculum/manuals/W4_chart_vision.html>
> 🏠 **전체 강의노트 홈**: <https://keerhee.github.io/invest-ax-curriculum/>
> 📦 **GitHub 레포**: <https://github.com/keerhee/invest-ax-curriculum>

**핵심 기술**: Chart-IMG · Claude Vision · 3D 통합 판단

## 📁 폴더 내 파일

| 파일 | 설명 |
|------|------|
| [`W4.json`](W4.json) | n8n 워크플로우 — Webhook → Chart-IMG + W2/W3 lookup → Vision → Verdict |
| [`W4_verdict.xlsx`](W4_verdict.xlsx) | verdict 시트 헤더 (8컬럼) |

## 🚦 사용 방법

1. [📖 W4 강의노트](https://keerhee.github.io/invest-ax-curriculum/manuals/W4_chart_vision.html)에서 흐름 이해
2. `W4.json` 을 n8n에 import (Workflows → Add → Import from file)
3. `W4_verdict.xlsx` 을 Google Drive에 업로드 → Google Sheets로 변환
4. n8n Sheets Trigger 노드를 본인 시트로 다시 선택
5. 각 노드의 자격증명(`PUT_YOUR_*`) 본인 키로 교체
6. Activate → 출력 검증 → 5개 과제 풀기

## ↔️ 다른 주차로 이동

[← W3 뉴스센티먼트](https://github.com/keerhee/invest-ax-curriculum/tree/main/W3%20%EB%89%B4%EC%8A%A4%EC%84%BC%ED%8B%B0%EB%A8%BC%ED%8A%B8) · [→ W5 스케줄링RAG](https://github.com/keerhee/invest-ax-curriculum/tree/main/W5%20%EC%8A%A4%EC%BC%80%EC%A4%84%EB%A7%81RAG)

---

📚 [전체 커리큘럼 README](https://github.com/keerhee/invest-ax-curriculum/blob/main/README.md) · 🌐 [강의노트 홈](https://keerhee.github.io/invest-ax-curriculum/)
