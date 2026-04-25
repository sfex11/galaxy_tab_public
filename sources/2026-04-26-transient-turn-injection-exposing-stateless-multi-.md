# Transient Turn Injection: Exposing Stateless Multi-Turn Vulnerabilities in Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-26
**링크**: http://arxiv.org/abs/2604.21860v1

## 💡 핵심 인사이트

단일 턴 검열의 안전성 보장은 다중 턴 환경에서 합성되지 않으며, 턴 간 상태를 유지하지 않는 stateless moderation은 적대적 의도의 시간적 분산에 구조적으로 무방비하다.

## 📖 분석

# Transient Turn Injection: Exposing Stateless Multi-Turn Vulnerabilities in LLMs

## 핵심 기여

TTI(Transient Turn Injection)는 다중 턴 대화에서 검열(modulation)이 턴 간에 상태를 유지하지 않는 **stateless moderation의 구조적 결함**을 체계적으로 공격하는 기법이다. 단일 턴 내에서는 정책을 준수하면서도, 여러 터에 걸쳐 적대적 의도를 분산 배치하여 최종 턴에서 안전 정책을 우회한다.

## Wiki 연결망

### 안전성 전이 격차의 시간적 실증
기존 Wiki에 등록된 [[concepts/safety-transfer-gap|안전성 전이 격차]]가 제시한 메타프레임 — 평가 모달리티에서 검증된 안전성이 운영 모달리티로 전이되지 않는 현상 — 에 대해, TTI는 그 **시간적 인스턴스([[concepts/temporal-transfer-gap|시간적 전이 격차]])**를 구체적으로 실증한다. SafetyALFRED가 환경적 전이를 다루었다면, TTI는 동일 세션 내의 시간적 전이를 다룬다.

### 상태 없는 아키텍처 취약점의 공통 근원 확인
[[concepts/stateless-architecture-vulnerability|상태 없는 아키텍처 취약점]]이 도출한 통찰 — 도구 선택 맥락 상실과 안전 검열 맥락 상실의 공통 근원이 상태 없는 설계에 있다 — 에 대해, TTI는 안전 검열 측면에서 이를 독립적으로 확인한다. [[entities/tool-attention|Tool Attention]] 논문이 도구 스키마 맥락의 상실을 다루었다면, TTI는 안전 정책 맥락의 상실을 다룬다.

### 사후 가드레일 한계의 구조적 증명
[[concepts/post-hoc-guardrail-limitation|사후 가드레일 한계]]가 주장한 "런타임 가드레일이 근본적 안전을 보장하지 못한다"는 구조적 한계를, TTI는 실제 공격 성공률로 정량화한다. 턴별 독립 검사가 턴 간 의도 누적을 탐지하지 못함을 보여준다.

### 다중 턴 통계적 인증과의 긴장
[[concepts/multi-turn-statistical-certification|다중 턴 통계적 인증]]이 지적한 턴 수 증가에 따른 샘플 복잡도 기하급수적 증가 문제를, TTI는 공격자 측면에서 역이용한다. 안전 증명이 턴 시퀀스의 결합 분포를 다루어야 하지만, 현실적 검열은 각 턴의 주변 분포만 검사한다.

## 공격 메커니즘

LLM 기반 자동화 공격 에이전트가 반복적으로 턴 분할 전략을 탐색하여, 상업적·오픈소스 모델 모두에서 정책 집행을 회피한다. 이는 [[concepts/distributed-adversarial-intent|분산적 적대적 의도]] 개념의 구체적 구현이며, [[concepts/model-independent-safety-defect|모델 독립적 안전 결함]] 가설을 지지한다.

## 🔗 관련 논문

- 2026 04 25 tool attention is all you need dynamic tool gating
- 2026 04 23 safetyalfred evaluating safety conscious planning 
- 2026 04 25 bounding the black box a statistical certification
- 2026 04 23 an ai agent execution environment to safeguard use
- 2026 04 24 swe chat coding agent interactions from real users

## 🏷️ 엔티티

- [[entities/transient-turn-injection.md|transient-turn-injection]]
- [[entities/ai-safety.md|ai-safety]]
- [[entities/llm.md|llm]]
- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/stateless-moderation.md|stateless-moderation]]
- [[concepts/multi-turn-attack.md|multi-turn-attack]]
- [[concepts/safety-transfer-gap.md|safety-transfer-gap]]
- [[concepts/temporal-transfer-gap.md|temporal-transfer-gap]]
- [[concepts/stateless-architecture-vulnerability.md|stateless-architecture-vulnerability]]
- [[concepts/post-hoc-guardrail-limitation.md|post-hoc-guardrail-limitation]]
- [[concepts/distributed-adversarial-intent.md|distributed-adversarial-intent]]
- [[concepts/multi-turn-statistical-certification.md|multi-turn-statistical-certification]]
- [[concepts/model-independent-safety-defect.md|model-independent-safety-defect]]
- [[concepts/session-level-safety-enforcement.md|session-level-safety-enforcement]]

---
_LLM 분석으로 생성됨_
