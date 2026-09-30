# Towards Communication-Efficient Social Intelligence in Language Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-30
**링크**: http://arxiv.org/abs/2609.35749v1

## 💡 핵심 인사이트

사회적 지능의 본질은 말의 양이 아니라 '무엇을 말하지 않을 것인가'의 판단이며, 이 침묵 판단은 teacher 감독 하의 이중 목표 훈련으로 학습 가능하다.

## 📖 분석

TACT(Teacher-Assisted Communication Training)는 사회적 목표 달성을 높이면서 통신 비용을 낮추는 이중 목표를 teacher-student 훈련으로 동시 최적화한다. 핵심 진단은 에이전트가 파트너의 제약을 다루고 목표를 진전시킬 '충분한 말'과 상호작용에 기여하지 않는 '여분의 말'을 구분하지 못한다는 것이다. 이는 [[communication-access-planning-gap]]의 훈련 측 해법이 된다 — 대역폭이 아니라 '무엇을 말할지'의 계획 능력이 병목이라는 진단에 대해, 이 계획 능력 자체를 학습 가능한 정책으로 격상시킨다. 기존 [[knowledge-distillation]]이 지식·추론의 전이를 다뤘다면 TACT는 '침묵 판단'의 전이라는 새 축을 추가한다. [[expected-value-of-information]] 관점에서 각 발화의 기대 가치가 음수인 구간(도움 없는 말)을 teacher 감독으로 식별·억제하는 것으로 볼 수 있다. log(N)-Questions 게임([[shannon-game-taxonomy]], [[channel-capacity-bounded-refinement]])이 최적 프로토콜 하에서의 모델 한계를 진단했다면, TACT는 프로토콜이 아닌 훈련 신호 설계로 그 한계를 이동시키려는 경로다. 파트너의 시간·주의를 존중한다는 정의는 [[theory-of-mind]]가 추론 능력이 아닌 발화 억제 정책으로 실현되는 형태를 제시한다.

## 🔗 관련 논문

- Playing log(N)-Questions over Wikipedia Abstracts: Communication Effic
- The Natural Language Interaction Protocol and Standard for AI Agents
- Mind2Dialogue: Training Human-Aware Language Models by Simulating User
- Superintelligent Retrieval Agent: The Next Frontier of Information Ret

## 🏷️ 엔티티

- [[entities/communication-access-planning-gap.md|communication-access-planning-gap]]
- [[entities/expected-value-of-information.md|expected-value-of-information]]
- [[entities/token-efficiency.md|token-efficiency]]
- [[entities/knowledge-distillation.md|knowledge-distillation]]
- [[entities/theory-of-mind.md|theory-of-mind]]
- [[entities/teacher-assisted-communication-training.md|teacher-assisted-communication-training]]

## 📐 개념

- [[concepts/teacher-assisted-communication-training.md|teacher-assisted-communication-training]]
- [[concepts/communication-efficiency-under-social-goals.md|communication-efficiency-under-social-goals]]
- [[concepts/sufficiency-silence-boundary.md|sufficiency-silence-boundary]]

---
_LLM 분석으로 생성됨_
