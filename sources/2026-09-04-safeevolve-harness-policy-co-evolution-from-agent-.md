# SafeEvolve: Harness-Policy Co-Evolution from Agent Experience for Safety Alignment

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-04
**링크**: http://arxiv.org/abs/2609.02786v1

## 💡 핵심 인사이트

안전 정렬은 외부 하네스 제어와 내부 정책 최적화 중 하나의 고립적 적용으로는 달성 불가능하며, 에이전트 경험에서 두 계층이 동시 진화하는 공진화를 통해서만 런타임 제어와 내재적 안전이 결합된다.

## 📖 분석

SafeEvolve는 안전 정렬의 두 대립 패러다임 — 외부 하네스 업데이트(런타임 제어)와 내부 정책 최적화(내재적 안전) — 중 어느 하나의 고립적 적용은 런타임 제어와 내재적 안전 사이의 간극을 메우지 못한다고 진단한다. 이는 [[dual-layer-safety-inevitability]]의 직접적 실증이다: 안전성이 모델 내부에 내재되어야 한다는 요구([[capability-safety-inseparability]])와 외부에서 검증·제어되어야 한다는 요구([[algorithm-system-translation-gap]])가 동시에 충족되어야 하기 때문이다.

기존 [[harness-model-co-evolution]](Design Conductor 2.0)이 하드웨어 설계의 성능 최적화를 대상으로 했다면, SafeEvolve는 공진화의 대상을 안전 정렬로 확장한다. 에이전트 경험에서 하네스 정책과 모델 정책을 동시에 진화시켜, 안전을 정적 속성이 아닌 지속 유지가 필요한 조건부 상태([[safety-as-conditional-state]])로 다룬다.

이 논문은 세 지점에서 기존 Wiki를 연결한다: (1) [[harness-native-training]]의 훈련-배포 인터페이스 통합 논리를 안전 차원으로 이식한다. (2) [[experience-based-alignment]]가 스킬 성공률 기반 행동 최적화였다면, 안전 경험 자체가 정렬의 학습 원료가 됨을 보여준다. (3) 유해 최종 응답과 다단계 실행 궤적을 모두 위험 대상으로 삼아, [[trajectory-opacity]]가 지적한 궤적 수준 안전 문제를 자가 진화 루프로 해결하려 한다. 다만 [[endogenous-self-evolution]]의 자기 참조적 위험([[exploration-hacking]])이 안전 진화 루프에서도 재현될 수 있다는 점은 후속 검증 과제로 남는다.

## 🔗 관련 논문

- Design Conductor 2.0: An agent builds a TurboQuant inference
- MOSS: Self-Evolution through Source-Level Rewriting in Auton
- Exploration Hacking: Can LLMs Learn to Resist RL Training?
- SkillOS: Learning Skill Curation for Self-Evolving Agents

## 🏷️ 엔티티

- [[entities/harness-model-co-evolution.md|harness-model-co-evolution]]
- [[entities/agentic-harness-engineering.md|agentic-harness-engineering]]
- [[entities/dual-layer-safety-inevitability.md|dual-layer-safety-inevitability]]
- [[entities/ai-safety.md|ai-safety]]
- [[entities/experience-based-alignment.md|experience-based-alignment]]
- [[entities/harness-native-training.md|harness-native-training]]
- [[entities/safety-as-conditional-state.md|safety-as-conditional-state]]
- [[entities/endogenous-self-evolution.md|endogenous-self-evolution]]

## 📐 개념

- [[concepts/harness-policy-co-evolution.md|harness-policy-co-evolution]]
- [[concepts/experience-driven-safety-alignment.md|experience-driven-safety-alignment]]
- [[concepts/runtime-intrinsic-safety-bridge.md|runtime-intrinsic-safety-bridge]]
- [[concepts/trajectory-level-strategy.md|trajectory-level-strategy]]
- [[concepts/self-referential-agent-paradigm.md|self-referential-agent-paradigm]]

---
_LLM 분석으로 생성됨_
