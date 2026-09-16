# Learning to Coach for Experiential Learning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-16
**링크**: http://arxiv.org/abs/2609.15851v1

## 💡 핵심 인사이트

원시 궤적에서 실행 가능한 지식을 추출하는 추상화 연산 자체를 별도 코치 모듈로 학습시켜, 개선 능력을 동결된 성능 모델과 분리하고 하류 보상으로 최적화할 수 있음을 입증했다.

## 📖 분석

## 핵심 요약

L2C는 궤적 소비 경로에 '코칭'이라는 제3의 중간자를 추가한다. 기존 Wiki에서 궤적은 스킬로 절차화되거나([[skillos]]), 환경으로 재질화되거나([[terminal-universe]]), 보상 신호로 소비되었으나, L2C는 궤적을 코치 모듈의 훈련 신호로 소비하여 액터의 후속 응답 정확도로 환류되는 간접 재사용 경로를 연다.

## 구조적 발견

1. **개선-성능 분리**: 개선 능력이 액터와 분리된 별도 파라미터 공간(코치)에 거주하며 액터는 동결된다. LOCUS·이산 확산 계열의 파라미터화-행동 분리를 모듈 간 분리로 확장한다([[parameter-decoupling]]).

2. **추상화의 학습 가능성**: 잡음 난 원시 궤적에서 실행 가능한 지식 추출 자체가 하류 보상으로 최적화 가능한 학습 연산임을 입증한다. 규칙 기반 큐레이션([[skill-curation-as-learning]])과 달리 추상화 품질이 외부 검증자(액터 성능)로 간접 평가되므로, 추출의 질에 대한 순환적 자가 판정 문제를 우회한다.

3. **동결 액터의 상한 내 개선**: P(y) 불변 하에서 코칭이 조건부 유도만 재구성하는 구조로 [[marginal-distribution-ceiling]]의 실증 사례가 된다.

자기 개선([[self-improving-agent]])과 대비되는 '외부 위임 개선'의 극단으로, 개선 실행 자율성 스펙트럼([[improvement-execution-autonomy]])의 반대편을 표시한다.

## 🔗 관련 논문

- SkillOS: Learning Skill Curation for Self-Evolving Agents
- From Raw Experience to Skill Consumption: A Systematic Study
- Terminal-Universe: Turning Agent Trajectories into Scalable Terminal E
- LOCUS: Task-Aware Low-Rank Post-Training for Token-Efficient Language
- Unlocking Lossless Speedups in LLMs via Discrete Diffusion

## 🏷️ 엔티티

- [[entities/experience-reuse.md|experience-reuse]]
- [[entities/skill-consumption-gap.md|skill-consumption-gap]]
- [[entities/self-improving-agent.md|self-improving-agent]]
- [[entities/parameter-decoupling.md|parameter-decoupling]]
- [[entities/harness-side-compensation.md|harness-side-compensation]]
- [[entities/credit-assignment-granularity.md|credit-assignment-granularity]]
- [[entities/llm-as-judge.md|llm-as-judge]]
- [[entities/generalization-gap.md|generalization-gap]]
- [[entities/marginal-distribution-ceiling.md|marginal-distribution-ceiling]]
- [[entities/skill-curation-as-learning.md|skill-curation-as-learning]]
- [[entities/improvement-execution-autonomy.md|improvement-execution-autonomy]]

## 📐 개념

- [[concepts/coach-actor-decoupling.md|coach-actor-decoupling]]
- [[concepts/llm-as-coach.md|llm-as-coach]]
- [[concepts/coaching-reward.md|coaching-reward]]
- [[concepts/trajectory-as-coaching-signal.md|trajectory-as-coaching-signal]]
- [[concepts/improvement-delegation.md|improvement-delegation]]

---
_LLM 분석으로 생성됨_
