# Reward-Based Online LLM Routing via NeuralUCB

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-04-02  
**링크**: None

## 핵심 요약

이 논문은 여러 LLM 중 어떤 모델에 쿼리를 보낼지 실시간으로 결정하는 **비용 인식 LLM 라우팅** 문제를 다룬다. 기존 지도학습 기반 라우팅과 부분 피드백 방식의 한계를 극복하기 위해 **NeuralUCB**(신경망 + Upper Confidence Bound) 알고리즘을 라우팅 정책에 적용했다. RouterBench 벤치마크에서 온라인 시뮬레이션 실험을 수행한 결과, 제안 방법은 랜덤·최소비용 베이스라인 대비 유틸리티 보상에서 일관되게 우수했으며, 최대품질 베이스라인 대비 추론 비용을 크게 절감하면서도 경쟁력 있는 품질을 유지했다. 다만 액션 변별력과 탐색 전략에는 개선 과제가 남아 있다.

## 인사이트

1. **탐색-활용 균형이 핵심**: NeuralUCB의 UCB 기반 탐색 전략이 온라인 환경에서 미지의 LLM 조합을 효과적으로 시도하면서도 품질을 유지할 수 있게 한다.
2. **비용-품질 트레이드오프 최적화**: 항상 최고 품질 모델을 쓰는 것이 아니라, 쿼리 특성에 맞는 모델을 선택함으로써 비용을 대폭 줄이면서도 유사한 성능을 달성할 수 있다.
3. **부분 피드백 환경의 현실성**: 실제 서비스에서는 선택한 모델의 결과만 관측 가능하므로, 전체 레이블이 필요한 지도학습보다 부분 피드백(밴딧) 프레임워크가 더 실용적이다.

## 응용 가능성

1. **LLM API 게이트웨이**: GPT-4, Claude, Gemini 등 다수의 LLM API를 운영하는 서비스에서 쿼리 난이도에 따라 자동으로 최적 모델을 선택해 비용을 절감하는 지능형 라우터로 활용할 수 있다.
2. **엣지-클라우드 하이브리드 추론**: 간단한 쿼리는 경량 로컬 모델로, 복잡한 쿼리는 클라우드 대형 모델로 동적 분배하는 온디바이스 라우팅 시스템에 적용할 수 있다.

## 추출된 엔티티

- Claude 3.5
- GPT-4

## 추출된 개념

_없음_

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-04-02-Reward-BasedOnlineLLMRoutingvi.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-03-27-claudini-autoresearch-discovers-state-of-the-art-a.md]] (공통 Entity: Claude 3.5)
- [[sources/2026-03-26-reqfusion-a-multi-provider-framework-for-automated.md]] (공통 Entity: Claude 3.5)
- [[sources/2026-03-27-march-multi-agent-reinforced-self-check-for-llm-ha.md]] (공통 Entity: GPT-4)
- [[sources/2026-03-26-code-review-agent-benchmark.md]] (공통 Entity: Claude 3.5)
- [[sources/2026-04-03-textttyc-bench-benchmarking-ai-agents-for-long-ter.md]] (공통 Entity: Claude 3.5)
