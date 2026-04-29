# W1 — 데이터 수집 자동화

> 🌐 **강의노트**: <https://keerhee.github.io/invest-ax-curriculum/manuals/W1_data_collection.html>
> 🏠 **전체 강의노트 홈**: <https://keerhee.github.io/invest-ax-curriculum/>
> 📦 **GitHub 레포**: <https://github.com/keerhee/invest-ax-curriculum>

**핵심 기술**: CoinGecko · Yahoo Finance · FRED · Google Sheets

## 📁 폴더 내 파일

| 파일 | 설명 |
|------|------|
| [`W1.json`](W1.json) | n8n 워크플로우 — Cron → Yahoo+CoinGecko+FRED → Sheets append |
| [`W1_종목마스터.xlsx`](W1_종목마스터.xlsx) | 관심종목 9건 샘플 (한국·미국·암호화폐·매크로) |

## 🚦 사용 방법

1. [📖 W1 강의노트](https://keerhee.github.io/invest-ax-curriculum/manuals/W1_data_collection.html)에서 흐름 이해
2. `W1.json` 을 n8n에 import (Workflows → Add → Import from file)
3. `W1_종목마스터.xlsx` 을 Google Drive에 업로드 → Google Sheets로 변환
4. n8n Sheets Trigger 노드를 본인 시트로 다시 선택
5. 각 노드의 자격증명(`PUT_YOUR_*`) 본인 키로 교체
6. Activate → 출력 검증 → 5개 과제 풀기

## ↔️ 다른 주차로 이동

[→ W2 기술적지표](https://github.com/keerhee/invest-ax-curriculum/tree/main/W2%20%EA%B8%B0%EC%88%A0%EC%A0%81%EC%A7%80%ED%91%9C)

---

📚 [전체 커리큘럼 README](https://github.com/keerhee/invest-ax-curriculum/blob/main/README.md) · 🌐 [강의노트 홈](https://keerhee.github.io/invest-ax-curriculum/)
