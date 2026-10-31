# On the Fundamental Limits of Prefill-Based Decoding Length Prediction

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-31
**링크**: http://arxiv.org/abs/2610.40541v1

## 💡 핵심 인사이트

자회귀 디코딩의 내재적 확률성이 길이 예측에 제거 불가능한 엔트로피 하한을 부과하므로, 예측 정확도 벤치마크는 예측기 품질이 아니라 태스크 구성의 난이도를 측정한다.

## 📖 분석

프리필 단계 은닉 상태만으로 LLM의 디코딩 길이를 예측하는 문제를 추론 스케줄링([[predictability-driven-serving]], [[aggregate-pipeline-serving]])의 핵심 프리미티브로 다루며, 기존 벤치마크의 구조적 결함과 예측의 근본 한계를 동시에 규명한다.

핵심 발견은 두 가지다. 첫째, 벤치마크가 예측기 품질과 태스크 난이도를 혼동한다 — 타겟 모델·데이터셋·샘플링 구성이 바뀌면 동일 예측기의 정확도가 붕괴하므로 교차 구성 비교는 예측기 품질을 측정하지 못한다([[matched-condition-comparison]], [[benchmark-specification-gap]]). 둘째, 이 불안정성의 근원은 자회귀 디코딩([[autoregressive-generation]])의 내재적 확률성이다 — 디코딩 길이는 프롬프트의 결정론적 함수가 아니라 샘플링 분포 위의 확률 변수이며, 예측 오차에는 제거 불가능한 엔트로피 하한이 존재한다.

이는 토큰 소비 예측([[token-consumption-forecasting]])과 예측가능성 기반 서빙([[predictability-driven-serving]])에 근본 한계 차원의 보정을 제공한다. 프리필 상태 판독이라는 점에서 [[residual-stream-length-encoding]]·[[internal-prediction-readout]] 계보에 속하며, 에이전트 내부의 [[complexity-meta-cognition]]과 대비되는 시스템 측 외부 판독 경로를 형성한다. [[same-request-same-reading-assumption]] 계열이 계측기 측 불안정성을 다뤘다면 본 논문은 측정 대상 자체의 확률성이 만드는 한계를 정식화하여 측정 불확실성 논의의 양축을 완성한다. [[adaptive-inference]]와 [[speculation-length-adaptation]]의 설계는 벤치마크 수치가 아닌 이론적 하한을 기준으로 재평가되어야 한다.

## 🔗 관련 논문

- TokenCast: Forecasting Token Consumption During LLM Agent Execution
- Pythia: Toward Predictability-Driven Agent-Native LLM Serving
- Measuring the Serving Stack Instead of the Model: Hidden Confounds

## 🏷️ 엔티티

- [[entities/token-consumption-forecasting.md|token-consumption-forecasting]]
- [[entities/predictability-driven-serving.md|predictability-driven-serving]]
- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/aggregate-pipeline-serving.md|aggregate-pipeline-serving]]
- [[entities/benchmark-specification-gap.md|benchmark-specification-gap]]
- [[entities/matched-condition-comparison.md|matched-condition-comparison]]
- [[entities/same-request-same-reading-assumption.md|same-request-same-reading-assumption]]
- [[entities/residual-stream-length-encoding.md|residual-stream-length-encoding]]
- [[entities/internal-prediction-readout.md|internal-prediction-readout]]
- [[entities/decoding-stochasticity-bound.md|decoding-stochasticity-bound]]
- [[entities/predictor-hardness-conflation.md|predictor-hardness-conflation]]
- [[entities/prefill-length-prediction.md|prefill-length-prediction]]

## 📐 개념

- [[concepts/decoding-stochasticity-bound.md|decoding-stochasticity-bound]]
- [[concepts/predictor-hardness-conflation.md|predictor-hardness-conflation]]
- [[concepts/prefill-length-prediction.md|prefill-length-prediction]]
- [[concepts/benchmark-specification-gap.md|benchmark-specification-gap]]
- [[concepts/matched-condition-comparison.md|matched-condition-comparison]]
- [[concepts/same-request-same-reading-assumption.md|same-request-same-reading-assumption]]
- [[concepts/residual-stream-length-encoding.md|residual-stream-length-encoding]]
- [[concepts/internal-prediction-readout.md|internal-prediction-readout]]
- [[concepts/autoregressive-generation.md|autoregressive-generation]]
- [[concepts/speculation-length-adaptation.md|speculation-length-adaptation]]
- [[concepts/adaptive-inference.md|adaptive-inference]]
- [[concepts/complexity-meta-cognition.md|complexity-meta-cognition]]
- [[concepts/decode-phase-gemv-serving-cost.md|decode-phase-gemv-serving-cost]]

---
_LLM 분석으로 생성됨_
