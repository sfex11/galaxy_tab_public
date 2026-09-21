# ExpBoN: Exponential-Noise Best-of-$n$ for Efficient Test-Time LLM Alignment

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-22
**링크**: http://arxiv.org/abs/2609.21899v1

## 💡 핵심 인사이트

차별적 프라이버시의 지수 노이즈 기제를 정렬로 재수출하여, 리워드-분포 이동 트레이드오프를 유한 시간 보장과 함께 연속 제어 가능한 소프트 선택 축으로 형식화했다.

## 📖 분석

## ExpBoN: 지수 노이즈 소프트 Best-of-n

ExpBoN은 추론 시점 정렬에서 하드 Best-of-n(argmax)이 리워드-분포 이동 트레이드오프를 거칠게만 제어하는 한계를 해소한다. 차별적 프라이버시의 report-noisy-max에서 유래한 지수 노이즈로 선택을 완화하여, 하드 최대화와 균등 샘플링 사이를 소프트니스 파라미터로 연속 보간하는 선택 패밀리를 제시하고 정확한 유한 시간 보장을 제공한다. 소프트 BoN의 극한 분포가 KL-정규화 리워드 최대화의 최적 분포임을 밝혀, 추론 시점 정렬의 목표 상태를 형식화한다.

### Wiki 연결

- [[distribution-internal-optimization]]: 원분포 지지 집합을 유지한 채 확률 질량만 이동시키는 표본 재가중 경로. 구조적 출력 축소와 상보적 극점이다.
- [[marginal-distribution-ceiling]]: KL 정규화 항이 사전학습 분포 천장을 암묵적 한계에서 정규화 강도로 제어되는 명시적 변수로 격상시킨다.
- [[differential-privacy]]: DP 프리미티브의 정렬 재수출 사례로, 기제의 목적 독립적 이식성을 강화한다.
- [[test-time-scaling]]: n 증가라는 양적 축에 소프트니스라는 질적 축을 추가한다.
- [[probability-quality-coupling]]: '최고 확률=품질'에서 '온도 조절 기대 리워드=품질'로 판정 기준이 이동한다.

하드 argmax에서 소프트 선택으로의 전환은 [[output-entropy-degradation]]이 훈련 시점에서 보인 다양성-리워드 긴장을 추론 시점 연속 제어로 해소하는 대응물이다.

## 🔗 관련 논문

- Beyond Truncation: Rethinking LLM Decoding as Ensemble Pruni
- A Zeroth-Order Paradigm for LLM Preference Alignment
- Escaping Mode Collapse in LLM Generation via Geometric Regul
- Vector Policy Optimization: Training for Diversity Improves 

## 🏷️ 엔티티

- [[entities/inference-time-behavior-control.md|inference-time-behavior-control]]
- [[entities/distribution-internal-optimization.md|distribution-internal-optimization]]
- [[entities/marginal-distribution-ceiling.md|marginal-distribution-ceiling]]
- [[entities/test-time-scaling.md|test-time-scaling]]
- [[entities/differential-privacy.md|differential-privacy]]
- [[entities/probability-quality-coupling.md|probability-quality-coupling]]
- [[entities/soft-best-of-n.md|soft-best-of-n]]
- [[entities/kl-regularized-reward-maximization.md|kl-regularized-reward-maximization]]
- [[entities/report-noisy-max-reuse.md|report-noisy-max-reuse]]

## 📐 개념

- [[concepts/soft-best-of-n.md|soft-best-of-n]]
- [[concepts/kl-regularized-reward-maximization.md|kl-regularized-reward-maximization]]
- [[concepts/report-noisy-max-reuse.md|report-noisy-max-reuse]]
- [[concepts/temperature-controlled-selection.md|temperature-controlled-selection]]
- [[concepts/inference-time-alignment.md|inference-time-alignment]]

---
_LLM 분석으로 생성됨_
