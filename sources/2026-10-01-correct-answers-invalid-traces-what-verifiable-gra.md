# Correct Answers, Invalid Traces: What Verifiable Grade-School Math Reveals About Chain-of-Thought Traces

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-01
**링크**: http://arxiv.org/abs/2609.38107v1

## 💡 핵심 인사이트

정답의 정확성은 추론 과정의 유효성을 담보하지 않는다 — 검증 가능한 수학에서조차 모델의 사고 흔적은 ground-truth 의존 구조와 무관하게 무효할 수 있으므로, trace 기반 디버깅·감사·추론 능력 주장은 trace 자체의 독립적 기계 검증을 전제로 해야 한다.

## 📖 분석

### Correct Answers, Invalid Traces: What Verifiable Grade-School Math Reveals About Chain-of-Thought Traces (2026-10-01)

iGSM에서 정답이 옳아도 사고 흔적(CoT trace)이 무효할 수 있음을 기계적으로 입증한다. iGSM은 정확한 수량과 의존 구조를 노출하는 합성 초등수학 벤치마크로, 자연어 trace와 달리 모델 trace를 ground-truth 의존 사슬과 대조해 유효성을 판정할 수 있게 한다.

이는 cot-as-translated-report 논제에 최초의 기계적 감사 증거를 제공한다 — 결과 신호(정답)와 과정 신호(trace)가 분리 가능하며(신규 개념 answer-trace-decoupling), 가장 유리한 조건(검증 가능한 수학·작은 탐색 공간)에서조차 실제로 분리됨이 관찰된다.

[[cot-monitorability]] 관점에서 이는 비적대적 무효성 문제다. Corrupt Plans, Clean Traces가 계획 오염 하의 흔적 세척을 보였다면 본 논문은 회피 의도 없이 정답-흔적 결합이 깨짐을 보여, trace 감시의 기본 전제가 적대성과 무관하게 재점검되어야 함을 시사한다. [[trace-integrity-faithfulness-divergence]]의 무결성-충실성 분리에 결과 수준 대응물(정답 유효성 ≠ 과정 유효성, 그 역도 비성립)을 추가한다.

방법론적으로는 verified-reasoning-trace의 실현 조건을 규정한다 — 합성 도메인 + 정확한 의존 노출이라는 최소 설계가 trace 수준 기계 검증을 가능하게 한다. legibility-interpretability-gap의 강한 형태(판독 가능하고 정답과 결합된 trace조차 무효)의 실측이며, process-reward-model 감독 데이터 품질 감사와 meaning-insensitive-metric 비판의 trace 수준 확장으로 이어진다.

## 🔗 관련 논문

- Corrupt Plans, Clean Traces: Evading Chain-of-Thought Monitoring
- Legibility is Not Interpretability: Comparing Judged and Actual Import
- When LLM Decompilers Recompile More and Preserve Less
- Necessary or Sufficient? Evaluating LLM Explanations With Behavioural

## 🏷️ 엔티티

- [[entities/igsm.md|igsm]]
- [[entities/answer-trace-decoupling.md|answer-trace-decoupling]]
- [[entities/cot-as-translated-report.md|cot-as-translated-report]]
- [[entities/cot-monitorability.md|cot-monitorability]]
- [[entities/trace-integrity-faithfulness-divergence.md|trace-integrity-faithfulness-divergence]]
- [[entities/verified-reasoning-trace.md|verified-reasoning-trace]]
- [[entities/legibility-interpretability-gap.md|legibility-interpretability-gap]]
- [[entities/meaning-insensitive-metric.md|meaning-insensitive-metric]]
- [[entities/process-reward-model.md|process-reward-model]]

## 📐 개념

- [[concepts/answer-trace-decoupling.md|answer-trace-decoupling]]
- [[concepts/cot-as-translated-report.md|cot-as-translated-report]]
- [[concepts/cot-monitorability.md|cot-monitorability]]
- [[concepts/trace-integrity-faithfulness-divergence.md|trace-integrity-faithfulness-divergence]]
- [[concepts/verified-reasoning-trace.md|verified-reasoning-trace]]
- [[concepts/single-surface-signal-insufficiency.md|single-surface-signal-insufficiency]]
- [[concepts/report-context-divergence.md|report-context-divergence]]
- [[concepts/score-narrative-conflation.md|score-narrative-conflation]]
- [[concepts/legibility-interpretability-gap.md|legibility-interpretability-gap]]
- [[concepts/meaning-insensitive-metric.md|meaning-insensitive-metric]]
- [[concepts/process-reward-model.md|process-reward-model]]

---
_LLM 분석으로 생성됨_
