# Not All Reasoning Generalizes: A Case Study on Learning Generalizable Reasoning Strategies in RLVR

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-04
**링크**: http://arxiv.org/abs/2611.03627v1

## 💡 핵심 인사이트

RLVR로 획득한 추론 능력의 일반화 여부는 전략 수준에서 결정되며, 일반화 가능한 추론 전략을 관측·선별·유도하는 것이 RL 훈련 설계의 핵심 변수다.

## 📖 분석

RLVR의 일반화 가능성을 '추론 전략' 수준에서 분해하는 통제 실험 연구다. f(x)=y 형태의 비단사 문자열 함수 방정식 풀이 프레임워크를 설계하여, 여러 유효 해가 공존하는 조건에서 모델이 채택하는 추론 전략을 외부에서 관측 가능하게 만들고, easy-to-hard OOD 일반화의 명확한 조작적 정의를 제공한다.

핵심 발견은 RLVR로 획득한 추론이 모두 일반화되는 것이 아니라, 일반화 여부가 학습된 추론 전략의 종류에 의해 결정된다는 점이다. [[rl-reasoning-transfer-boundary]]가 표현력 관점에서 RL이 가르칠 수 있는 추론의 경계를 그렸다면, 본 논문은 전략 관점에서 '경계 내부의 무엇이 일반화되는가'를 분리 측정하는 미시 축을 연다.

[[generalization-gap]] 논의에 '전략 수준 귀속' 차원을 추가한다 — 일반화 실패가 단일 현상이 아니라 어떤 전략을 학습시켰는가의 함수임을 통제 조건 하에서 실증한다. [[search-policy-learning]]과의 접점에서, 탐색 정책 학습이 일반화 가능한 전략을 표적으로 삼아야 한다는 훈련-추론 연속 설계 방향을 시사한다.

방법론적으로, [[adversarial-problem-generation]] 계열의 동적 벤치마크가 난이도를 변이시킨다면 본 논문은 문제 구조 자체(비단사성)를 통제해 전략 관측 가능성을 확보하는 상보적 템플릿을 제공한다.

## 🔗 관련 논문

- Can RL Teach Long-Horizon Reasoning to LLMs? Expressiveness and Generalization
- Beyond Repeated Sampling: Learning Search Policies for LLM Reasoning
- MathDuels: Evaluating LLMs as Problem Posers and Solvers

## 🏷️ 엔티티

- [[entities/rlvr.md|rlvr]]
- [[entities/rl-reasoning-transfer-boundary.md|rl-reasoning-transfer-boundary]]
- [[entities/generalization-gap.md|generalization-gap]]
- [[entities/search-policy-learning.md|search-policy-learning]]

## 📐 개념

- [[concepts/reasoning-strategy-generalization.md|reasoning-strategy-generalization]]

---
_LLM 분석으로 생성됨_
