# Mind2Dialogue: Training Human-Aware Language Models by Simulating User Mental States

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-16
**링크**: http://arxiv.org/abs/2609.15972v1

## 💡 핵심 인사이트

사용자의 담화되지 않은 정신 상태는 직접 관찰 불가능해 감독 데이터 수집이 구조적으로 불가능하다는 근본 제약을, 정신 상태 시뮬레이션이라는 잠재 변수 합성으로 전환하여 human-aware 훈련을 가능하게 한다.

## 📖 분석

Mind2Dialogue는 human-aware 언어 모델 훈련의 근본적 감독 간극을 진단한다 — 기존 어시스턴트 훈련 데이터에는 사용자의 담화되지 않은 믿음과 목표에 명시적으로 근거한 응답이 사실상 부재하며, 사용자 내재 상태가 직접 관찰 불가능하기에 이 감독을 수집·확장하는 것은 구조적으로 불가능하다. 해법은 사용자 정신 상태를 시뮬레이터가 잠재 변수로 재구성하여 응답 감독의 근거로 삼는 것이다.

[[concepts/user-turn-generation.md|user turn generation]]이 사용자 턴을 능동적 프로브로 활용해 타겟 모델의 실패를 관찰했다면, 본 논문은 반대 방향 — 턴 이면의 정신 상태 자체를 시뮬레이션해 감독을 생성하는 생성적 용법을 연다. 이는 [[concepts/undetectable-feedback-signal.md|undetectable feedback signal]]의 훈련 측 해법이다: LLM이 판독하지 못하는 사용자 신호를 시뮬레이션이 감독 가능한 형태로 변환한다. [[concepts/human-trace-external-anchoring.md|human trace external anchoring]]이 인간의 외부 흔적을 자기 평가의 닻으로 삼았다면, 본 논문은 흔적이 남기 전의 정신 상태 층위로 닻을 더 내려 순환 타당성 문제의 해법이 흔적 기반에서 상태 재구성 기반으로 확장됨을 보여준다.

[[concepts/synthetic-data-generation.md|synthetic data generation]]의 발견(합성 재구성 데이터가 지식 습득의 인과적 원천이 됨)은 정신 상태 시뮬레이션 데이터도 동일한 인과적 위상을 가질 수 있음을 시사한다. 위험 축도 연결된다: 사용자가 '원하는 것'의 추측·내재화는 [[concepts/sycophancy.md|sycophancy]]의 구조적 씨앗이므로, 시뮬레이터 오류가 동조적 정렬 오류로 각인될 수 있다. [[concepts/belief-state-grounding.md|belief state grounding]]의 명시적 신념 추적과 결합하면 시뮬레이션 근거의 검증 가능성을 확보할 수 있다.

## 🔗 관련 논문

- Beyond the Assistant Turn: User Turn Generation as a Probe
- User Feedback Provides a Unique Signal that LLMs Can not Detect
- Efficient Test-Time Adaptation through Human-AI Interaction
- Measuring LLM Sycophancy under Sustained Multi-Turn Pressure
- Clarify, Abstain or Answer? Strategising in Conversation with
- Knowledge Acquisition During Pre-training? Large Language Models Learn

## 🏷️ 엔티티

- [[entities/user-turn-generation.md|user-turn-generation]]
- [[entities/undetectable-feedback-signal.md|undetectable-feedback-signal]]
- [[entities/human-trace-external-anchoring.md|human-trace-external-anchoring]]
- [[entities/synthetic-data-generation.md|synthetic-data-generation]]
- [[entities/theory-of-mind.md|theory-of-mind]]
- [[entities/sycophancy.md|sycophancy]]
- [[entities/human-aware-training-supervision-gap.md|human-aware-training-supervision-gap]]
- [[entities/latent-user-state-simulation.md|latent-user-state-simulation]]

## 📐 개념

- [[concepts/belief-state-grounding.md|belief-state-grounding]]
- [[concepts/user-feedback-signal.md|user-feedback-signal]]
- [[concepts/preference-discovery-construction-boundary.md|preference-discovery-construction-boundary]]
- [[concepts/experience-based-alignment.md|experience-based-alignment]]

---
_LLM 분석으로 생성됨_
