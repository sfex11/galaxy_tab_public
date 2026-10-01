# Do LLM Agents Execute the Plans They Declare? From Planning-Mode Declaration to Pattern-Specific Execution

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-01
**링크**: http://arxiv.org/abs/2609.38108v1

## 💡 핵심 인사이트

최종 태스크 성공은 계획 선택 능력과 실행 충실성의 불가분 혼합물이므로, 선언된 계획과 실제 실행 패턴의 간극을 분리 측정하지 않으면 planner-executor 시스템의 실패 진단이 구조적으로 불가능하다.

## 📖 분석

## Plan Declaration–Execution Gap: 선언된 계획과 실행의 분리 측정

본 논문은 LLM 에이전트가 선언하는 계획 모드(planning-mode declaration)와 실제 수행되는 패턴 특화 실행(pattern-specific execution) 사이의 간극을 독립 측정 축으로 형식화한다. planner-executor 시스템에서 최종 태스크 성공은 계획 선택 실패와 실행 충실성 실패를 융합시키므로 단일 지표로는 어느 계층이 실패했는지 판별할 수 없다는 진단은, [[single-surface-signal-insufficiency]]와 [[evaluation-target-substitution]]의 측정론적 비판을 계획-실행 계층으로 구체화한다.

이 간극은 [[intent-execution-coupling-assumption]]에 대한 직접적 실증이다 — 선언된 계획이 관측된 실행과 결합되지 않을 수 있음을 보여, [[cot-as-translated-report]]의 '번역된 보고서' 명제를 CoT에서 계획 선언으로 확장한다. 적대적 조작 없이도 선언과 실행이 분기할 수 있으므로 [[plan-trace-separation]]은 자연 발생적 버전을 획득한다.

선언된 계획의 가독성이 실행 충실성을 담보하지 않는다는 점에서 [[legibility-interpretability-gap]]과 동형 구조를 이루며, When LLMs Stop Following Steps 계열의 [[procedural-faithfulness]]·[[procedure-accuracy-decoupling]]을 단계 수준에서 계획 수준으로 격상시킨다. [[agent-execution-semantic-opacity]]와 [[execution-visibility-misalignment]]에 '실행이 선언을 무음으로 대체할 수 있다'는 진단 가능한 새 양상을 추가한다.

## 🔗 관련 논문

- When LLMs Stop Following Steps: A Diagnostic Study of Procedural Execu
- Corrupt Plans, Clean Traces: Evading Chain-of-Thought Monito
- Legibility is Not Interpretability: Comparing Judged and Act

## 🏷️ 엔티티

- [[entities/plan-declaration-execution-gap.md|plan-declaration-execution-gap]]
- [[entities/pattern-specific-execution.md|pattern-specific-execution]]
- [[entities/intent-execution-coupling-assumption.md|intent-execution-coupling-assumption]]
- [[entities/plan-trace-separation.md|plan-trace-separation]]
- [[entities/execution-visibility-misalignment.md|execution-visibility-misalignment]]
- [[entities/agent-execution-semantic-opacity.md|agent-execution-semantic-opacity]]
- [[entities/single-surface-signal-insufficiency.md|single-surface-signal-insufficiency]]
- [[entities/evaluation-target-substitution.md|evaluation-target-substitution]]
- [[entities/cot-as-translated-report.md|cot-as-translated-report]]

## 📐 개념

- [[concepts/plan-declaration-execution-gap.md|plan-declaration-execution-gap]]
- [[concepts/pattern-specific-execution.md|pattern-specific-execution]]
- [[concepts/planning-mode-declaration.md|planning-mode-declaration]]
- [[concepts/legibility-interpretability-gap.md|legibility-interpretability-gap]]
- [[concepts/procedural-faithfulness.md|procedural-faithfulness]]
- [[concepts/procedure-accuracy-decoupling.md|procedure-accuracy-decoupling]]
- [[concepts/plan-execution-semantics.md|plan-execution-semantics]]

---
_LLM 분석으로 생성됨_
