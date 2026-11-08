# On the Fundamental Limits of Prefill-Based Decoding Length Prediction

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-02
**링크**: http://arxiv.org/abs/2610.40541v1

## 💡 핵심 인사이트

길이 예측의 정확도 한계는 예측기의 결함이 아니라 자기회귀 디코딩의 내재적 확률성이 규정하는 이론적 하한이며, 벤치마크 수치는 타겟 구성에 조건부라 교차 구성 비교로는 예측기 품질을 측정할 수 없다.

## 📖 분석

프리필 단계 은닉 상태만으로 디코딩 길이를 예측하는 원시 연산의 근본 한계를 규명한다. 세 가지 발견: (1) 기존 벤치마크는 예측기 품질과 태스크 난이도를 혼동한다 — 타겟 모델·데이터셋·샘플링 구성이 바뀌면 예측기가 동일해도 보고된 정확도가 붕괴한다([[concepts/predictor-hardness-conflation.md|predictor hardness conflation]]). (2) 이 불안정성의 원천은 자기회귀 디코딩의 내재적 확률성이며, 이것이 부과하는 엔트로피 하한 아래로 예측 오차는 내려갈 수 없다([[concepts/decoding-stochasticity-bound.md|decoding stochasticity bound]]). (3) 따라서 정확도 수치는 타겟 구성에 조건부이며, 교차 구성 비교는 예측기 품질을 측정하지 못한다. 이는 [[concepts/predictability-driven-serving.md|predictability driven serving]]의 Pythia 계보에 이론적 보정을 제공한다 — 스케줄링용 길이 예측([[concepts/prefill-length-prediction.md|prefill length prediction]])은 확률성 천장 아래에서만 유효하므로, 서빙 설계는 벤치마크 수치가 아닌 이론적 하한과 조건부 유효 범위를 기준으로 삼아야 한다. 에이전트 실행 수준의 [[concepts/token-consumption-forecasting.md|token consumption forecasting]](TokenCast)과 결합하면, 미시(디코딩 길이)와 거시(실행 전체) 예측이 동일한 AR 확률성 근원에서 서로 다른 불확실성 계층을 상속함을 시사한다. 벤치마크 혼동 문제는 [[concepts/benchmark-specification-gap.md|benchmark specification gap]] 계열의 측정 타당성 문제이자, [[concepts/same-request-same-reading-assumption.md|same request same reading assumption]]의 디코딩 수준 확장 — 샘플링 구성 변경이 곧 판독값 변경이다 — 로 읽힌다.

## 🔗 관련 논문

- TokenCast: Forecasting Token Consumption During LLM Agent Ex
- Pythia: Toward Predictability-Driven Agent-Native LLM Servin
- Measuring the Serving Stack Instead of the Model: Hidden Con

## 🏷️ 엔티티

- [[entities/predictor-hardness-conflation.md|predictor-hardness-conflation]]
- [[entities/decoding-stochasticity-bound.md|decoding-stochasticity-bound]]
- [[entities/prefill-length-prediction.md|prefill-length-prediction]]
- [[entities/predictability-driven-serving.md|predictability-driven-serving]]
- [[entities/token-consumption-forecasting.md|token-consumption-forecasting]]
- [[entities/residual-stream-length-encoding.md|residual-stream-length-encoding]]
- [[entities/benchmark-specification-gap.md|benchmark-specification-gap]]
- [[entities/same-request-same-reading-assumption.md|same-request-same-reading-assumption]]
- [[entities/internal-prediction-readout.md|internal-prediction-readout]]

## 📐 개념

- [[concepts/predictor-hardness-conflation.md|predictor-hardness-conflation]]
- [[concepts/decoding-stochasticity-bound.md|decoding-stochasticity-bound]]
- [[concepts/prefill-length-prediction.md|prefill-length-prediction]]
- [[concepts/residual-stream-length-encoding.md|residual-stream-length-encoding]]

---
_LLM 분석으로 생성됨_
