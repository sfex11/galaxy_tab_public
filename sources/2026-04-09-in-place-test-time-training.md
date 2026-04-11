# In-Place Test-Time Training

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-09
**링크**: http://arxiv.org/abs/2604.06169v1

## 💡 핵심 인사이트

기존 Transformer 아키텍처를 변경하지 않고 추론 시점에 파라미터를 동적 갱신하는 In-Place TTT는 LLM의 정적 배포 패러다임을 근본적으로 전환하여 연속적 정보 적응을 가능하게 한다.

## 📖 분석

## In-Place Test-Time Training

기존 LLM의 "학습 후 배포(train then deploy)" 패러다임의 한계를 극복하기 위한 새로운 접근법을 제안한다. Test-Time Training(TTT)은 추론 시점에 모델 파라미터의 일부(fast weights)를 업데이트하여 실시간으로 새로운 정보에 적응할 수 있게 하지만, 기존 LLM 생태계에서는 아키텍처 비호환성, 계산 비효율성 등의 장벽이 존재했다.

In-Place TTT는 이러한 문제를 해결하기 위해 기존 Transformer 아키텍처 내에서 직접(in-place) TTT를 수행하는 방식을 제안한다. 별도의 아키텍처 변경 없이 모델의 일부 파라미터를 추론 시점에 동적으로 갱신함으로써, 연속적인 정보 스트림에 대한 적응력을 확보한다.

이 연구는 test-time scaling 연구([[sources/2026-04-03-reasoning-shift-how-context-silently-shortens-llm-.md|Reasoning Shift]])와 밀접한 관련이 있으며, 추론 시점에 추가 연산을 투입하여 성능을 높이는 패러다임을 공유한다. 또한 KV-cache 최적화([[sources/2026-04-03-universal-yoco-for-efficient-depth-scaling.md|Universal YOCO]])와도 연결되는데, TTT의 fast weights가 KV-cache의 역할을 대체하거나 보완할 수 있기 때문이다. on-device inference 효율성 관점에서도 중요한 시사점을 제공하며, continual learning 및 non-stationary dynamics 문제에 대한 LLM 수준의 해법으로 볼 수 있다.

특히 LLM의 long-context 처리 능력과도 연결되며, 고정된 context window를 넘어 동적으로 지식을 흡수하는 메커니즘으로서의 의미가 크다.

## 🔗 관련 논문

- 2026 04 03 reasoning shift how context silently shortens llm 
- 2026 04 03 universal yoco for efficient depth scaling
- 2026 04 11 what do language models learn and when the implici
- 2026 04 11 cram less to fit more training data pruning improv

## 🏷️ 엔티티

- [[entities/llm.md|llm]]
- [[entities/transformer.md|transformer]]

## 📐 개념

- [[concepts/test-time-scaling.md|test-time-scaling]]
- [[concepts/kv-cache-optimization.md|kv-cache-optimization]]
- [[concepts/on-device-inference.md|on-device-inference]]
- [[concepts/continual-learning.md|continual-learning]]
- [[concepts/non-stationary-dynamics.md|non-stationary-dynamics]]
- [[concepts/long-context.md|long-context]]
- [[concepts/test-time-training.md|test-time-training]]

---
_LLM 분석으로 재생성됨_
