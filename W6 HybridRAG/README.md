# W6 — Hybrid RAG 실전

> 🌐 **강의노트**: <https://keerhee.github.io/invest-ax-curriculum/manuals/W6_hybrid_rag.html>
> 🏠 **전체 강의노트 홈**: <https://keerhee.github.io/invest-ax-curriculum/>
> 📦 **GitHub 레포**: <https://github.com/keerhee/invest-ax-curriculum>

**핵심 기술**: PDF 임베딩 · BM25+Vector · Cohere Rerank · 출처 인용

## 📁 폴더 내 파일

| 파일 | 설명 |
|------|------|
| [`W6.json`](W6.json) | n8n 워크플로우 본편 — Supabase Vector + BM25 → Cohere Rerank → Claude |
| [`W6_PDF목록.xlsx`](W6_PDF목록.xlsx) | 임베딩할 사업보고서/공시 PDF 메타데이터 시트 |
| 💎 [`W6_BONUS_qdrant_hybrid.json`](W6_BONUS_qdrant_hybrid.json) | **보너스** — Qdrant native hybrid (Dense + BM25 + RRF) 1-call |
| 💎 [`W6_BONUS_샘플질의.xlsx`](W6_BONUS_샘플질의.xlsx) | **보너스** — 8개 금융 질의로 Dense / BM25 / Hybrid 비교 실험 |

## 🚦 사용 방법

1. [📖 W6 강의노트](https://keerhee.github.io/invest-ax-curriculum/manuals/W6_hybrid_rag.html)에서 흐름 이해 (본편 + 💎 보너스 섹션)
2. `W6.json` 을 n8n에 import (Workflows → Add → Import from file)
3. `W6_PDF목록.xlsx` 을 Google Drive에 업로드 → Google Sheets로 변환
4. n8n Sheets Trigger 노드를 본인 시트로 다시 선택
5. 각 노드의 자격증명(`PUT_YOUR_*`) 본인 키로 교체
6. Activate → 출력 검증 → 5개 과제 풀기

## 💎 보너스 — Qdrant Native Hybrid (참조 영상 기반)

본편의 Supabase pgvector + ts_rank 흐름을 **Qdrant 1.10+ native hybrid**로 옮긴 응용 실습.
사업보고서·공시·IR 자료에 대해 한 번의 API 호출로 Dense + BM25 + RRF fusion 결과를 받습니다.

**참조 영상**:
- [Hybrid Search in Legal AI with Qdrant & n8n](https://www.youtube.com/watch?v=7LEhwjETnu4) (Qdrant 공식, **주참조**)
- [Qdrant Hybrid Search Tutorial](https://youtu.be/QuDGpV9Nhzc) (BlogYourCode)
- [How to Set Up and Use Qdrant for Hybrid Search](https://youtu.be/pssHxg8GDFc) (Chirag Patil)

**보너스 흐름**:
1. `W6_BONUS_qdrant_hybrid.json` 을 n8n에 import
2. Qdrant Cloud에 컬렉션 생성 (named vectors: dense 1536d + sparse idf)
3. FastEmbed BM25 sparse 모델 띄우기 (`docker run qdrant/fastembed-server` 또는 Python)
4. 사업보고서 PDF 3종 임베딩 (Dense + Sparse 동시 upsert)
5. `W6_BONUS_샘플질의.xlsx` 의 8개 질의로 Dense / BM25 / Hybrid 모드 비교
6. 본인 채점으로 fusion=rrf vs fusion=dbsf 효과 측정

## ↔️ 다른 주차로 이동

[← W5 스케줄링RAG](https://github.com/keerhee/invest-ax-curriculum/tree/main/W5%20%EC%8A%A4%EC%BC%80%EC%A4%84%EB%A7%81RAG) · [→ W7 멀티에이전트](https://github.com/keerhee/invest-ax-curriculum/tree/main/W7%20%EB%A9%80%ED%8B%B0%EC%97%90%EC%9D%B4%EC%A0%84%ED%8A%B8)

---

📚 [전체 커리큘럼 README](https://github.com/keerhee/invest-ax-curriculum/blob/main/README.md) · 🌐 [강의노트 홈](https://keerhee.github.io/invest-ax-curriculum/)
