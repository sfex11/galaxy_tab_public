# Position: agentic AI orchestration should be Bayes-consistent

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-05
**링크**: http://arxiv.org/abs/2605.00742v1

## 💡 핵심 인사이트

LLM 추론 자체가 아닌 LLM을 구성요소로 활용하는 제어 계층(orchestration layer)이야말로 베이지안 결정 이론의 일관성 원칙이 명확히 적용되어야 하는 영역이며, 이는 algorithm-system-translation-gap에 대한 규범적 해답을 제공한다.

## 📖 분석

# Bayes-Consistent Agentic AI Orchestration

## 정의
에이전트 AI 시스템의 제어 계층(orchestration layer)이 도구 호출, 전문가 자문, 자원 할당 등 불확실성 하의 의사결정을 수행할 때 베이지안 결정 이론의 일관성 원칙을 준수해야 한다는 입장 논문. LLM 자체의 추론에서 베이지안 접근의 실용성이 불명확하더라도, LLM을 구성요소로 활용하는 제어 계층은 베이지안 원칙이 명확히 적용되는 영역임을 주장한다.

## 기존 Wiki와의 관계

이 논문은 [[entities/algorithm-system-translation-gap|algorithm-system-translation-gap]]에 대한 **규범적 해답**을 제시한다. 기존 Wiki가 이 간극을 '진단만' 기술해왔다면, 본 논문은 제어 계층이라는 구체적 좌표에서 베이지안 결정 이론이라는 잘 정립된 알고리즘적 프레임워크를 시스템 구현으로 번역하는 경로를 제공한다.

[[entities/knowledge-state-orchestration|knowledge-state-orchestration]](ADEMA)이 '지식 상태의 연속성 보장'을 구조적으로 다루었다면, 본 논문은 '불확실성 하에서의 의사결정 일관성'이라는 보완적 차원을 추가한다. ADEMA의 상태 추적이 베이지안 일관성 없이 수행되면, 상태는 추적되어도 그 상태에 기반한 행동이 규범적으로 결함될 수 있다.

[[entities/agentic-harness-engineering|agentic-harness-engineering]]의 하네스가 '관측 가능성 주도 진화'를 다룬다면, 본 논문은 하네스 설계 자체가 준수해야 할 **의사결정 이론적 기준**을 제시하여 하네스 엔지니어링의 평가 기준을 '효율성'에서 '일관성+효율성'으로 확장한다.

## 다른 논문과의 연결

- [[sources/2026-05-03-crab-a-semantics-aware-checkpointrestore-runtime-f.md|Crab]]이 의미론적 의존 그래프를 인식하는 C/R 런타임이라면, 베이지안 일관적 오케스트레이션은 복원 시점의 **의사결정 재평가**를 규범적으로 요구한다 — 과거 상태로 복원한 후 원래와 다른 행동을 선택하는 것이 베이지안 일관성 관점에서 정당한지를 사후 확률 업데이트로 판단할 수 있어야 한다.
- [[sources/2026-04-30-adema-a-knowledge-state-orchestration-architecture.md|ADEMA]]의 지식 상태 오케스트레이션이 베이지안 일관성을 내재하면, 장기 추론에서의 지식 상태 드리프트를 확률적 일관성 위반으로 정식화하여 탐지 가능해진다.
- [[sources/2026-05-02-exploration-hacking-can-llms-learn-to-resist-rl-tr.md|Exploration Hacking]]의 '기만적 자가 평가'는 베이지안 일관성 관점에서 **사후 확률의 인위적 왜곡**으로 재정형될 수 있어, 탐색 해킹 탐지에 정량적 기준을 제공할 수 있다.

## 🔗 관련 논문

- 2026-04-30-adema-a-knowledge-state-orchestration-architecture-for-long.md
- 2026-05-02-crab-a-semantics-aware-checkpointrestore-runtime-f.md
- 2026-05-02-exploration-hacking-can-llms-learn-to-resist-rl-tr.md
- 2026-04-30-agentic-harness-engineering-observability-driven-a.md
- 2026-04-30-from-soliloquy-to-agora-memory-enhanced-llm-agents-with-de.md

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/knowledge-state-orchestration.md|knowledge-state-orchestration]]
- [[entities/algorithm-system-translation-gap.md|algorithm-system-translation-gap]]
- [[entities/agentic-harness-engineering.md|agentic-harness-engineering]]
- [[entities/uncertainty-quantification.md|uncertainty-quantification]]
- [[entities/epistemic-bookkeeping.md|epistemic-bookkeeping]]
- [[entities/knowledge-state-drift.md|knowledge-state-drift]]
- [[entities/multi-agent-system.md|multi-agent-system]]

## 📐 개념

- [[concepts/bayes-consistent-agentic-orchestration.md|bayes-consistent-agentic-orchestration]]
- [[concepts/control-layer-decision-theory.md|control-layer-decision-theory]]
- [[concepts/normative-orchestration-principle.md|normative-orchestration-principle]]

---
_LLM 분석으로 생성됨_
