# Recursive Multi-Agent Systems

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-30
**링크**: http://arxiv.org/abs/2604.25917v1

## 💡 핵심 인사이트

다중 에이전트 협력을 프로토콜 설계 문제가 아닌 연산적 스케일링 문제로 재정의하여, 협력 루프의 반복 깊이 자체가 새로운 확장 축이 됨을 보여준다.

## 📖 분석

# RecursiveMAS: 순환적 다중 에이전트 시스템

**카테고리**: AI/ML — 다중 에이전트 시스템
**생성일**: 2026-04-30

## 정의

RecursiveMAS는 단일 모델의 잠재 상태 순환 반복(latent-state recursion)이라는 확장 축을 다중 에이전트 시스템으로 전이한 프레임워크로, 이질적 에이전트 간 협력 자체를 순환적 연산으로 취급하여 협력의 '깊이'를 스케일링한다.

## 기존 Wiki와의 관계

기존 [[entities/latent-inter-agent-communication|잠재 에이전트 간 통신]]이 에이전트 간 정보 전달의 '형태'를 잠재 공간으로 이전했다면, RecursiveMAS는 이를 한 단계 더 나아가 통신 자체를 '순환적 연산 단계'로 재정의한다. 즉, 에이전트 A의 출력이 잠재 공간에서 에이전트 B에 의해 정제되고, 이 정제 결과가 다시 A로 피드백되는 루프가 단일 모델의 recursive reasoning과 동등한 연산 단위로 처리된다.

이는 [[concepts/thought-action-separation|사고-행동 분리]] 논의에 새로운 복잡성을 추가한다. 잠재 공간에서의 순환적 정제가 '사고'인지 '협력적 행동'인지 경계가 모호해지며, [[concepts/trajectory-opacity|궤적 불투명성]]은 단일 에이전트의 내적 추론을 넘어 에이전트 간 순환 루프 전체로 확장된다.

## 핵심 메커니즘

1. **통합 잠재 공간**: 이질적 에이전트가 공유하는 잠재 표현 공간에서 상호 정제 수행
2. **순환 깊이 스케일링**: 반복 횟수를 늘려 협력 자체의 깊이를 확장
3. **단일 연산으로의 통합**: 다중 에이전트 상호작용을 하나의 확장된 순환 연산으로 취급

## 연결점

[[sources/2026-04-26-learning-to-communicate-toward-end-to-end-optimiza.md|Learning to Communicate]]가 미시적 통신 채널을 최적화했다면, RecursiveMAS는 최적화된 채널 위에서의 거시적 순환 구조를 설계한다. [[concepts/capability-cooperation-paradox|능력-협력 역설]]에 대한 잠재적 해법 경로이기도 한데, 순환적 정제가 전략적 이기심을 상쇄하는지는 미해결 질문이다.

## 🔗 관련 논문

- 2026 04 26 learning to communicate toward end to end optimiza

## 🏷️ 엔티티

- [[entities/multi-agent-system.md|multi-agent-system]]
- [[entities/latent-inter-agent-communication.md|latent-inter-agent-communication]]
- [[entities/differentiable-inter-agent-communication.md|differentiable-inter-agent-communication]]
- [[entities/latent-communication-channel.md|latent-communication-channel]]
- [[entities/recursive-multi-agent-scaling.md|recursive-multi-agent-scaling]]
- [[entities/communication-reasoning-joint-optimization.md|communication-reasoning-joint-optimization]]

## 📐 개념

- [[concepts/recursive-collaboration-scaling.md|recursive-collaboration-scaling]]
- [[concepts/agent-loop-as-computation.md|agent-loop-as-computation]]
- [[concepts/latent-space-agent-unification.md|latent-space-agent-unification]]
- [[concepts/collaboration-depth-axis.md|collaboration-depth-axis]]

---
_LLM 분석으로 생성됨_
