# StrataFlux: Memory-Hierarchy-Native Low-Bit LLM Inference

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-07
**링크**: http://arxiv.org/abs/2611.08363v1

## 💡 핵심 인사이트

저비트 양자화의 정확도 손실은 하드 천장이 아니라 메모리 계층 배치의 함수이며, 호스트 RAM·SSD에 고정밀 정제 원본을 계층화하면 양자화의 속도·메모리 이득을 유지한 채 정확도를 회복할 수 있다.

## 📖 분석

StrataFlux는 저비트 양자화의 정확도 손실을 메모리 계층 자체에서 회복하는 추론 프레임워크다. 양자화(메모리·속도 이득, 정확도 손실)와 고정밀 데이터 오프로딩(정확도 유지, 생성 정지)의 전통적 트레이드오프를 정제 표현·선택·전달의 공동 설계로 해소하여, 호스트 RAM과 SSD를 추론의 일급 자원으로 격상한다. 이는 [[on-demand-attention]]과 [[on-demand-frame-fetch]]가 확립한 '온디맨드 에스컬레이션' 패턴의 정밀도 차원 이식이다 — 저비트가 기본 계층이 되고 정확도에 결정적인 엔트리만 고정밀 원본을 인출한다. [[extreme-low-bit-quantization]] 계열이 저비트 형식 자체의 최적화를 다뤘다면 본 논문은 양자화 손실이 하드 천장이 아니라 계층 배치의 함수임을 보여 품질 문제를 '더 나은 저비트 형식'에서 '계층화된 정밀도 관리'로 이동시킨다. [[flash-dllm]]의 IO 인지 캐싱이 처리량을 위한 IO 은닉이었다면 StrataFlux는 IO가 정확도 회복의 통로가 되어 [[capability-forming-serving]]의 정밀도 버전을 제공하며, [[kv-cache-optimization]]의 대상도 압축·폐기에서 정밀도 티어링으로 확장된다. [[on-device-inference]] 관점에서도 메모리 제약 환경의 성능-효율 프론티어가 모델 크기에서 메모리 계층 설계로 이동함을 시사하며, 압축과 오프로딩이 경쟁 전략이 아닌 단일 메모리 계층 설계의 상보적 층위로 재정의되는 전환점이다.

## 🔗 관련 논문

- 2026 09 04 unfolding the leech lattice fused multi shell deco
- 2026 09 24 flash dllm io aware kv caching and parallel decodi
- 2026 11 03 latent sparse attention towards subquadratic ultra
- 2026 11 04 cisa retrofitting dense attention models with chun

## 🏷️ 엔티티

- [[entities/extreme-low-bit-quantization.md|extreme-low-bit-quantization]]
- [[entities/kv-cache-optimization.md|kv-cache-optimization]]
- [[entities/flash-dllm.md|flash-dllm]]
- [[entities/on-device-inference.md|on-device-inference]]
- [[entities/model-compression.md|model-compression]]
- [[entities/decode-phase-gemv-serving-cost.md|decode-phase-gemv-serving-cost]]
- [[entities/agent-native-serving.md|agent-native-serving]]
- [[entities/ultra-long-context-serving.md|ultra-long-context-serving]]

## 📐 개념

- [[concepts/memory-hierarchy-native-inference.md|memory-hierarchy-native-inference]]
- [[concepts/precision-escalation-on-demand.md|precision-escalation-on-demand]]
- [[concepts/quantization-offloading-tradeoff-dissolution.md|quantization-offloading-tradeoff-dissolution]]
- [[concepts/query-deferred-representation-contract.md|query-deferred-representation-contract]]
- [[concepts/local-sufficiency.md|local-sufficiency]]

---
_LLM 분석으로 생성됨_
