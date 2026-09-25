# Shopping by algorithm: How agentic AI deploys human heuristics as a surrogate consumer

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-25
**링크**: http://arxiv.org/abs/2609.28372v1

## 💡 핵심 인사이트

AI 위임은 인간 편향을 제거하지 않는다 — 상용 LLM이 대리 소비자로서 마케팅 가격 큐에 대한 인간형 휴리스틱 감수성을 보이며, 도구 호출 비용이 그 발현 조건을 결정한다.

## 📖 분석

# Shopping by Algorithm: 대리 소비자로서의 에이전틱 AI (2026-09-25)

소비자가 LLM에 구매 결정을 위임하는 '대리 소비자' 설정을 통제 실험으로 분석한 논문. 정보판 프로세스 트레이싱을 에이전틱 환경에 이식한 Tool-Lab은 제품 속성을 비용 있는 도구 호출 뒤에 배치하여 선택 전 정보 획득 과정을 관찰 가능하게 만든다. 3개 공급자의 8개 상용 LLM에서 가격 큐(just-below pricing, promotional framing)가 에이전트의 정보 획득과 선택에 미치는 영향을 추적하며, 도구 호출 비용이 휴리스틱 발현을 조절하는 조건 변수로 작동함을 보인다.

## 기존 Wiki와의 관계

**[[value-sensitive-delegation]]**: OpenClaw 야생 데이터가 일상 위임의 가치 분포를 관찰했다면, 본 논문은 가장 밀도 높은 위임 도메인(구매)의 통제 실험 버전을 제공한다. 위임된 결정이 사용자 선호가 아닌 에이전트 내재 휴리스틱을 따를 수 있어 가치 침해의 인과적 메커니즘 후보를 추가한다.

**[[choice-architecture]]**: Mecha-nudges가 기계 대상 뉘지를 개념화했다면, 본 논문은 마케팅 큐라는 구체적 뉘지가 AI 쇼핑 에이전트에 실제로 작동함을 실증한다. 인간 소비자를 겨냥해 설계된 선택 아키텍처가 AI 매개 구매로 전이됨을 보여준다.

**[[expected-value-of-information]]**: Tool-Lab은 정보 수집 판단에 명시적 비용 구조를 부여한 실험적 EVI 테스트베드다. 도구 호출 비용이 정보 획득 전략과 휴리스틱 의존도를 동시에 변화시켜, [[cost-aware-agent-evaluation]]의 비용 축이 능력 진단 도구로도 기능할 수 있음을 시사한다.

**새 축 — 인간 휴리스틱 계승**: LLM이 인간 생성 텍스트 학습의 산물로서 인간 의사결정 휴리스틱을 결정에 배치하면, [[autonomous-commerce]]에서 에이전트가 편향을 교정하지 않고 재생산할 수 있다. AI 위임 연구가 능력 문제에서 행동 경제학 문제로 확장되는 전환점이다.

## 🔗 관련 논문

- Value-Sensitive Delegation in Everyday AI Agent Use: Evidence from OpenClaw
- Does AI Save Time on Product Design? A Randomized Controlled Experiment
- Understanding Operator Attitudes Toward AI-Supported Decision Making

## 🏷️ 엔티티

- [[entities/surrogate-consumer-agent.md|surrogate-consumer-agent]]
- [[entities/tool-lab-process-tracing.md|tool-lab-process-tracing]]
- [[entities/human-heuristic-inheritance.md|human-heuristic-inheritance]]
- [[entities/pricing-cue-susceptibility.md|pricing-cue-susceptibility]]
- [[entities/value-sensitive-delegation.md|value-sensitive-delegation]]
- [[entities/choice-architecture.md|choice-architecture]]
- [[entities/expected-value-of-information.md|expected-value-of-information]]
- [[entities/autonomous-commerce.md|autonomous-commerce]]
- [[entities/cost-aware-agent-evaluation.md|cost-aware-agent-evaluation]]
- [[entities/persuasion-openness.md|persuasion-openness]]
- [[entities/ai-decision-making.md|ai-decision-making]]

## 📐 개념

- [[concepts/delegation-bias-reproduction.md|delegation-bias-reproduction]]
- [[concepts/surrogate-consumer-agency.md|surrogate-consumer-agency]]
- [[concepts/cost-conditioned-heuristic-expression.md|cost-conditioned-heuristic-expression]]
- [[concepts/information-board-process-tracing-agentification.md|information-board-process-tracing-agentification]]

---
_LLM 분석으로 생성됨_
