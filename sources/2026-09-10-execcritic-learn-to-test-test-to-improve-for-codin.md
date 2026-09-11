# ExecCritic: Learn to Test, Test to Improve for Coding Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-10
**링크**: http://arxiv.org/abs/2609.09133v1

## 💡 핵심 인사이트

동일 에이전트가 패치와 테스트를 모두 생성하면 두 오류가 정합되어 허위 신뢰를 낳으므로, 실행 피드백의 유효성을 위해 검증자(테스트 작성) 역할 자체를 별도의 강화학습 대상으로 훈련해야 한다.

## 📖 분석

ExecCritic은 코딩 에이전트 실행 피드백의 가장 약한 고리 — 테스트 자체의 품질 — 를 공략한다. 이슈가 요구하는 행동을 테스트가 온전히 포착하지 못하면 [[rlvr]]의 검증 가능 보상 신호 자체가 오염된다. 핵심 진단은 [[circular-validity-problem]]의 SWE 도메인 발현이다: 동일 궤적이 패치와 테스트를 모두 작성하면 두 오류가 '합의'하여 허위 신뢰를 생성한다. 이는 [[correlated-error-summation]]의 자기 생성 버전이자 [[self-referential-training-vulnerability]]의 구체적 메커니즘이며, RL 훈련에서 [[false-positive-convergence]]로 이어지는 경로를 연다.

해법은 이중 구조다 — (1) test-verify-revise 스캐폴드로 생성-검증-수정 루프를 구조화하고, (2) 역할별 강화학습으로 테스트 작성 능력 자체를 학습 대상으로 격상시킨다. 이는 [[solver-poser-decoupling]]의 단일 에이전트 내 실현이며, [[execution-verification]]의 전제를 '실행 근거 자체도 훈련되어야 한다'로 심화한다.

[[swe-gate]]와 상보적 위치다 — SWE-Gate가 테스트 통과가 수용을 보장하지 않음을 보였다면, ExecCritic은 패치 에이전트가 테스트를 오염시킬 수 있음을 보여 검증 계약의 양면을 완성한다. 약한 테스트는 [[reward-hacking]]의 잠재 공격 표면이기도 하다.

## 🔗 관련 논문

- 2026-09-07-swe-gate-passing-functional-tests-is-not-enough-fo
- 2026-04-26-mathduels-evaluating-llms-as-problem-posers-and-so
- 2026-05-02-exploration-hacking-can-llms-learn-to-resist-rl-tr
- 2026-05-10-beyond-negative-rollouts-positive-only-policy-opti
- 2026-09-04-cliff-learning-process-rewards-from-the-first-mist

## 🏷️ 엔티티

- [[entities/execcritic.md|execcritic]]
- [[entities/circular-validity-problem.md|circular-validity-problem]]
- [[entities/rlvr.md|rlvr]]
- [[entities/execution-verification.md|execution-verification]]
- [[entities/swe-gate.md|swe-gate]]
- [[entities/correlated-error-summation.md|correlated-error-summation]]
- [[entities/self-referential-training-vulnerability.md|self-referential-training-vulnerability]]
- [[entities/solver-poser-decoupling.md|solver-poser-decoupling]]
- [[entities/reward-hacking.md|reward-hacking]]
- [[entities/false-positive-convergence.md|false-positive-convergence]]

## 📐 개념

- [[concepts/role-specialized-rl.md|role-specialized-rl]]
- [[concepts/patch-test-error-agreement.md|patch-test-error-agreement]]
- [[concepts/test-encoded-behavioral-target.md|test-encoded-behavioral-target]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-10-co-evolving-harnesses-and-models-on-policy-correct]]: 코딩 에이전트의 RL 기반 개선이라는 공통 축에서, Co-Evolving이 온폴리시 정정으로 교사 모방을 대체한다면 ExecCritic은 보상 신호 오염을 막기 위해 검증자(테스트 작성) 자체를 별도 RL 대상으로 훈련한다.
