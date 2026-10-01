# Probability is Not Enough: Exploring and Counting Divergent Tokens for Reasoning Uncertainty Quantification in LLMs

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-01
**링크**: http://arxiv.org/abs/2609.38070v1

## 💡 핵심 인사이트

CoT 신뢰도의 근거는 핵심 토큰의 확률값이 아니라 추론 궤적이 기준 경로에서 이탈하는 구조(발산 토큰의 계수)에 있으며, 신뢰도 추정기의 확률 전제는 개입 실험으로 검증되어야 한다.

## 📖 분석

2026-10-01 발표된 본 논문은 CoT 신뢰도 추정의 표준 접근 — 선별된 핵심 토큰의 확률 — 에 대해 '확률은 충분하지 않다'는 진단을 내린다. 파일럿 연구에서 선택된 토큰 확률을 조악한 대체물로 교체·교란하는 개입 실험을 통해, 확률값 자체가 신뢰도 신호의 결정적 운반체가 아님을 확인하고, 대신 추론 궤적을 탐색하여 기준 경로에서 이탈하는 발산 토큰(divergent tokens)의 존재·빈도를 계수하는 구조적 신호로 불확실성 정량화를 재설계한다.

Wiki 관점에서 이 논문은 [[probability-quality-coupling]]의 균열을 신뢰도 추정 도메인에서 실증하고, 판정 신호의 확률 외부 이동([[extra-probabilistic-adjudication]])을 답변 판정에서 계측기 차원으로 확장한다. 개입으로 신호의 인과적 기여를 검증하는 파일럿 설계는 [[causal-load-verification]]의 방법론을 사후 감지 도메인으로 이식한 사례다. [[temperature-scaled-calibration]]·[[multi-signal-hallucination-detection]] 계열이 확률 기반 보정과 다중 신호 결합을 다뤘다면, 본 논문은 그 전제인 확률의 위상 자체를 재검토하는 상위 축을 제공한다. 탐색-계수 접근은 [[soft-best-of-n]]·[[concept-conditioned-sampling]]의 테스트타임 샘플링과 신뢰도 추정이 수렴하는 지점을, 발산 분포 판독은 [[score-distributional-confidence]]의 스코어 분포 판독이 검색에서 생성 궤적으로 확장되는 흐름을 보여준다.

## 🔗 관련 논문

- Predictable Failure in Multi-Hop Retrieval: Score-Distributional Confidence
- Domain-Specific Hallucination Detection in Large Language Models
- Beyond Repeated Sampling: Learning Search Policies for LLM Reasoning

## 🏷️ 엔티티

- [[entities/uncertainty-quantification.md|uncertainty-quantification]]
- [[entities/probability-quality-coupling.md|probability-quality-coupling]]
- [[entities/extra-probabilistic-adjudication.md|extra-probabilistic-adjudication]]
- [[entities/causal-load-verification.md|causal-load-verification]]
- [[entities/temperature-scaled-calibration.md|temperature-scaled-calibration]]
- [[entities/multi-signal-hallucination-detection.md|multi-signal-hallucination-detection]]
- [[entities/score-distributional-confidence.md|score-distributional-confidence]]
- [[entities/soft-best-of-n.md|soft-best-of-n]]
- [[entities/concept-conditioned-sampling.md|concept-conditioned-sampling]]
- [[entities/detector-as-instrument.md|detector-as-instrument]]
- [[entities/divergent-token-counting.md|divergent-token-counting]]

## 📐 개념

- [[concepts/uncertainty-underestimation.md|uncertainty-underestimation]]
- [[concepts/reasoning-chain.md|reasoning-chain]]
- [[concepts/cot-as-translated-report.md|cot-as-translated-report]]
- [[concepts/confidence-consistency-decoupling.md|confidence-consistency-decoupling]]
- [[concepts/uncertainty-quantification.md|uncertainty-quantification]]
- [[concepts/probability-quality-coupling.md|probability-quality-coupling]]
- [[concepts/extra-probabilistic-adjudication.md|extra-probabilistic-adjudication]]
- [[concepts/causal-load-verification.md|causal-load-verification]]

---
_LLM 분석으로 생성됨_
