# marginal-distribution-ceiling

**카테고리**: 미분류
**생성일**: 2026-05-01

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-05-01-select-to-think-unlocking-slm-potential-with-local.md|Select to Think: Unlocking SLM Potential with Local Sufficie]]

### Position-Aware Drafting for Inference Acceleration in LLM-Based Genera (2026-05-02)

타겟 분포를 변경하지 않고 추론만 가속한다는 명시적 전제를 준수하는 실제 구현 사례를 제공하여, 이 원리가 이론적 제약이 아닌 실용적 설계 원칙으로 기능함을 실증한다.

### Reliable Answers for Recurring Questions: Boosting Text-to-SQL Accurac (2026-05-03)

TeCoD가 타겟 분포를 변경하지 않고 출력 공간만 제약하여 정확도를 향상시킨다는 명시적 설계 전제를 실증 사례로 제공하여, 이 원리가 이론적 제약이 아닌 실용적 설계 원칙으로 기능함을 확인한다.

### Position-Aware Drafting for Inference Acceleration in LLM-Based Genera (2026-05-03)

position-aware drafting이 타겟 분포를 변경하지 않고 내부 구조만 인식하여 가속한다는 명시적 설계를 통해, 이 원리가 이론적 제약이 아닌 실용적 설계 원칙으로 기능함을 도메인 특화 맥락에서 재확인한다.

### SpecKV: Adaptive Speculative Decoding with Compression-Aware Gamma Sel (2026-05-05)

γ 적응이 타겟 분포를 변경하지 않는 제약 하에서 수용률을 최대화하는 구체적 구현 사례를 제공하여, 이 원칙이 이론적 제약이 아닌 실용적 설계 가이드로 기능함을 추가적으로 실증한다.

### EMO: Pretraining Mixture of Experts for Emergent Modularity (2026-05-10)

도메인별 전문가 부분집합만으로 추론할 때 해당 도메인의 P(y)가 보존되어야 한다는 조건을 사전학습에서 구조적으로 달성하는 실제 경로를 제공한다. 기존에 '분포 보존이 필요하다'는 원칙만 존재했다면, EMO는 전문가 조직 설계가 어떻게 P(y)의 도메인별 분해를 가능하게 하는지를 메커니즘 수준에서 구체화한다.

### Can RL Teach Long-Horizon Reasoning to LLMs? Expressiveness Is Key (2026-05-10)

표현력 한계가 P(y)의 구조적 특성으로 귀인됨을 실증하여, 성능 천장의 원인을 '사전학습 데이터 양'이 아닌 '학습된 표현 체계의 논리적 표현력'으로 확장한다.

### Post-Training Language Models for Gold-Medal Performance in Coding Com (2026-09-04)

Nano(SFT+RL) vs Ultra(SFT만)의 대조를 통해, 사전학습 주변 분포의 상한이 높은 대형 모델은 조건부 SFT만으로 상한 근접이 가능하지만 소형 모델은 RL이 상한 접근을 촉진해야 한다는 스케일 의존적 구조를 실증한다.

### Unlocking Lossless Speedups in LLMs via Discrete Diffusion (2026-09-06)

AR 가중치를 표준 NTP 목적함수로 그대로 학습함으로써 주변 분포 P(y)의 지형을 보존하고, 병렬화 가속이 조건부 최적화의 성능 상한선을 훼손하지 않음을 설계 수준에서 보장하는 실증 사례를 제공한다.

### Distill Globally, Adapt Locally: Reasoning Distillation and Product-Ty (2026-09-08)

교사 LLM의 추론 품질이 증류 학생의 성능 천장을 규정하는 구조를 제공한다 — P(y)→P(y|x) 천장 개념이 교사-학생 증류 관계로 확장되며, 증류는 천장을 돌파하는 것이 아니라 천장을 학생에게 최대한 이전하는 작업임을 시사한다.

→ [[sources/2026-09-08-distill-globally-adapt-locally-reasoning-distillat.md|상세 보기]]

### Don't Drop Dropout: Optimizing Layer Sparsity for Efficient LLM Traini (2026-09-08)

Layer dropout이 사전학습 분포 P(y)의 형성 자체를 수정하면서도 정확도 저하를 완화 가능함을 보여, P(y)의 형상화에 설계 자유도가 스케일링 관행이 가정한 것보다 크다는 증거를 제공한다. 정규화가 일반화 수단을 넘어 P(y)의 추론 옵션을 결정하는 매개변수로 재해석된다.

→ [[sources/2026-09-08-dont-drop-dropout-optimizing-layer-sparsity-for-ef.md|상세 보기]]
