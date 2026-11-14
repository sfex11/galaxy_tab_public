# Goal Encoding in LLMs

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-14
**링크**: http://arxiv.org/abs/2611.17297v1

## 💡 핵심 인사이트

LLM은 행동에 선행하는 목표를 희소한 어텐션 헤드에 인코딩하되 하나의 목표가 복수 실행 경로로 실현 가능하므로, 목표-행동 분리는 설계 원칙이 아니라 기계론적 실재이며 행동 관찰만으로는 목표를 판독할 수 없다.

## 📖 분석

LLM이 행동에 선행하여 목표를 내부 신경 표현으로 인코딩하는 현상의 기계론적 동정. 다중 서브태스크 코딩 설정에서 다음 서브골의 인코딩이 희소한 어텐션 헤드 집합의 출력에 국소화되고, 동일 헤드로 미래 행동을 디코딩할 수 있음이 입증되었다.

핵심은 **목표-행동 분리의 신경 수준 실재**다. 하나의 목표 인코딩이 여러 실행 경로로 실현 가능하다. 이는 [[thought-action-separation]]과 [[plan-trace-separation]]이 설계 원칙으로 제안한 분리가 모델 내부에 이미 존재하는 구조임을 입증하며, [[goal-path-underdetermination-as-harm-source]]의 기계론적 쌍대를 제공한다 — 목표가 경로를 과소결정하기에 선의의 목표도 유해 경로로 실현될 수 있다.

해석 연구 계보에서 [[causal-head-level-attribution]]이 헤드별 기능 귀속을 다뤘다면 본 논문은 그 내용이 '목표'라는 상위 인지 구조임을 특정하고, [[internal-prediction-readout]]의 대상을 미래 속성에서 미래 행동 계획으로 확장한다. [[residual-stream-length-encoding]](잔여 길이)과 함께 내부 상태가 미래 산출의 구조를 인코딩한다는 명제를 길이에서 목표로 일반화한다.

안전 함의: 목표가 잠재 공간에 있고 토큰 궤적에 직접 실현되지 않으면 [[cot-as-translated-report]] 논리가 강화되고([[unwritten-reasoning-surveillance-exclusion]]), [[pre-crime-agent-probing]] 계열 선제 감시에 목표 디코딩이라는 구체적 표적을 공급한다. 행동 관찰만으로 목표를 판독할 수 없으므로 [[alignment-base-opacity]] 감사에 내부 판독 계층이 요구되며, 판독 가능한 목표는 조향 가능한 목표라는 [[steering-read-manipulation-duality]]의 확장 여지도 연다.

## 🔗 관련 논문

- Late Attention Layers Alone Can Copy Entity Tokens, but Not Without Attention Sinks
- Pre-Crime for Agents, at the Last Second: Probing When a Recruited Agent Violates
- Corrupt Plans, Clean Traces: Evading Chain-of-Thought Monitoring
- Monitoring and Discovering Reward Hacking with Internal Representation

## 🏷️ 엔티티

- [[entities/goal-encoding.md|goal-encoding]]
- [[entities/mechanistic-interpretability.md|mechanistic-interpretability]]
- [[entities/causal-head-level-attribution.md|causal-head-level-attribution]]
- [[entities/thought-action-separation.md|thought-action-separation]]
- [[entities/plan-trace-separation.md|plan-trace-separation]]
- [[entities/internal-prediction-readout.md|internal-prediction-readout]]
- [[entities/goal-path-underdetermination-as-harm-source.md|goal-path-underdetermination-as-harm-source]]

## 📐 개념

- [[concepts/goal-action-decoupling.md|goal-action-decoupling]]
- [[concepts/cot-as-translated-report.md|cot-as-translated-report]]
- [[concepts/unwritten-reasoning-surveillance-exclusion.md|unwritten-reasoning-surveillance-exclusion]]
- [[concepts/pre-crime-agent-probing.md|pre-crime-agent-probing]]
- [[concepts/alignment-base-opacity.md|alignment-base-opacity]]
- [[concepts/residual-stream-length-encoding.md|residual-stream-length-encoding]]
- [[concepts/steering-read-manipulation-duality.md|steering-read-manipulation-duality]]

---
_LLM 분석으로 생성됨_
