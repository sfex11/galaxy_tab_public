# Don't Drop Dropout: Optimizing Layer Sparsity for Efficient LLM Training and Inference

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-08
**링크**: http://arxiv.org/abs/2609.05275v1

## 💡 핵심 인사이트

모델의 깊이 탄력성은 자연 부여가 아니라 사전학습 레시피가 창출하는 속성이며 — layer dropout은 훈련 시점 정규화를 추론 시점 zero-shot 프루닝 유연성으로 전환하고, 스케일링 시대의 dropout 기각은 정량화되지 않은 가정에 기반한 관행이었음을 폭로한다.

## 📖 분석

## 분석

본 논문은 layer dropout(stochastic depth)이 LLM 사전학습 레시피에서 소멸한 것이 정량화되지 않은 가정에 기반함을 진단하고, 계층별 희소성 최적화를 통해 훈련 가속·정확도 보존·프루닝 견고성을 동시에 달성할 수 있음을 보인다.

### 기존 Wiki 내 위치

[[model-compression]] 축에서 새로운 위치를 점유한다. 기존 압축 연구가 post-training(양자화, 증류, 프루닝) 중심으로 전개되어 왔다면, 본 논문은 '사전학습 시점에 프루닝 가능한 모델을 만들어내는' 경로를 연다. Layer dropout은 훈련 기법이지만 그 실질 가치는 추론 시점에 실현된다 — 재훈련 없이 계층을 제거하는 elastic depth 추론이라는 [[model-pruning]]의 새로운 전제다.

[[adaptive-inference]] 관점에서도 새로운 적응 축이 추가된다. SpecKV의 압축률 반응과 CADENCE의 컨텍스트 반응은 모두 고정 아키텍처 내부에서 작동했으나, 계층 수준 탄력성은 아키텍처 깊이 선택 자체를 가능하게 한다.

[[knowledge-distillation]]과의 대조도 중요하다. TIDE류 증류는 소형 모델로의 전이에 재훈련을 요구하지만, layer dropout은 '재훈련 없이, 하나의 모델로 다중 깊이'를 제공한다. 이는 [[post-training]] 논의와 공명한다 — 일부 능력(탄력성)은 사후 추가가 아니라 사전학습에 내장되어야 한다는 교훈이다.

### 핵심

모델의 깊이 탄력성은 자연 부여가 아니라 사전학습 레시피가 창출하는 속성이다. dropout의 소멸은 정량화되지 않은 가정에 기반한 스케일링 관행이었으며, 이를 정량화함으로써 훈련 시점 정규화가 추론 시점 유연성으로 전환된다.

## 🔗 관련 논문

- Carbon-Taxed Transformers: A Green Compression Pipeline for
- Turning the TIDE: Cross-Architecture Distillation for Diffus
- Unlocking Lossless Speedups in LLMs via Discrete Diffusion

## 🏷️ 엔티티

- [[entities/model-compression.md|model-compression]]
- [[entities/model-pruning.md|model-pruning]]
- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/on-device-inference.md|on-device-inference]]
- [[entities/marginal-distribution-ceiling.md|marginal-distribution-ceiling]]
- [[entities/layer-dropout.md|layer-dropout]]

## 📐 개념

- [[concepts/stochastic-depth.md|stochastic-depth]]
- [[concepts/zero-shot-layer-pruning.md|zero-shot-layer-pruning]]
- [[concepts/elastic-depth-inference.md|elastic-depth-inference]]

---
_LLM 분석으로 생성됨_
