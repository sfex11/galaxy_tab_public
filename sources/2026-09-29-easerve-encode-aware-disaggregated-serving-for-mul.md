# EAServe: Encode-Aware Disaggregated Serving for Multimodal Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-29
**링크**: http://arxiv.org/abs/2609.31551v1

## 💡 핵심 인사이트

멀티모달 서빙에서 Encode가 제3의 독립 위상으로 격상되면서, 서빙 최적화의 단위가 모델 전체에서 위상별 이질적 자원 풀로 세분화된다.

## 📖 분석

본 논문은 MLLM 서빙에 3단계 분리(Encode-Prefill-Decode, EPD)를 제안한다. 텍스트 LLM에서 Prefill-Decode 분리가 표준이 된 반면, 멀티모달은 이미지·비디오·오디오를 임베딩으로 변환하는 Encode라는 제3의 위상을 추가하며, 세 위상의 연산 특성이 이질적이므로 단일 GPU 풀 할당은 자원 낭비를 낳는다.

Wiki 관점에서 두 축이 교차한다. 첫째, Pythia([[agent-native-serving]])와 Flash-dLLM([[flash-dllm]]) 계열의 서빙 최적화 논의에 '위상 수준 자원 분리'라는 새 축을 제공한다. [[decode-phase-gemv-serving-cost]]가 디코드 위상의 비용 특성을 다뤘다면 본 논문은 이를 3위상 이질성 구조로 일반화한다. 둘째, [[modality-asymmetric-memory-cost]]가 문서화한 모달리티 비대칭이 서빙 인프라 계층에서 실체화되는 지점이다. Encode 위상의 독립 자원 풀 요구는 시각 모달리티의 처리 비용이 텍스트와 구조적으로 다름을 인프라 설계가 인정했음을 의미하며, [[multimodal-llm]]·[[video-inference-efficiency]] 논의에 인프라 차원의 근거를 부여한다. 또한 [[aggregate-pipeline-serving]]이 스키마 축적이라는 단계 간 인터페이스 병목을 다뤘다면, 본 논문은 위상 간 연산 특성 차이라는 또 다른 파이프라인 구조 문제를 해결하여, 서빙 스택의 내부 구조가 점진적으로 세분화되는 흐름을 확정한다.

## 🔗 관련 논문

- Pythia: Toward Predictability-Driven Agent-Native LLM Servin
- Flash-dLLM: IO-Aware KV Caching and Parallel Decoding for Fa
- Why Is Video Still So Expensive? A Survey of Inference-Effic
- Caption-once, Frames-on-Demand: Visual-Need Routing for Budget-Aware A

## 🏷️ 엔티티

- [[entities/agent-native-serving.md|agent-native-serving]]
- [[entities/modality-asymmetric-memory-cost.md|modality-asymmetric-memory-cost]]
- [[entities/decode-phase-gemv-serving-cost.md|decode-phase-gemv-serving-cost]]
- [[entities/aggregate-pipeline-serving.md|aggregate-pipeline-serving]]
- [[entities/multimodal-llm.md|multimodal-llm]]
- [[entities/video-inference-efficiency.md|video-inference-efficiency]]
- [[entities/flash-dllm.md|flash-dllm]]
- [[entities/easerve.md|easerve]]

## 📐 개념

- [[concepts/encode-prefill-decode-disaggregation.md|encode-prefill-decode-disaggregation]]
- [[concepts/phase-heterogeneous-resource-allocation.md|phase-heterogeneous-resource-allocation]]
- [[concepts/modality-asymmetric-memory-cost.md|modality-asymmetric-memory-cost]]
- [[concepts/multimodal-llm.md|multimodal-llm]]

---
_LLM 분석으로 생성됨_
