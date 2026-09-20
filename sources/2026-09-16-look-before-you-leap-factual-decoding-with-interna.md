# Look Before You Leap: Factual Decoding with Internal Attribution Signals

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-16
**링크**: http://arxiv.org/abs/2609.15745v1

## 💡 핵심 인사이트

환각 개입의 제3 위치 — 사후 교정과 가중치 개입 사이의 '디코딩 중 선제 억제' — 를 열고, 제어 근거를 슬라이딩 윈도우 MLP 어블레이션으로 식별한 내부 귀속 신호에서 획득함으로써 초기 오류의 눈덩이 복합화를 생성 완료 전에 차단한다.

## 📖 분석

DescaPE(DEcoding Signal Control Against Path Error-snowballing)는 환각 대응의 제3 축을 연다. 사후 교정(post-hoc correction)과 가중치 수준 개입(weight-level intervention) 어느 쪽도 자기회귀 생성에서 초기 사실 오류가 눈덩이처럼 복합화되는 것을 선제 차단하지 못한다는 진단 위에서, 디코딩 시점에 내부 귀속 신호로 환각 유발 궤적을 억제하는 프레임워크를 제안한다.

Wiki 축적 지형과의 관계: (1) [[entities/multi-signal-hallucination-detection.md|multi signal hallucination detection]](Domain-Specific Hallucination Detection)이 분류기·불확실성·보정 3신호로 '생성 완료 후' 환각을 감지했다면, 본 논문은 개입 시점을 '생성 중'으로 이동시켜 환각 개입의 사후 감지—선제 억제 이중 구조를 완성한다. (2) [[concepts/unrecoverable-reasoning-error.md|unrecoverable reasoning error]]이 규정한 '초기 오류의 자기회귀적 복합화로 사후 복구 불가' 실패 모드에 대한 최초의 디코딩 수준 처방이 된다. (3) 슬라이딩 윈도우 MLP 어블레이션은 [[concepts/causal-mechanistic-interpretability.md|causal mechanistic interpretability]]의 개입 실험을 해석 도구에서 디코딩 제어기의 근거 신호로 전환한다. (4) [[concepts/intra-generative-intervention.md|intra generative intervention]]의 '토큰 생성 중 실시간 개입' 패러다임을 사실 정확성 도메인에서 구현하며, [[concepts/residual-stream-monitoring.md|residual stream monitoring]]과 [[concepts/inference-time-behavior-control.md|inference time behavior control]]이 개척한 내부 신호 기반 추론 시점 개입 계열에 환각 억제라는 새 응용 축을 추가한다.

## 🔗 관련 논문

- Domain-Specific Hallucination Detection in Large Language Models
- MoRFI: Monotonic Sparse Autoencoder Feature Identification
- It's Not RoPE that Creates Sinks: The Role of Self-Concentration

## 🏷️ 엔티티

- [[entities/multi-signal-hallucination-detection.md|multi-signal-hallucination-detection]]
- [[entities/closed-book-qa-hallucination.md|closed-book-qa-hallucination]]
- [[entities/inference-time-behavior-control.md|inference-time-behavior-control]]
- [[entities/residual-stream-monitoring.md|residual-stream-monitoring]]
- [[entities/causal-mechanistic-interpretability.md|causal-mechanistic-interpretability]]

## 📐 개념

- [[concepts/unrecoverable-reasoning-error.md|unrecoverable-reasoning-error]]
- [[concepts/intra-generative-intervention.md|intra-generative-intervention]]
- [[concepts/response-level-hallucination-detection.md|response-level-hallucination-detection]]
- [[concepts/detector-as-instrument.md|detector-as-instrument]]
- [[concepts/temperature-scaled-calibration.md|temperature-scaled-calibration]]

---
_LLM 분석으로 생성됨_
