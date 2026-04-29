# SP — 한국투자증권 모의투자

> 🌐 **강의노트**: <https://keerhee.github.io/invest-ax-curriculum/manuals/SP_kis_korea.html>
> 🏠 **전체 강의노트 홈**: <https://keerhee.github.io/invest-ax-curriculum/>
> 📦 **GitHub 레포**: <https://github.com/keerhee/invest-ax-curriculum>

**핵심 기술**: OAuth · HashKey · 한국 호가단위

## 📁 폴더 내 파일

| 파일 | 설명 |
|------|------|
| [`SP.json`](SP.json) | n8n 워크플로우 — Webhook → Token → 호가snap → HashKey → Order |
| [`SP_KIS주문이력.xlsx`](SP_KIS주문이력.xlsx) | KIS 주문이력 시트 (10컬럼) |

## 🚦 사용 방법

1. [📖 SP 강의노트](https://keerhee.github.io/invest-ax-curriculum/manuals/SP_kis_korea.html)에서 흐름 이해
2. `SP.json` 을 n8n에 import (Workflows → Add → Import from file)
3. `SP_KIS주문이력.xlsx` 을 Google Drive에 업로드 → Google Sheets로 변환
4. n8n Sheets Trigger 노드를 본인 시트로 다시 선택
5. 각 노드의 자격증명(`PUT_YOUR_*`) 본인 키로 교체
6. Activate → 출력 검증 → 5개 과제 풀기

## ↔️ 다른 주차로 이동

[← W8 PaperTrading](https://github.com/keerhee/invest-ax-curriculum/tree/main/W8%20PaperTrading)

---

📚 [전체 커리큘럼 README](https://github.com/keerhee/invest-ax-curriculum/blob/main/README.md) · 🌐 [강의노트 홈](https://keerhee.github.io/invest-ax-curriculum/)
