# Bayesian Belief Layer for Controllable Opinion Dynamics in LLM Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-22
**링크**: http://arxiv.org/abs/2609.21997v1

## 💡 핵심 인사이트

LLM 에이전트의 신념 갱신을 컨텍스트 속 암묵적 현상에서 확률적 명시 계층으로 이전하면, 설득 수용도(κ)가 지정·검증 가능한 설계 파라미터가 되고 집단 의견 역학은 학습 사전분포의 은폐된 상속에서 벗어난다.

## 📖 분석

이 논문은 소셜 시뮬레이션에서 LLM 에이전트의 의견 수정이 암묵적으로 컨텍스트 내에서 일어나는 문제를 진단한다 — 설득 수용도를 지정·검증할 수 없고, 집단 의견 역학이 모델 학습 사전분포를 은밀히 상속한다. Bayesian Chronicle Agents(BCA)는 '무엇을 믿는가'와 '어떻게 말하는가'를 분리하는 최소 신념 계층을 제시한다: 각 입장은 확률로 표현되고, 들은 발화마다 베이지안 한 스텝으로 갱신되며, 단일 사전강도 파라미터 κ가 완고함을 인코딩한다.

Wiki 축적과의 관계: ① [[policy-constraint-hardening]]이 제안한 소프트 제약→하드 제약 전환의 신념 도메인 실현으로, [[context-delegation]]이 진단한 '암묵적 컨텍스트 위임'에 구조적 대안을 제공한다. ② [[bayesian-update-cumulative-error]]가 베이즈 규칙 위반의 누적 오차를 진단했다면, 본 논문은 발화당 정확히 한 스텝의 갱신 강제라는 처방 측을 완성한다. ③ [[sycophancy]]·[[agreement-pressure]] 측정 연구에 지정·검증 가능한 제어 변수 κ를 공급하여, 설득 수용성이 창발적 속성에서 설계 파라미터로 격상된다. ④ [[turn-driven-drift]]의 드리프트 원인(턴 수)이 실제 증거(발화)로 치환되고, [[machine-behavior]] 수준에서는 집단 의견 동역학의 사전 상속이 개별 κ 분포로 조정 가능해진다. 신념이 명시적 확률 객체가 되면 [[belief-aggregation]]과 [[collective-belief-formation]]이 전제하던 개체 수준 원시 연산이 처음으로 구현 가능해진다.

## 🔗 관련 논문

- Copying explains the collective behavior of AI agents in the wild
- Measuring LLM Sycophancy under Sustained Multi-Turn Pressure
- ADEMA: A Knowledge-State Orchestration Architecture for Long
- Flag Game: A Toy Model for Mechanistic Swarm Interpretabilit
- Binary Decisions in DAOs: Accountability and Belief Aggregat
- Position: agentic AI orchestration should be Bayes-consisten

## 🏷️ 엔티티

- [[entities/explicit-belief-layer.md|explicit-belief-layer]]
- [[entities/bayesian-chronicle-agents.md|bayesian-chronicle-agents]]
- [[entities/policy-constraint-hardening.md|policy-constraint-hardening]]
- [[entities/context-delegation.md|context-delegation]]
- [[entities/bayesian-update-cumulative-error.md|bayesian-update-cumulative-error]]
- [[entities/sycophancy.md|sycophancy]]
- [[entities/agreement-pressure.md|agreement-pressure]]
- [[entities/turn-driven-drift.md|turn-driven-drift]]
- [[entities/knowledge-state-drift.md|knowledge-state-drift]]
- [[entities/machine-behavior.md|machine-behavior]]
- [[entities/belief-aggregation.md|belief-aggregation]]
- [[entities/collective-belief-formation.md|collective-belief-formation]]
- [[entities/belief-state-grounding.md|belief-state-grounding]]
- [[entities/bias-synchronization.md|bias-synchronization]]

## 📐 개념

- [[concepts/explicit-belief-layer.md|explicit-belief-layer]]
- [[concepts/bayesian-chronicle-agents.md|bayesian-chronicle-agents]]
- [[concepts/prior-strength-parameter.md|prior-strength-parameter]]
- [[concepts/belief-generation-separation.md|belief-generation-separation]]
- [[concepts/training-prior-inheritance.md|training-prior-inheritance]]
- [[concepts/bayesian-update-per-utterance.md|bayesian-update-per-utterance]]

---
_LLM 분석으로 생성됨_
