# kv-cache-optimization

**카테고리**: 미분류
**생성일**: 2026-04-25

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-04-25-tool-attention-is-all-you-need-dynamic-tool-gating.md|Tool Attention Is All You Need: Dynamic Tool Gating and Lazy]]

### Tool Attention Is All You Need: Dynamic Tool Gating and Lazy Schema Lo (2026-04-26)

MCP Tax가 KV 캐시를 직접 팽창시켜 서빙 비용을 기하급수적으로 증가시키는 메커니즘을 제공하며, 캐시 압축 기법과 상보적으로 작동하는 상류(upstream) 최적화로 Tool Attention을 위치시킨다.

### Learning to Communicate: Toward End-to-End Optimization of Multi-Agent (2026-04-26)

KV 캐시를 단일 모델 내부의 메모리 최적화 대상에서 에이전트 간 정보 전달 매체로 재해석하며, 기존 토큰 효율성 중심의 접근을 다중 에이전트 협력 효율성으로 확장하는 새로운 응용 경로를 제시한다.

### Pythia: Toward Predictability-Driven Agent-Native LLM Serving (2026-04-30)

에이전트 토폴로지의 예측가능한 호출 패턴을 활용해 KV 캐시의 프리페치나 재사용 전략을 구조화할 수 있어, 기존 캐시 압축 기법과 상보적으로 작동하는 상류 최적화 경로가 된다.

### Unifying Sparse Attention with Hierarchical Memory for Scalable Long-C (2026-05-01)

캐시 압축·프루닝 등 알고리즘 수준 최적화에서 계층적 메모리 아키텍처를 통한 구조적 해법으로 패러다임을 확장하며, 기존 기법들이 서로 다른 입도에서 동작하여 시스템 수준 이득으로 번역되지 못하는 원인을 최초로 형식화한다.

### Make Your LVLM KV Cache More Lightweight (2026-05-05)

KV 캐시 최적화의 대상을 텍스트 토큰에서 시각 토큰으로 확장한다. 기존에 스키마 축적·계층적 메모리 등 텍스트 중심 최적화에 머물던 이 엔티티에, 시각 임베딩의 구조적 중복성을 프리필 단계에서 제거하는 모달리티 인식 최적화 축을 추가한다.

### SpecKV: Adaptive Speculative Decoding with Compression-Aware Gamma Sel (2026-05-05)

KV 캐시 압축(LightKV 등)이 추측 디코딩의 γ 선택과 어떻게 상호작용하는지에 대한 구조적 질문을 제기한다. 압축 수준이 γ의 최적값을 변화시킨다면, KV 압축과 추측 디코딩은 독립적으로 최적화할 수 없는 결합 최적화 문제가 됨을 시사한다.
