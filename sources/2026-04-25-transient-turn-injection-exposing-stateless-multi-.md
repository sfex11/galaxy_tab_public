# Transient Turn Injection: Exposing Stateless Multi-Turn Vulnerabilities in Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-25
**링크**: http://arxiv.org/abs/2604.21860v1

## 💡 핵심 인사이트

턴 단위 무상태 검열은 각 턴이 개별적으로 안전하더라도 턴 시퀀스의 합성이 안전하지 않을 수 있다는 구성적 안전성 문제를 대화 도메인에서 체계적으로 공격 가능하게 만드는 구조적 취약성이다.

## 📖 분석

# Transient Turn Injection: Stateless Moderation의 구조적 취약성

## 핵심 발견

Transient Turn Injection(TTI)는 LLM의 안전 검열이 **턴 단위로 무상태(stateless)적으로 수행된다**는 구조적 결함을 체계적으로 공격하는 기법이다. 개별 턴은 각각 정책을 준수하므로 단독으로는 무해해 보이지만, 다중 턴에 걸쳐 적대적 의도를 분산 배치함으로써 최종적으로 정책 위반 결과를 달성한다.

## 기존 Wiki와의 관계

### compositional-safety의 실증적 사례
TTI는 Wiki에 이미 축적된 구성적 안전성 불가능성 — safe(A) ∧ safe(B) ⊭ safe(A∘B) — 를 대화 도메인에서 구체적으로 실증한다. 각 턴이 개별적으로 안전하더라도 턴의 합성(sequence)이 안전하지 않다는 것을 공격자 관점에서 증명한다.

### post-hoc-guardrail-limitation의 결정적 사례
상태less 턴별 검열은 사후 가드레일의 파라다임적 사례이다. [[concepts/post-hoc-guardrail-limitation|사후적 가드레일 한계]]가 이론적으로 경고하던 바를 TTI가 실험적으로 확인한다 — 검열이 생성 이후 각 턴에 독립적으로 적용될 때, 턴 간 맥락을 고려하지 못하는 것이 치명적 공격 표면이 된다.

### model-independent-safety-defect의 확장
상업 모델과 오픈소스 모델 모두에서 TTI가 작동한다면, 이는 특정 모델의 정렬 결함이 아니라 **검열 아키텍처 패러다임 자체의 결함**이다. 기존 Wiki가 체화 계획 도메인에서 식별했던 모델 독립적 안전 결함을 대화 수준 안전으로 확장한다.

## 공격 메커니즘

LLM 기반 공격자 에이전트가 반복적으로 턴을 생성·테스트하며 정책 집행을 우회하는 경로를 자동 탐색한다. 이는 [[entities/llm-agent|LLM 에이전트]]의 계획 능력이 공격 도구로 전용되는 사례로, [[concepts/strategic-exploitation|전략적 착취]] 개념과 연결된다.

## 방어 함의

TTI에 대한 근본적 방어는 턴 수준 검열을 넘어 **세션 수준(stateful) 맥락 추적**이 필요함을 시사하며, 이는 [[concepts/intra-generative-intervention|추론 중간 개입]]이 턴 간 경계로 확장되어야 함을 의미한다. [[entities/ai-safety|AI 안전성]] 연구가 단일 턴 평가에서 세션 수준 평가로 패러다임 전환을 요구하는 논거를 강화한다.

## 🔗 관련 논문

- 2026 04 23 an ai agent execution environment to safeguard use
- 2026 04 23 safetyalfred evaluating safety conscious planning
- 2026 04 24 relative principals pluralistic alignment and the

## 🏷️ 엔티티

- [[entities/ai-safety.md|ai-safety]]
- [[entities/llm-agent.md|llm-agent]]
- [[entities/llm.md|llm]]
- [[entities/transient-turn-injection.md|transient-turn-injection]]

## 📐 개념

- [[concepts/stateless-moderation.md|stateless-moderation]]
- [[concepts/distributed-adversarial-intent.md|distributed-adversarial-intent]]
- [[concepts/compositional-safety.md|compositional-safety]]
- [[concepts/post-hoc-guardrail-limitation.md|post-hoc-guardrail-limitation]]
- [[concepts/model-independent-safety-defect.md|model-independent-safety-defect]]
- [[concepts/multi-turn-attack.md|multi-turn-attack]]
- [[concepts/session-level-safety-enforcement.md|session-level-safety-enforcement]]

---
_LLM 분석으로 생성됨_
