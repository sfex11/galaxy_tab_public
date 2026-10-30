# Can LLMs Uncover Hidden Physical Laws through Free Exploration?

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-30
**링크**: http://arxiv.org/abs/2610.37649v1

## 💡 핵심 인사이트

과학적 발견 능력의 평가 단위를 '주어진 질문에 대한 답'에서 '스스로 형성한 질문에 대한 발견'으로 격상시켜, 자발적 이상 감지와 자기 주도 실험 설계가 LLM 과학 능력의 진짜 병목임을 규명한다.

## 📖 분석

## 핵심 기여

과학적 발견의 첫 단계인 '질문 형성'을 평가 대상으로 격상시킨다. 물리 법칙이 하나 이상 실세계와 다르게 변형된 시뮬레이션 세계를 자동 생성하는 [[longchang]] 프레임워크를 제시하여, 에이전트가 이상 행동(예: 무거운 물체가 더 느리게 낙하)을 외부 지시 없이 스스로 감지하고 실험을 통해 법칙을 발견할 수 있는지를 측정한다. [[altered-physics-world]]의 원천이자 [[unguided-scientific-discovery]]의 체계적 평가 환경이다.

## 기존 Wiki와의 관계

- [[counterfactual-physics-reasoning]] 계열(DiscoverPhysics)이 out-of-the-box 추론을 물었다면, 본 논문은 '관찰→질문→실험→법칙'의 완전 사슬을 평가 대상으로 확장한다.
- [[environment-mutation-operator]]의 변이 대상이 문제 난이도(MathDuels 계열)에서 물리 법칙 자체로 이동한다. 법칙 수준 변이는 에이전트의 내재된 물리 사전과 환경 간 구조적 괴리를 의도적으로 창출하는 평가 환경 생성 수단이다.
- [[prior-violation-noticing]]이 발견 파이프라인의 첫 관문임을 실증한다 — 사전 위반이 감지되지 않으면 이후 전 과정이 무효화된다.
- [[autonomous-laboratory-agent]]의 요구 능력 스펙트럼을 소급 확장한다 — '무엇을 조사할지'가 미지수인 설정을 제공한다.
- [[formal-falsification]]과 대칭을 이룬다 — CPS 반증 프레임워크가 안전 검증의 역방향 방법론이었다면, 본 논문의 반증 루프는 지식 생성의 정방향 엔진이다.
- [[world-model]] 관점에서 에이전트의 암묵적 물리 사전과 실제 동역학 간 괴리 탐지·갱신 능력이 발견의 전제조건임을 보여준다.

## 인사이트

평가자가 질문을 사전에 고정하는 것 자체가 [[evaluator-assumption]]의 산물임을 드러내며, 개방형 목표 하 자기 주도 탐색이 LLM 과학 능력의 실질 병목임을 규명한다.

## 🔗 관련 논문

- DiscoverPhysics: Benchmarking LLMs for Out-of-the-Box Scientific Reasoning
- Evidence-Grounded Agentic Formulation Development in an Autonomous Laboratory
- Understanding the limits of latent world models
- Scaling Laws for Tool-Use Agents via Controllable Environment Synthesis
- MathDuels: Evaluating LLMs as Problem Posers and Solvers
- Large Language Models as Falsifiers for Cyber-Physical Systems

## 🏷️ 엔티티

- [[entities/longchang.md|longchang]]
- [[entities/unguided-scientific-discovery.md|unguided-scientific-discovery]]
- [[entities/counterfactual-physics-reasoning.md|counterfactual-physics-reasoning]]
- [[entities/environment-mutation-operator.md|environment-mutation-operator]]
- [[entities/prior-violation-noticing.md|prior-violation-noticing]]
- [[entities/autonomous-laboratory-agent.md|autonomous-laboratory-agent]]
- [[entities/world-model.md|world-model]]
- [[entities/formal-falsification.md|formal-falsification]]
- [[entities/evaluator-assumption.md|evaluator-assumption]]

## 📐 개념

- [[concepts/free-exploration-discovery.md|free-exploration-discovery]]
- [[concepts/prior-violation-noticing.md|prior-violation-noticing]]
- [[concepts/altered-physics-world.md|altered-physics-world]]

---
_LLM 분석으로 생성됨_
