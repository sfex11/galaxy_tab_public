# Demystifying OPD: Length Inflation and Stabilization Strategies for Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-13
**링크**: http://arxiv.org/abs/2604.08527v1

## 💡 핵심 인사이트

On-Policy Distillation에서 훈련 중 on-policy 롤아웃의 길이가 급격히 팽창하여 truncation collapse를 유발하며, 이것이 반복 포화 및 편향된 그래디언트를 통해 훈련 불안정성의 근본 원인이 된다.

## 📖 분석

## Demystifying OPD: Length Inflation and Stabilization Strategies for Large Language Models

본 논문은 **On-Policy Distillation(OPD)**의 핵심 실패 모드인 **length inflation(길이 팽창)** 현상을 체계적으로 분석한다. OPD는 학생 모델이 자신의 분포에서 생성한 롤아웃에 대해 강한 교사 모델의 감독을 받는 훈련 방식인데, 훈련이 진행됨에 따라 on-policy 롤아웃의 길이가 급격히 증가하여 **truncation collapse**가 발생한다. 이는 반복 포화(repetition saturation)와 결합되어 편향된 그래디언트 신호를 유발하고, 훈련 불안정성 및 검증 성능의 급격한 하락으로 이어진다.

### 기존 Wiki와의 관계

이 논문은 기존 Wiki의 [[on-policy-distillation]] 개념과 직접적으로 연결되며, 특히 Nemotron-Cascade 2에서 다룬 cascade RL 및 distillation 파이프라인의 안정성 문제를 심화한다. [[truncation-collapse]]와 [[length-inflation]] 개념은 이미 2026-04-12자로 등록되어 있으며, 본 논문이 해당 개념의 주요 출처이다.

[[scaling-laws]] 및 [[curriculum-learning]]과도 관련이 있는데, OPD의 길이 팽창은 훈련 데이터 분포가 학습 중 동적으로 변하는 non-stationary 문제이기 때문이다. [[reasoning-shift]]에서 다룬 컨텍스트에 따른 추론 길이 변화 현상과도 맥락을 공유한다.

### 핵심 기여

1. OPD에서 길이 팽창→truncation→반복 포화의 인과 체인을 최초로 규명
2. 안정화 전략(stabilization strategies) 제안으로 OPD 실용성 향상
3. 편향된 그래디언트 신호의 메커니즘을 수학적으로 분석

## 🔗 관련 논문

- 2026 04 12 demystifying opd length inflation and stabilizatio
- 2026 04 11 cram less to fit more training data pruning improv
- 2026 04 11 what do language models learn and when the implici

## 📐 개념

- [[concepts/on-policy-distillation.md|on-policy-distillation]]
- [[concepts/truncation-collapse.md|truncation-collapse]]
- [[concepts/length-inflation.md|length-inflation]]
- [[concepts/training-data-pruning.md|training-data-pruning]]
- [[concepts/scaling-laws.md|scaling-laws]]
- [[concepts/reasoning-shift.md|reasoning-shift]]

---
_LLM 분석으로 생성됨_
