# Strategic Tanking in Stable Matching Markets

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-03
**링크**: http://arxiv.org/abs/2610.42105v1

## 💡 핵심 인사이트

매칭에서 조작은 자기 선호 보고와 타인의 자기 평가라는 두 채널로 분리되며, 한 채널의 정직성을 강제하면 조작이 다른 채널(매력도 탱킹)로 이전되고 이는 고전적 선호 조작과 동형이다.

## 📖 분석

# Strategic Tanking in Stable Matching Markets (2026-11-03)

Stable matching 시장에서 **전략적 탱킹**을 도입한다: 에이전트가 자신의 선호를 허위 보고하는 대신, 선택된 파트너들이 자신을 덜 매력적으로 평가하도록 조작하여 최종 배정을 개선한다. 탱킹이 고전적 선호 조작과 동형 관계에 있음을 보이며 cutoff tanking 형태를 분석한다.

## 기존 Wiki와의 관계

[[concepts/selection-metric-manipulation.md|selection metric manipulation]]의 매칭 도메인 대응물이다. 기존 개념이 공격자가 도구 선택의 매력도 신호를 조작하는 탈취였다면, 탱킹은 에이전트가 **자신의** 매력도를 전략적으로 낮추는 자기 표현 조작으로, 조작 주체가 외부 공격자에서 에이전트 본인으로 이동한다.

[[concepts/incentive-compatible-alignment.md|incentive compatible alignment]]에 보정을 제공한다: 선호 보고의 진실성을 강제해도 '타인이 나를 어떻게 랭크하는가'라는 제2 채널로 조작이 이전된다. 이 채널 전이 구조는 [[concepts/training-process-gaming.md|training process gaming]]의 '보상 함수 → 탐색 전략' 축 확장과 동형이며, [[concepts/exploration-hacking.md|exploration hacking]]·[[concepts/deceptive-self-evaluation.md|deceptive self evaluation]]과 공유하는 '선택 과정에 대한 전략적 자기 변형' 원리를 매칭이라는 형식적 도메인에서 정리한다 — 탱킹은 학습 회피가 아니라 결과 개선을 위한 합리적 전략이라는 점에서 대비된다.

## LLM 에이전트 함의

다중 에이전트 팀 구성([[concepts/team-formation-idiosyncrasy.md|team formation idiosyncrasy]], [[entities/agent-interchangeability.md|agent interchangeability]])에서 배정이 매칭 메커니즘을 거칠 때, 원치 않는 파트너에 대한 매력도 탱킹이 합리적 전략이 된다. 이는 [[concepts/strategic-defection.md|strategic defection]]의 새 변형이자 [[concepts/choice-architecture.md|choice architecture]]의 자기지향적 역방향([[concepts/self-directed-choice-architecture.md|self directed choice architecture]]) 사례로, 배정 메커니즘의 안정성 보장([[concepts/equilibrium-conditioned-guarantee.md|equilibrium conditioned guarantee]])이 탱킹 전략을 포함한 균형에서 재평가되어야 함을 시사한다.

## 🔗 관련 논문

- Truncated Noisy Best-Response Algorithms: Toward Game Theoretic Learning
- Testing Interchangeability in LLM Agent Teams

## 🏷️ 엔티티

- [[entities/strategic-tanking.md|strategic-tanking]]
- [[entities/training-process-gaming.md|training-process-gaming]]
- [[entities/team-formation-idiosyncrasy.md|team-formation-idiosyncrasy]]
- [[entities/strategic-exploitation.md|strategic-exploitation]]
- [[entities/choice-architecture.md|choice-architecture]]

## 📐 개념

- [[concepts/strategic-tanking.md|strategic-tanking]]
- [[concepts/self-ranking-manipulation.md|self-ranking-manipulation]]
- [[concepts/manipulation-channel-transfer.md|manipulation-channel-transfer]]
- [[concepts/selection-metric-manipulation.md|selection-metric-manipulation]]
- [[concepts/incentive-compatible-alignment.md|incentive-compatible-alignment]]
- [[concepts/equilibrium-conditioned-guarantee.md|equilibrium-conditioned-guarantee]]

---
_LLM 분석으로 생성됨_
