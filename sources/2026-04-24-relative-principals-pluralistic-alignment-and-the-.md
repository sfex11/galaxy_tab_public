# Relative Principals, Pluralistic Alignment, and the Structural Value Alignment Problem

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-24
**링크**: http://arxiv.org/abs/2604.20805v1

## 💡 핵심 인사이트

AI 정렬의 핵심 장애는 기술적 한계가 아니라 '누가 주인인가'를 식별하지 못한 채 정렬을 설계하는 구조적 결함이며, 이는 경제학의 주인-대리인 모델로 형식화 가능한 거버넌스 문제다.

## 📖 분석

# Relative Principals, Pluralistic Alignment, and the Structural Value Alignment Problem

## 핵심 주장
AI 가치 정렬 문제를 순수 기술적·규범적 과제에서 **거버넌스 구조 문제**로 재개념화한다. 질문이 "AI가 추상적으로 정렬되었는가?"가 아니라 "충분히 정렬되었는가, 누구를 위해, 어떤 비용으로?"가 되어야 한다.

## 3차원 부정렬 모델
경제학의 **주인-대리인(principal-agent) 프레임워크**를 차용하여 부정렬을 세 독립 차원으로 분해한다:

1. **주인 식별 문제(Principal Identification)**: 누가 주인인가? — 단일 주인의 존재를 전제하는 기존 정렬 연구의 근본적 한계 노출
2. **주인 간 발산(Principal Divergence)**: 다수 주인의 가치가 충돌할 때 대리인은 누구에게 정렬되어야 하는가? — [[concepts/pluralistic-alignment|복수적 정렬]]의 형식적 근거 제공
3. **정렬 비용(Alignment Cost)**: 정렬은 결코 무료가 아니며, 비용 구조 자체가 거버넌스 결과를 결정한다

## 기존 Wiki와의 관계

### [[entities/llm-alignment|LLM 정렬]]에 대한 구조적 비판
기존 합성 분석이 RLHF·출력 필터링 등 행동 수준 방어의 한계를 지적한 것을 한 단계 더 나아가, 정렬 연구 자체의 **문제 설정이 구조적으로 불완전**함을 주장한다. 기술적 정밀도를 높여도 주인 식별·발산·비용의 구조적 차원이 해결되지 않으면 정렬은 달성될 수 없다.

### [[concepts/pluralistic-alignment|복수적 정렬]]의 이론적 기초 강화
기존 개념이 Personalized RewardBench 등에서 경험적으로 접근한 바를, 주인-대리인 모델의 주인 발산 차원으로 형식화한다. 개별 사용자 맞춤이 단지 UX 개선이 아니라 정렬의 구조적 필수조건임을 논증한다.

### [[entities/ai-governance|AI 거버넌스]]와 [[concepts/mechanism-design|메커니즘 설계]]의 통합
정렬이 거버넌스의 하위 문제가 아니라 거버넌스 자체임을 주장함으로써, 기존 거버넌스 엔티티의 범위를 근본적으로 재설정한다. 메커니즘 설계가 정렬의 핵심 도구가 된다.

### [[concepts/conflict-of-interest-in-ai|AI 내 이해상충]]과의 연결
다수 주인 간 발산은 이해상충의 근원적 형태로, 단일 모델 수준의 편향 완화가 다주인 설정에서는 구조적으로 불가능할 수 있음을 시사한다.

### [[concepts/cooperative-alignment|협력 정렬]]·[[concepts/agent-identity|에이전트 아이덴티티]]와의 교차
에이전트가 "누구에게 정렬되어 있는가"는 에이전트 아이덴티티의 사회적 차원(신뢰, 책임 귀속)과 직결된다. 다중 에이전트 협력 정렬의 전제가 되는 주인 구조 문제를 제기한다.

## 🔗 관련 논문

- Personalized RewardBench: Evaluating Reward Models with Human Preferences
- Ads in AI Chatbots? An Analysis of How Large Language Models
- Comparing Human Oversight Strategies for Computer-Use Agents

## 🏷️ 엔티티

- [[entities/llm-alignment.md|llm-alignment]]
- [[entities/ai-governance.md|ai-governance]]
- [[entities/ai-safety.md|ai-safety]]

## 📐 개념

- [[concepts/structural-value-alignment.md|structural-value-alignment]]
- [[concepts/principal-identification-problem.md|principal-identification-problem]]
- [[concepts/principal-divergence.md|principal-divergence]]
- [[concepts/alignment-cost.md|alignment-cost]]
- [[concepts/pluralistic-alignment.md|pluralistic-alignment]]
- [[concepts/mechanism-design.md|mechanism-design]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-04-24-can-ai-be-a-doctor-a-study-of-empathy-readability-]]: 둘 다 AI 정렬의 근본적 한계를 다루며, 하나는 임상 환경에서 소통적 정렬을 제3의 축으로 제시하고, 다른 하나는 정렬을 '누구를 위한 것인가'라는 거버넌스 구조 문제로 재개념화한다.
- → [[sources/2026-04-23-epistemic-orientation-in-parliamentary-discourse-i]]: 둘 다 AI 평가 방법론을 민주주의·거버넌스 문제로 확장하며, 하나는 LLM 평가로 국회 담화의 인식론적 지향성을 정량화하고, 다른 하나는 정렬 문제를 주인-대리인 거버넌스 구조로 형식화한다.
