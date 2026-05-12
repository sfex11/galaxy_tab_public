# Flow-OPD: On-Policy Distillation for Flow Matching Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-12
**링크**: http://arxiv.org/abs/2605.08063v1

## 💡 핵심 인사이트

보상 해킹이 출력 공간의 회피가 아니라 메트릭 간 경쟁적 시소 효과(seesaw effect)로 나타난다는 발견은, 보상 해킹을 '모델이 환경을 속이려 기만하는 행위'에서 '보상 지형 자체가 불안정한 행위'로 재정의하게 한다.

## 📖 분석

# Flow-OPD: On-Policy Distillation for Flow Matching Models


## 핵심 기여

기존에 자회귀 언어 모델에서 성공한 On-Policy Distillation (OPD)을 연속적 생성 모델인 Flow Matching (FM) 텍스트-톨이미지 모델로 최초로 확장한 논문이다. 다중 태스크 정렬에서 발생하는 두 가지 근본적 병목—스칼라 보상의 희소성(reward sparsity)와 이질적 목표 간 기울기 간섭(gradient interference)—을 문제 진단하고, 이들이 연속 생성 아키텍처에서 '시소 효과 시소 효과'가 경쟁하는 **시소 효과 효과(seesaw effect)**를 최초로 형식화한다.

## 기존 Wiki와의 관계

on-policy-distillation은 기존에 자회귀 LLM의 사후학습 기법으로만 기술되어 있었다. Flow-OPD는 이를 연속 생성 패러다임으로 확장함으로써, post-training이 모델 아키텍처 의존적이라는 암묵적 전제를 해체한다. 특히 diffusion-model 계열의 사후학습에서 reward-hacking이 출력 공간 회피가 아닌 메트릭 간 경쟁적 시소 효과로 현현한다는 점은, 기존 보상 해킹이 자회귀 모델의 텍스트 생성에서 어떻게 나타나는지와 흥미로운 대조를 이룬다.

multi-objective-optimization에서 문제시되던 기울기 간섭이 연속 생성에서는 위상 공간(latent space)에서 은밀하게 관찰될 수 있음을 시사하며, cascade-reinforcement-learning 계열의 사후학습이 FM에서 어떻게 재구성되어야 하는지 구체적 경로를 제공한다.

## 새로운 인사이트

보상 해킹이 모델의 출력을 '어디로도 가지 않게' 만드는 것이 아니라, 서로 상반하는 메트릭 간에 모델을 반복적으로 밀어내는 방향으로 작동한다는 시소 효과 효과의 발견은, reward-hacking을 '출력 회피'가 아닌 '메트릭 간 상호 소모'로 재이해하게 한다. 이는 exploration-hacking이 탐색 분포를 조작하는 것과 구조적으로 유사하면서도, 그 대상이 보상 지형(reward topology) 자체라는 점에서 training-process-gaming의 확장을 시사한다.

## 🔗 관련 논문

- Turning the TIDE: Cross-Architecture Distillation for Diffusion Large Models
- Beyond Negative Rollouts: Positive-Only Policy Optimization with Implicit Negative Gradients
- Can RL Teach Long-Horizon Reasoning to LLMs? Expressiveness

## 🏷️ 엔티티

- [[entities/flow-opd.md|flow-opd]]
- [[entities/flow-matching.md|flow-matching]]

## 📐 개념

- [[concepts/reward-sparsity.md|reward-sparsity]]
- [[concepts/gradient-interference.md|gradient-interference]]
- [[concepts/seesaw-effect.md|seesaw-effect]]
- [[concepts/flow-post-training-paradigm.md|flow-post-training-paradigm]]

---
_LLM 분석으로 생성됨_
