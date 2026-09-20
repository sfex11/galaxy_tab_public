# An Empirical Study of Harness Design for Coding Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-19
**링크**: http://arxiv.org/abs/2609.20804v1

## 💡 핵심 인사이트

하네스는 모놀리식 시스템이 아니라 계획·행동 공간·컨텍스트 관리로 분해 가능한 구성요소의 조합이며, 실행 루프를 고정한 구성요소 어블레이션만이 각 요소의 기여도를 인과적으로 분리할 수 있다.

## 📖 분석

# 하네스 구성요소 분해 실증 (Harness Design for Coding Agents)

실행 루프를 고정한 채 계획(planning)·행동 공간(action space)·컨텍스트 관리(context management)의 3구성요소만 변이시켜 각각의 기여도를 분리 측정하는 통제 실험적 하네스 연구다. 기존 평가가 하네스를 모놀리식 시스템으로 다뤄 구성요소별 효과를 알 수 없었던 공백을 채운다.

**Wiki에서의 위치**:
- [[concepts/harness-design-combinatorics.md|harness design combinatorics]]의 '하네스=독립 차원의 조합' 관점에 첫 실증적 토대를 제공한다. 추상적 차원 구분을 계획·행동공간·컨텍스트라는 조작적 축으로 구체화한다.
- [[concepts/harness-as-hidden-variable.md|harness as hidden variable]]을 관측 가능하게 만든다. 전체 성능 비교를 벗어나 구성요소 수준 어블레이션으로 하네스의 성능 기여 구조를 노출한다.
- [[concepts/model-harness-decomposability.md|model harness decomposability]]에 데이터를 공급한다. 4개 모델에서 동일 변이를 반복함으로써 하네스 효과가 이식 가능한 설계 원칙인지 모델 조건부인지 판별 가능해진다.
- [[concepts/component-independence-assumption.md|component independence assumption]]의 직접 검증 무대 — 구성요소 간 상호작용(예: 넓은 행동 공간이 컨텍스트 관리 부담을 증폭)의 존재를 측정한다.

**연결점**: "Coding Agents Have Converged"(2026-09-17)가 모델 성능 수렴을 보였다면, 본 논문은 수렴 후 잔여 차이의 원천이 하네스 구성에 있음을 정량화한다. [[concepts/harness-task-matching-bottleneck.md|harness task matching bottleneck]]의 '작업별 하네스 구성 선택이 병목' 주장에 경험적 근거를 부여하며, Crab이 실행 환경 계층([[concepts/semantics-aware-checkpoint.md|semantics aware checkpoint]])을 다뤘다면 본 논문은 에이전트 루프 설계 계층을 다룬다.

**새 개념**: fixed-loop-component-ablation — 루프를 불변량으로 고정하고 구성요소만 변이해 인과적 기여도를 추정하는 하네스 실험 방법론. 관측성 기반 자동 진화([[concepts/observability-driven-evolution.md|observability driven evolution]])가 '어떻게 개선할까'였다면, 이는 '무엇이 중요한가'를 먼저 답하는 진단 계층이다.

## 🔗 관련 논문

- Coding Agents Have Converged: Why the SWE Bench Leaderboards Are Flattening (2026-09-17)
- Agentic Harness Engineering: Observability-Driven Automatic Evolution (2026-04-30)
- From Model Scaling to System Scaling: Scaling the Harness in the Loop (2026-05-27)
- Crab: A Semantics-Aware Checkpoint/Restore Runtime for Agent Sandboxes (2026-05-02)
- ClawGym: A Scalable Framework for Building Effective Claw Agents (2026-05-01)

## 🏷️ 엔티티

- [[entities/harness-engineering.md|harness-engineering]]
- [[entities/agentic-harness-engineering.md|agentic-harness-engineering]]
- [[entities/system-scaling.md|system-scaling]]

## 📐 개념

- [[concepts/harness-design-combinatorics.md|harness-design-combinatorics]]
- [[concepts/harness-as-hidden-variable.md|harness-as-hidden-variable]]
- [[concepts/model-harness-decomposability.md|model-harness-decomposability]]
- [[concepts/component-independence-assumption.md|component-independence-assumption]]
- [[concepts/harness-task-matching-bottleneck.md|harness-task-matching-bottleneck]]
- [[concepts/fixed-loop-component-ablation.md|fixed-loop-component-ablation]]

---
_LLM 분석으로 생성됨_
