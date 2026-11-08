# CISA: Retrofitting Dense Attention Models with Chunk-Indexed Sparse Attention

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-04
**링크**: http://arxiv.org/abs/2611.03200v1

## 💡 핵심 인사이트

KV 캐시의 기존 키에 이미 인덱스로 쓸 수 있는 요약 구조가 내재되어 있어, 별도 인덱스 캐시와 학습 없이도 dense 모델을 chunk 기반 sparse attention으로 개조할 수 있다.

## 📖 분석

# CISA: Chunk-Indexed Sparse Attention

사전학습된 dense attention 모델을 그래디언트 업데이트 없이 chunk 기반 sparse attention으로 개조하는 추론시점 방법. KV 캐시의 기존 키에 내재된 compact summary를 chunk 인덱스로 재사용해 토큰 수준 인덱싱과 별도 풀길이 인덱스 캐시를 모두 회피하고, KV 그룹당 하나의 인덱싱 쿼리로 선정된 chunk를 그룹 내 쿼리들이 공유(QShare)한다.

## Wiki 내 위치

[[concepts/kv-cache-optimization.md|kv cache optimization]] 논의에 '캐시 자체를 인덱스로 격상'이라는 상류 최적화를 추가한다. 계층 메모리나 트리 인덱서처럼 별도 인덱스 구조를 유지하던 희소화 계열과 달리, 기존 키 요약을 인덱스로 재사용해 인덱스 유지 비용을 구조적으로 제거함을 보여준다.

[[concepts/sparse-attention-unification.md|sparse attention unification]]에 학습 프리 경로를 제공한다. 기존 계열이 학습된 계층 메모리를 전제했다면, 본 논문은 dense 사전학습 모델의 개조 가능성을 보여 희소화의 적용 시점을 학습에서 추론으로 확장한다.

[[concepts/hierarchical-kv-memory.md|hierarchical kv memory]]의 캐시 입도 질문에 '고정 크기 chunk'라는 대안을 제시한다. 토큰 단위와 학습된 잠재 단위([[concepts/latent-projected-sparse-retrieval.md|latent projected sparse retrieval]])에 이어 세 번째 입도이며, chunk 선택이 기존 키 요약에 의해 이루어져 입도와 선택 기준이 분리됨을 보여준다.

[[concepts/indexer-quadratic-bottleneck.md|indexer quadratic bottleneck]]의 직접적 완화 경로다. [[concepts/subquadratic-attention.md|subquadratic attention]]의 트리 인덱서가 병목을 효율적 인덱스 구조로 완화했다면, 본 논문은 인덱서를 키의 내재 요약으로 대체해 병목 자체를 회피한다.

## 🔗 관련 논문

- Latent Sparse Attention: Towards Subquadratic Ultra-Long Context Attention
- Subquadratic Attention with a Hierarchical Tree-Structured Indexer
- Unifying Sparse Attention with Hierarchical Memory for Scalable Long-Context
- Flash-dLLM: IO-Aware KV Caching and Parallel Decoding

## 🏷️ 엔티티

- [[entities/kv-cache-optimization.md|kv-cache-optimization]]
- [[entities/sparse-attention-unification.md|sparse-attention-unification]]
- [[entities/hierarchical-kv-memory.md|hierarchical-kv-memory]]
- [[entities/indexer-quadratic-bottleneck.md|indexer-quadratic-bottleneck]]
- [[entities/subquadratic-attention.md|subquadratic-attention]]
- [[entities/cisa.md|cisa]]

## 📐 개념

- [[concepts/chunk-level-kv-selection.md|chunk-level-kv-selection]]
- [[concepts/index-cache-elimination.md|index-cache-elimination]]
- [[concepts/cross-query-chunk-sharing.md|cross-query-chunk-sharing]]
- [[concepts/training-free-attention-retrofit.md|training-free-attention-retrofit]]
- [[concepts/long-context.md|long-context]]
- [[concepts/ultra-long-context-serving.md|ultra-long-context-serving]]

---
_LLM 분석으로 생성됨_
