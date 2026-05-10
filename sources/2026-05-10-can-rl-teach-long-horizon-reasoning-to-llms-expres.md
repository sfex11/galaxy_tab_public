# Can RL Teach Long-Horizon Reasoning to LLMs? Expressiveness Is Key

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-10
**링크**: http://arxiv.org/abs/2605.06638v1

## 💡 핵심 인사이트

RL이 LLM에 장기 추론을 가르칠 수 있는지의 여부는 탐색 깊이가 아니라 기저 논리의 표현력에 의해 결정되며, 표현력 임계 미달 상태에서의 RL 학습은 경로 제공이 아닌 표현력 내 최적화로 수렴한다.

## 📖 분석

# ScaleLogic: RL 기반 장기 추론의 표현력 병목

## 정의
ScaleLogic은 논리적 추론에서 난이도의 두 축—증명 계획의 깊이(horizon)와 기저 논리의 표현력(expressiveness)—을 독립적으로 제어 가능한 합성 프레임워크로, RL이 LLM의 장기 추론을 가르칠 수 있는지를 체계적으로 조사한다.

## 기존 Wiki와의 관계

기존 `exploration-absorption-decoupling`이 RL의 기여를 '경로 제공'으로 재정의했다면, 본 논문은 그 경로의 **흡수 가능성**이 기저 논리의 표현력에 의해 결정됨을 실증한다. 즉, RL이 아무리 긴 탐색 경로를 제공해도 표현력이 부족한 논리 체계에서는 경로가 능력으로 전환되지 않는다.

`non-linear-task-scaling`이 Design Conductor 2.0에서 비선형 태스크 스케일링을 문제화했다면, 본 논문은 이를 RL 학습 곡선에서 **두 축의 독립적 비선형성**으로 구체화한다: 깊이에 대한 스케일링과 표현력에 대한 스케일링이 서로 다른 임계점을 가지며, 표현력 임계가 깊이 임계보다 먼저 도달한다.

## 핵심 발견

표현력이 병목이라는 발견은 `marginal-distribution-ceiling`과 깊이 연결된다: 사전학습 분포 P(y)가 특정 논리 체계의 표현력에 의해 형성되며, RL이 P(y|x)를 최적화하더라도 P(y)의 표현력 한계를 넘어서는 추론은 구조적으로 불가능하다. 이는 RL 기반 사후학습의 근본적 한계를 **학습 알고리즘이 아닌 표현 체계**에서 찾는 새로운 문제화이다.

`exploration-hacking`과의 관계에서 흥미로운 대조가 emerges: 탐색 해킹이 모델이 '쉬운 경로만 찾는' 문제라면, 본 논문은 반대로 모델이 '표현력 한계 내에서는 올바르게 학습하지만 그 한계 자체가 보이지 않는' 문제를 보여준다. 두 현상은 공통적으로 RL 학습의 실제 효과를 과대평가하게 만든다.

## 🔗 관련 논문

- 2026 05 09 can rl teach long horizon reasoning to llms expressive
- 2026 05 02 exploration hacking can llms learn to resist rl tr
- 2026 05 08 design conductor 20 an agent builds a turboquant i
- 2026 05 01 select to think unlocking slm potential with local

## 🏷️ 엔티티

- [[entities/reinforcement-learning.md|reinforcement-learning]]
- [[entities/non-linear-task-scaling.md|non-linear-task-scaling]]
- [[entities/scalelogic.md|scalelogic]]
- [[entities/logic-expressiveness.md|logic-expressiveness]]
- [[entities/proof-planning-depth.md|proof-planning-depth]]
- [[entities/marginal-distribution-ceiling.md|marginal-distribution-ceiling]]
- [[entities/exploration-absorption-decoupling.md|exploration-absorption-decoupling]]
- [[entities/ceiling-performance-problem.md|ceiling-performance-problem]]

## 📐 개념

- [[concepts/logic-expressiveness-bottleneck.md|logic-expressiveness-bottleneck]]
- [[concepts/dual-axis-difficulty-control.md|dual-axis-difficulty-control]]
- [[concepts/proof-planning-horizon.md|proof-planning-horizon]]
- [[concepts/rl-reasoning-transfer-boundary.md|rl-reasoning-transfer-boundary]]
- [[concepts/expressiveness-conditioned-absorption.md|expressiveness-conditioned-absorption]]

---
_LLM 분석으로 생성됨_
