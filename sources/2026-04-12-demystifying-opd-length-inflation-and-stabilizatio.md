# Demystifying OPD: Length Inflation and Stabilization Strategies for Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-12
**링크**: http://arxiv.org/abs/2604.08527v1

## 💡 핵심 인사이트

On-policy distillation에서 훈련 중 발생하는 급격한 길이 팽창(length inflation)이 truncation collapse를 유발하여 그래디언트 편향과 훈련 불안정성의 근본 원인이 됨을 규명하고, 이에 대한 안정화 전략을 제시한다.

## 📖 분석

## Demystifying OPD: Length Inflation and Stabilization Strategies for Large Language Models

본 논문은 **On-Policy Distillation(OPD)**의 실패 모드를 체계적으로 분석한다. OPD는 학생 모델이 자체 생성 분포 하에서 강력한 교사 모델의 지도를 받아 학습하는 기법인데, 훈련이 진행됨에 따라 on-policy rollout에서 **급격한 길이 팽창(length inflation)**이 발생하고, 이로 인해 잘린(truncated) 시퀀스가 훈련 데이터를 지배하는 **truncation collapse** 현상이 나타남을 규명한다. 이 현상은 반복 포화(repetition saturation)와 동반되며, 편향된 그래디언트 신호를 유발해 심각한 훈련 불안정성과 검증 성능 급락을 초래한다.

이 연구는 기존 Wiki의 [[on-policy-distillation]] 개념과 직접적으로 연결된다. Nemotron-Cascade 2에서 다룬 cascade RL 기반 post-training과 on-policy distillation이 본 논문에서 분석하는 핵심 기법이다. 또한 [[knowledge-distillation]]의 실패 모드에 대한 구체적 사례 연구로, 기존의 distillation 연구들이 간과한 on-policy 환경에서의 길이 팽창 문제를 조명한다.

[[reward-hacking]] 개념과도 관련이 깊다. 길이 팽창은 보상 모델이 긴 응답에 높은 점수를 부여하는 경향에서 비롯될 수 있으며, 이는 RLHF 훈련에서의 reward hacking과 유사한 메커니즘이다. [[training-data-pruning]]과도 연결되는데, truncation collapse는 훈련 데이터의 품질 저하 문제와 맞닿아 있다. [[scaling-laws]] 관점에서도 모델 크기와 길이 팽창 간의 관계를 이해하는 데 기여한다.

## 🔗 관련 논문

- 2026 03 23 nemotron cascade 2 post training llms with cascade
- 2026 04 11 cram less to fit more training data pruning improv
- 2026 04 07 understanding the role of hallucination in reinfor
- 2026 04 11 what do language models learn and when the implici

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/on-policy-distillation.md|on-policy-distillation]]
- [[concepts/knowledge-distillation.md|knowledge-distillation]]
- [[concepts/reward-hacking.md|reward-hacking]]
- [[concepts/training-data-pruning.md|training-data-pruning]]
- [[concepts/scaling-laws.md|scaling-laws]]
- [[concepts/post-training.md|post-training]]
- [[concepts/length-inflation.md|length-inflation]]
- [[concepts/truncation-collapse.md|truncation-collapse]]

---
_LLM 분석으로 생성됨_
