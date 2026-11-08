# Latent Sparse Attention: Towards Subquadratic Ultra-Long Context Attention

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-03
**링크**: http://arxiv.org/abs/2610.42147v1

## 💡 핵심 인사이트

희소 어텐션의 검색 단위를 토큰에서 학습된 잠재 상태로 이동시키면 subquadratic 확장과 정확도를 동시에 확보할 수 있으며, 이는 선택적 망각 원리가 인프라 계층을 넘어 어텐션 아키텍처 자체에 내재화되었음을 의미한다.

## 📖 분석

## 개요

Latent Sparse Attention(LSA)은 1M+ 토큰 규모의 초장기 컨텍스트에서 토큰 임베딩과 KV 캐시를 잠재 공간으로 투영한 뒤 잠재 상태 수준에서 희소 검색을 수행하는 subquadratic 어텐션 방법이다. 기존 희소 어텐션은 전체 컨텍스트 크기에 대한 인덱싱 비용이 여전히 2차이거나, 초장기 규모에서 정확도가 붕괴한다는 딜레마에 놓여 있었는데, LSA는 '검색의 대상'을 원시 KV 캐시에서 압축된 잠재 상태로 이동시켜 이 딜레마를 회피한다.

## 기존 Wiki와의 관계

이 논문은 [[concepts/sparse-attention-unification.md|sparse attention unification]]이 제시한 계층적 메모리 구조와 병렬되는 대안 축을 제공한다. Unifying Sparse Attention이 정적 계층 메모리로 희소성을 확보했다면, LSA는 잠재 투영이라는 학습 가능한 압축 계층을 희소 인덱서 앞에 추가한다. 또한 [[concepts/hierarchical-kv-memory.md|hierarchical kv memory]]의 KV 캐시 구조화 논의에 '잠재 상태 단위 캐시 조직화'라는 새로운 설계 공간을 추가한다.

주목할 점은 이 방법이 agentic workflow의 장기 태스크를 명시적 동기로 삼는다는 것이다. [[concepts/agent-native-serving.md|agent native serving]]의 관점에서, 에이전트 실행이 스키마 축적과 다단계 상호작용으로 KV 캐시를 폭발시키는 구조적 문제([[concepts/schema-accumulation-bottleneck.md|schema accumulation bottleneck]], [[concepts/long-context.md|long context]])에 대해 모델 아키텍처 층의 직접적 해법을 제시한다. 세션 전체 궤적을 컨텍스트로 유지해야 하는 에이전트에게 [[concepts/kv-cache-optimization.md|kv cache optimization]]의 캐시 관리를 넘어서는 '캐시 구조 자체의 재설계'에 해당한다.

## 인사이트

희소 어텐션의 선택 단위가 토큰에서 잠재 상태로 이동하면, [[concepts/compression-forgetting-isomorphism.md|compression forgetting isomorphism]]이 예고한 '압축=선택적 망각' 원리가 어텐션 아키텍처 내부로 내재화된다. 인덱서가 어떤 잠재 상태를 검색할지 결정하는 것은 곧 어떤 과거 맥락이 현재 추론에 '존재'할지를 결정하는 것이므로, 장기 에이전트 실행에서 LSA의 인덱서는 사실상 런타임 메모리 관리자의 역할을 수행하게 된다. 이는 [[concepts/algorithm-system-translation-gap.md|algorithm system translation gap]]의 관점에서 주목할 지점이다 — 망각·선택 판단이 인프라 계층(서빙·캐시 정책)이 아닌 모델 가중치 내부(학습된 인덱서)로 이동한 사례다.

## 🏷️ 엔티티

- [[entities/sparse-attention-unification.md|sparse-attention-unification]]
- [[entities/hierarchical-kv-memory.md|hierarchical-kv-memory]]
- [[entities/long-context.md|long-context]]
- [[entities/agent-native-serving.md|agent-native-serving]]
- [[entities/kv-cache-optimization.md|kv-cache-optimization]]
- [[entities/algorithm-system-translation-gap.md|algorithm-system-translation-gap]]

## 📐 개념

- [[concepts/latent-projected-sparse-retrieval.md|latent-projected-sparse-retrieval]]
- [[concepts/subquadratic-attention.md|subquadratic-attention]]
- [[concepts/potential-memory-state-indexing.md|potential-memory-state-indexing]]
- [[concepts/ultra-long-context-serving.md|ultra-long-context-serving]]

---
_LLM 분석으로 생성됨_
