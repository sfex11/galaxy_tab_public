# Can LLMs Uncover Hidden Physical Laws through Free Exploration?

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-29
**링크**: http://arxiv.org/abs/2610.37649v1

## 💡 핵심 인사이트

기존 과학 벤치마크가 '주어진 질문에 답하는 능력'을 측정했다면, LongChang은 '무엇을 질문할지 스스로 발견하는 능력'을 측정하여 과학적 발견 평가의 출발점을 관찰 단계로 이동시킨다.

## 📖 분석

본 논문은 LongChang 프레임워크를 제안하여, 물리 법칙이 변형된 시뮬레이션 세계에서 LLM이 조사 대상을 통보받지 않은 채 이상 현상(예: 무거운 물체가 더 천천히 낙하)을 스스로 인지하고, 자유 탐색을 통해 법칙을 발견할 수 있는지 평가한다. 과학적 발견이 예상치 못한 관찰에서 시작한다는 통찰을 벤치마크 설계 원리로 형식화한 것이다.

DiscoverPhysics([[counterfactual-physics-reasoning]])가 주어진 질문에 대한 out-of-the-box 과학 추론을 측정했다면, 본 논문은 '이상 인지→질문 형성→실험 설계→법칙 발견'의 전 과정을 측정하여 과학 능력 평가의 출발점을 관찰 단계까지 소급한다.

변형 세계 생성은 [[agent-environment-generation]]의 평가 도메인 확장이며, 법칙 수준 변이는 [[environment-mutation-operator]]의 변이 대상이 태스크 난이도에서 물리 법칙 자체로 확장된 사례다. LLM의 사전 세계 모델([[world-model]])과 환경 간 괴리가 발견의 트리거가 된다는 점에서, 세계 모델 오류의 인식론적 지위가 결함에서 탐사 근거로 전환된다. 조사 대상의 부재는 [[reward-sparsity]]의 극단 형태로, 가이던스 없는 자율 탐색 능력이 새로운 평가 축임을 보여준다.

## 🔗 관련 논문

- DiscoverPhysics: Benchmarking LLMs for Out-of-the-Box Scientific Reasoning
- Evidence-Grounded Agentic Formulation Development in an Autonomous Lab
- Can Coding Agents Reproduce Findings in Computational Materials Science

## 🏷️ 엔티티

- [[entities/counterfactual-physics-reasoning.md|counterfactual-physics-reasoning]]
- [[entities/agent-environment-generation.md|agent-environment-generation]]
- [[entities/environment-mutation-operator.md|environment-mutation-operator]]
- [[entities/world-model.md|world-model]]
- [[entities/reward-sparsity.md|reward-sparsity]]
- [[entities/autonomous-laboratory-agent.md|autonomous-laboratory-agent]]
- [[entities/longchang.md|longchang]]
- [[entities/unguided-scientific-discovery.md|unguided-scientific-discovery]]

## 📐 개념

- [[concepts/prior-violation-noticing.md|prior-violation-noticing]]
- [[concepts/free-exploration-discovery.md|free-exploration-discovery]]
- [[concepts/altered-physics-world.md|altered-physics-world]]
- [[concepts/unguided-scientific-discovery.md|unguided-scientific-discovery]]

---
_LLM 분석으로 생성됨_
