# ShallowStream: Index Shallow then Answer Deep for Streaming Video Understanding

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-04
**링크**: http://arxiv.org/abs/2609.02780v1

## 💡 핵심 인사이트

질의 도착 전까지는 어떤 정보가 관련성 있는지 알 수 없으므로, 스트리밍 이해의 핵심은 질의 무관적으로 확장 가능한 '얕은 인덱스'를 유지하다가 질의 시점에만 깊은 계산을 발동하는 이단계 분리다.

## 📖 분석

# ShallowStream: 징-얕은 인덱싱과 깊은 답변의 이단계 분리

ShallowStream은 연속 비디오 스트림의 MLLM 처리 비용 문제를 "Index Shallow then Answer Deep"이라는 이단계 추론 패러다임으로 해결한다. 기존 접근(토큰 프루닝, 병합, 양자화, 온디맨드 프레임 검색, 컨텍스트 오프로딩)이 연속 스트림의 국소적 비용을 줄이는 최적화에 머물렀다면, 본 논문은 **질의 도착 전 계산과 질의 도착 후 계산을 구조적으로 분리**한다. 질의가 없는 구간에서는 가벼운 얕은 처리로 과거 프레임의 인덱스만 유지하고, 질의 도착 시점에만 깊은 처리를 발동해 답변을 생성한다.

이는 [[streaming-adaptive-inference]]의 가장 구체적 구현이다. [[adaptive-inference]] 관점에서 적응 트리거의 새 유형을 추가한다 — 외부 환경 반응(CADENCE), 내부 시스템 상태 반응(SpecKV)과 달리, '질의 도착'이라는 사용자 이벤트가 계산 깊이 자체를 결정한다.

핵심은 **미래 질의 불확실성**이다. 질의 도착 전에는 어떤 정보가 관련성 있을지 알 수 없는 상태에서 압축·인덱싱이 수행되어야 하므로, 인덱스는 "임의 질의에 대해 후속 깊은 처리로 확장 가능한" 질의 무관적 보존 단위로 설계되어야 한다. 이는 [[compression-relevance-isomorphism]]의 역문제이며, [[non-selective-context-accumulation]]의 대척점에 있는 선택적 유보 전략이다.

또한 [[autoregressive-paradigm-confinement]]를 완화한다 — 모든 입력을 순차 풀 처리하는 자기회귀 전제 대신 질의 조건부 지연 실행으로 스트리밍을 재구성한다. 체화 지능·자율주행·감시 등 상시 스트림 응용([[embodied-ai]], [[agentic-vlm]])에서 질의 도착 전 계산 예산을 절감하면서 답변 품질을 유지하는 실용적 경로를 제공한다. SpecKV(압축 상태 반응형 적응), Make Your LVLM KV Cache More Lightweight(시각 토큰 KV 압축), LongSeeker(탄력적 컨텍스트 조율)와 함께 스트리밍 효율화의 축을 형성한다.

## 🔗 관련 논문

- SpecKV: Adaptive Speculative Decoding with Compression-Aware
- Make Your LVLM KV Cache More Lightweight
- LongSeeker: Elastic Context Orchestration for Long-Horizon S
- Turning the TIDE: Cross-Architecture Distillation for Diffus

## 🏷️ 엔티티

- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/kv-cache-optimization.md|kv-cache-optimization]]
- [[entities/token-pruning.md|token-pruning]]
- [[entities/speculative-decoding.md|speculative-decoding]]
- [[entities/long-context.md|long-context]]
- [[entities/agentic-vlm.md|agentic-vlm]]
- [[entities/video-understanding.md|video-understanding]]
- [[entities/lightkv.md|lightkv]]

## 📐 개념

- [[concepts/streaming-adaptive-inference.md|streaming-adaptive-inference]]
- [[concepts/autoregressive-paradigm-confinement.md|autoregressive-paradigm-confinement]]
- [[concepts/compression-relevance-isomorphism.md|compression-relevance-isomorphism]]
- [[concepts/non-selective-context-accumulation.md|non-selective-context-accumulation]]
- [[concepts/modality-asymmetric-memory-cost.md|modality-asymmetric-memory-cost]]
- [[concepts/text-guided-vision-token-selection.md|text-guided-vision-token-selection]]
- [[concepts/perception-cognitive-capacity-mismatch.md|perception-cognitive-capacity-mismatch]]
- [[concepts/shallow-index-deep-answer.md|shallow-index-deep-answer]]
- [[concepts/future-query-agnostic-compression.md|future-query-agnostic-compression]]

---
_LLM 분석으로 생성됨_
