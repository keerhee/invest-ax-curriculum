# W2 — 기술적 지표 계산

> 🌐 **강의노트**: <https://keerhee.github.io/invest-ax-curriculum/manuals/W2_technical_indicators.html>
> 🏠 **전체 강의노트 홈**: <https://keerhee.github.io/invest-ax-curriculum/>
> 📦 **GitHub 레포**: <https://github.com/keerhee/invest-ax-curriculum>

**핵심 기술**: RSI · MA · 볼린저 밴드 · MACD — 라이브러리 없이 수식 직접

## 📁 폴더 내 파일

| 파일 | 설명 |
|------|------|
| [`W2.json`](W2.json) | n8n 워크플로우 — Sheets read → Code(MA/RSI/BB/MACD) → Sheets append |
| [`W2_지표설정.xlsx`](W2_지표설정.xlsx) | 5개 지표 임계값 참조표 |

## 🚦 사용 방법

1. [📖 W2 강의노트](https://keerhee.github.io/invest-ax-curriculum/manuals/W2_technical_indicators.html)에서 흐름 이해
2. `W2.json` 을 n8n에 import (Workflows → Add → Import from file)
3. `W2_지표설정.xlsx` 을 Google Drive에 업로드 → Google Sheets로 변환
4. n8n Sheets Trigger 노드를 본인 시트로 다시 선택
5. 각 노드의 자격증명(`PUT_YOUR_*`) 본인 키로 교체
6. Activate → 출력 검증 → 5개 과제 풀기

## ↔️ 다른 주차로 이동

[← W1 데이터수집](https://github.com/keerhee/invest-ax-curriculum/tree/main/W1%20%EB%8D%B0%EC%9D%B4%ED%84%B0%EC%88%98%EC%A7%91) · [→ W3 뉴스센티먼트](https://github.com/keerhee/invest-ax-curriculum/tree/main/W3%20%EB%89%B4%EC%8A%A4%EC%84%BC%ED%8B%B0%EB%A8%BC%ED%8A%B8)

---

📚 [전체 커리큘럼 README](https://github.com/keerhee/invest-ax-curriculum/blob/main/README.md) · 🌐 [강의노트 홈](https://keerhee.github.io/invest-ax-curriculum/)
