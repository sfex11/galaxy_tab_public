# Shockingly Simple Self-retrospection Improves Agentic Models Without RL

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-30
**링크**: http://arxiv.org/abs/2609.35741v1

## 💡 핵심 인사이트

보상도 시연도 아닌 자기 경험에 대한 설명 텍스트만으로 에이전트가 개선될 수 있다 — 학습 신호의 최소 단위가 외부 검증이 아닌 자기 서술일 수 있음을 실증한다.

## 📖 분석

ROFT(Retrospection-Only Fine-Tuning)는 에이전트가 과제 수행 경험을 '설명'하는 텍스트만으로 후속 행동을 개선하는 최소 온라인 절차로, RL이나 시연 없이 설명-전용 훈련이 행동 개선을 유발하는지 분리 검증한다. Wiki가 축적해온 경험 재사용 스펙트럼에 새 소비 경로를 추가한다 — [[experience-reuse]]가 궤적을 스킬(SkillOS), 환경(Terminal-Universe), 코칭 신호(Learning to Coach)로 소비했다면, ROFT는 궤적을 '서술'로 소비한다. 인간 인지과학의 자기설명 효과(self-explanation effect)를 에이전트 학습으로 이식한 것으로, 학습 신호의 단위가 상태 전이([[trajectory-as-coaching-signal]])나 보상([[rlvr]])이 아니라 설명 자체임을 시사한다. [[retrospective-thinking]]이 추론 시점 회고였다면 본 논문은 훈련 시점 회고로 축을 확장한다. 동시에 모델이 생성한 설명을 그 모델이 다시 학습하는 폐루프([[bootstrap-paradox]])의 실증 무대가 되어, [[circular-validity-problem]]과 [[self-referential-training-vulnerability]]가 제기한 자기참조 학습 타당성 문제를 개선의 관점에서 재검토하게 한다. [[self-improving-agent]] 스펙트럼에서 RL-free·검증자-free 개선 경로로서 [[closed-loop-training]]과 [[self-training-data-construction]] 논의를 연결한다.

## 🔗 관련 논문

- Strategically Diverse Sampling for Self-Training
- User Model Extraction via Belief Self-Distillation

## 🏷️ 엔티티

- [[entities/self-improving-agent.md|self-improving-agent]]
- [[entities/experience-reuse.md|experience-reuse]]
- [[entities/trajectory-as-coaching-signal.md|trajectory-as-coaching-signal]]
- [[entities/retrospective-thinking.md|retrospective-thinking]]
- [[entities/rlvr.md|rlvr]]
- [[entities/circular-validity-problem.md|circular-validity-problem]]
- [[entities/bootstrap-paradox.md|bootstrap-paradox]]
- [[entities/self-referential-training-vulnerability.md|self-referential-training-vulnerability]]
- [[entities/closed-loop-training.md|closed-loop-training]]
- [[entities/self-training-data-construction.md|self-training-data-construction]]

## 📐 개념

- [[concepts/explanation-only-training.md|explanation-only-training]]
- [[concepts/self-narration-as-training-signal.md|self-narration-as-training-signal]]

---
_LLM 분석으로 생성됨_
