# Who Governs the Machine? A Machine Identity Governance Taxonomy (MIGT) for AI Systems Operating Across Enterprise and Geopolitical Boundaries

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-09
**링크**: http://arxiv.org/abs/2604.06148v1

## 💡 핵심 인사이트

AI 에이전트의 자율성이 확대될수록, 모델 자체의 안전성뿐 아니라 에이전트가 행동에 사용하는 머신 아이덴티티(API 토큰, 서비스 계정 등)의 수명주기 거버넌스가 기업·지정학적 보안의 핵심 취약점이 된다.

## 📖 분석

## Who Governs the Machine? A Machine Identity Governance Taxonomy (MIGT)

AI 시스템의 거버넌스에서 간과되어 온 **머신 아이덴티티(machine identity)** 문제를 체계적으로 다룬 논문이다. AI 에이전트, 서비스 계정, API 토큰, 자동화 워크플로우 등 머신 아이덴티티가 기업 환경에서 인간 아이덴티티 대비 80:1 이상의 비율로 존재하지만, 이를 통합적으로 거버넌스하는 프레임워크가 부재했다는 점을 지적한다. 2024년 CrowdStrike 장애에서 단일 비관리 에이전트가 54~100억 달러 손실을 야기한 사례, Silk Typhoon·Salt Typhoon 등 국가 행위자의 머신 아이덴티티 악용 사례를 근거로 제시한다.

**MIGT(Machine Identity Governance Taxonomy)**는 머신 아이덴티티의 분류, 수명주기 관리, 크로스보더 규제 대응을 위한 통합 프레임워크를 제안한다. 이는 기존 [[ai-governance]] 논의가 주로 모델의 공정성·안전성에 집중한 반면, 운영 인프라 수준의 아이덴티티 관리라는 새로운 축을 추가한다.

[[llm-agent]] 및 [[multi-agent-system]] 연구가 에이전트의 자율성과 협업에 초점을 맞추는 데 비해, 본 논문은 에이전트가 실제로 '행동'할 때 사용하는 인증·권한 체계의 거버넌스를 다룬다는 점에서 상호보완적이다. [[privilege-escalation]] 연구(OpenClaw 보안 평가)와도 직접적으로 연결되며, 머신 아이덴티티의 과잉 권한이 공격 표면을 확대한다는 공통 문제의식을 공유한다. [[ai-safety]] 관점에서 TraceSafe 등 가드레일 연구와 함께 운영 단계 보안의 중요한 축을 형성한다.

## 🔗 관련 논문

- 2026 04 09 who governs the machine a machine identity governa
- 2026 04 07 a systematic security evaluation of openclaw and i
- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 03 20 differential privacy in generative ai agents analy

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/ai-governance.md|ai-governance]]
- [[concepts/privilege-escalation.md|privilege-escalation]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/machine-identity-governance.md|machine-identity-governance]]

---
_LLM 분석으로 재생성됨_
