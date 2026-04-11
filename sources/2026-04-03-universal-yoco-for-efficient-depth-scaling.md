# Universal YOCO for Efficient Depth Scaling

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-03
**링크**: http://arxiv.org/abs/2604.01220v1

## 💡 핵심 인사이트

YOCO의 단일 KV 캐시 저장과 재귀적 깊이 확장을 결합하면, 테스트 타임에 모델 깊이를 유연하게 스케일링하면서도 메모리 오버헤드를 억제할 수 있어, 두 기법의 시너지가 개별 적용을 초과하는 효율성을 달성한다.

## 📖 분석

## Universal YOCO for Efficient Depth Scaling

**Universal YOCO (YOCO-U)**는 YOCO(You Only Cache Once) 디코더-디코더 아키텍처와 재귀적 연산(recursive computation)을 결합하여 LLM의 깊이 스케일링을 효율적으로 수행하는 방법을 제안한다. 테스트 타임 스케일링(test-time scaling)이 LLM의 추론 및 에이전틱 능력을 크게 향상시키고 있지만, 기존 Transformer는 루핑 전략의 높은 연산 오버헤드와 모델 깊이에 비례하여 증가하는 KV 캐시 문제로 인해 추론 시 컴퓨트 스케일링이 비효율적이다.

YOCO-U는 두 가지 핵심 문제를 동시에 해결한다: (1) YOCO 구조를 통해 KV 캐시를 한 번만 저장하여 메모리 사용량을 대폭 줄이고, (2) 재귀적 연산으로 동일한 파라미터 블록을 반복 적용하여 깊이를 유연하게 확장할 수 있다. 이 시너지 효과는 개별 기법 단독 적용보다 더 큰 성능 향상을 가져온다.

이 연구는 기존 Wiki의 [[Transformer]] 엔티티와 직접적으로 관련되며, 특히 추론 효율성 측면에서 **speculative-decoding**, **multi-token-prediction** 등 추론 가속화 개념들과 상호보완적이다. KV 캐시 최적화는 **token-pruning** 개념과도 맥을 같이하며, 테스트 타임 컴퓨트 스케일링은 **scaling-laws** 개념의 새로운 축(깊이 방향 스케일링)을 제시한다. 또한 on-device-inference 관점에서 메모리 효율적 아키텍처로서의 실용적 가치가 크다.

## 🔗 관련 논문

- Efficient Training-Free Multi-Token Prediction via Embedding
- What do Language Models Learn and When? The Implicit Curricu
- Nemotron-Cascade 2: Post-Training LLMs with Cascade RL and M
- Sustainability Is Not Linear: Quantifying Performance, Energ
- Unified Spatio-Temporal Token Scoring for Efficient Video VL

## 🏷️ 엔티티

- [[entities/transformer.md|transformer]]

## 📐 개념

- [[concepts/speculative-decoding.md|speculative-decoding]]
- [[concepts/scaling-laws.md|scaling-laws]]
- [[concepts/token-pruning.md|token-pruning]]
- [[concepts/on-device-inference.md|on-device-inference]]
- [[concepts/kv-cache-optimization.md|kv-cache-optimization]]
- [[concepts/recursive-computation.md|recursive-computation]]
- [[concepts/depth-scaling.md|depth-scaling]]

---
_LLM 분석으로 재생성됨_
