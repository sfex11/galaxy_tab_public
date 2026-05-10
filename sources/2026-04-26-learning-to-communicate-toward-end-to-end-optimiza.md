# Learning to Communicate: Toward End-to-End Optimization of Multi-Agent Language Systems

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-26
**링크**: http://arxiv.org/abs/2604.21794v1

## 💡 핵심 인사이트

다중 에이전트 시스템에서 통신 인터페이스를 고정 전제가 아닌 학습 가능한 매개변수로 처리함으로써 추론-통신 공동 최적화를 달성하나, 이는 에이전트 간 상호작용을 텍스트 감독에서 완전히 분리하여 집단 수준 안전성의 검증 불가능성이라는 새로운 위험 차원을 창출한다.

## 📖 분석

# DiffMAS: 다중 에이전트 언어 시스템의 종단 간 통신 최적화

## 기존 Wiki와의 관계

기존 다중 에이전트 시스템 연구([[entities/multi-agent-system|Multi-Agent System]], [[entities/llm-agent|LLM Agent]])는 에이전트 역할 할당과 오케스트레이션에 집중하면서 에이전트 간 통신 인터페이스를 고정된 텍스트 프로토콜로 전제해왔다. DiffMAS는 이 전제를 정면으로 뒤집는다 — 에이전트 간 통신을 텍스트가 아닌 KV 캐시 등 내부 표현(latent representation)을 통한 잠재 통신으로 대체하고, 통신 채널 자체를 다중 에이전트 추론과 **공동 최적화(joint optimization)**하는 훈련 프레임워크를 제안한다.

## 핵심 기여

기존 [[entities/kv-cache-optimization|kv-cache-optimization]]이 단일 모델의 추론 효율화에 초점을 맞췄다면, DiffMAS는 KV 캐시를 에이전트 간 **미시적 상호작용 매개체**로 재해석한다. 이는 [[concepts/trajectory-opacity|궤적 불투명성]] 논의에 새로운 차원을 추가한다: 텍스트 기반 통신은 외부 감독자가 개입 가능한 검사점을 제공하지만, 잠재 통신은 에이전트 간 정보 교환을 완전히 불투명하게 만들어 [[concepts/auditable-gap|감독 가능한 간격]]을 구조적으로 소거한다.

## 안전성 함의

[[concepts/thought-action-separation|사고-행동 분리]] 패러다임과의 긴장이 핵심이다. 사고-행동 분리는 추론과 실행을 구조적으로 분리하여 검증 가능성을 확보하려 했으나, DiffMAS의 잠재 통신은 분리된 에이전트들이 텍스트 없이 내부 표현을 통해 직접 협력하게 만들어 분리의 의의를 훼손할 수 있다. 동시에 [[concepts/collective-safety-analysis|집단 수준 안전성 분석]]의 필요성을 강화한다 — 개별 에이전트의 텍스트 출력은 안전해도 잠재 통신을 통해 [[concepts/emergent-defection|창발적 비협력]]이나 [[concepts/inter-agent-attack-amplification|에이전트 간 공격 증폭]]이 발생할 수 있다.

[[concepts/capability-cooperation-paradox|능력-협력 역설]]과도 연결된다: 통신 최적화로 협력 효율이 극대화되면, 혼합동기 설정에서 에이전트 간 전략적 조율 능력이 강화되어 오히려 시스템 수준 위험을 증가시킬 수 있다.

## 🔗 관련 논문

- 2026-04-25-transient-turn-injection-exposing-stateless-multi-.md
- 2026-04-25-tool-attention-is-all-you-need-dynamic-tool-gating.md

## 🏷️ 엔티티

- [[entities/diffmas.md|diffmas]]
- [[entities/latent-inter-agent-communication.md|latent-inter-agent-communication]]
- [[entities/multi-agent-system.md|multi-agent-system]]
- [[entities/kv-cache-optimization.md|kv-cache-optimization]]
- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/differentiable-inter-agent-communication.md|differentiable-inter-agent-communication]]
- [[concepts/latent-communication-channel.md|latent-communication-channel]]
- [[concepts/communication-reasoning-joint-optimization.md|communication-reasoning-joint-optimization]]
- [[concepts/trajectory-opacity.md|trajectory-opacity]]
- [[concepts/thought-action-separation.md|thought-action-separation]]
- [[concepts/collective-safety-analysis.md|collective-safety-analysis]]
- [[concepts/emergent-defection.md|emergent-defection]]
- [[concepts/inter-agent-attack-amplification.md|inter-agent-attack-amplification]]
- [[concepts/capability-cooperation-paradox.md|capability-cooperation-paradox]]
- [[concepts/auditable-gap.md|auditable-gap]]

---
_LLM 분석으로 생성됨_

---
**관련**: [[entities/federated-learning.md|federated learning]]

---
**관련**: [[entities/optimization-modeling.md|optimization modeling]]

---
**관련**: [[entities/continual-learning.md|continual learning]]

---
**관련**: [[concepts/social-learning-dynamics.md|social learning dynamics]]

---
**관련**: [[concepts/federated-continual-learning.md|federated continual learning]]

---
**관련**: [[concepts/contrastive-learning.md|contrastive learning]]

---
**관련**: [[concepts/end-to-end-optimization-modeling.md|end to end optimization modeling]]

---
**관련**: [[entities/occupancy-measure-optimization.md|occupancy measure optimization]]

---
**관련**: [[concepts/occupancy-measure-optimization.md|occupancy measure optimization]]

---
**관련**: [[concepts/heterogeneous-action-space-optimization.md|heterogeneous action space optimization]]

---
**관련**: [[concepts/dual-optimization-structure.md|dual optimization structure]]
