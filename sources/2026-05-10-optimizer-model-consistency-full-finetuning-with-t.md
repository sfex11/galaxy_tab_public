# Optimizer-Model Consistency: Full Finetuning with the Same Optimizer as Pretraining Forgets Less

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-10
**링크**: http://arxiv.org/abs/2605.06654v1

## 💡 핵심 인사이트

사전학습 시 사용한 옵티마이저와의 일관성이 LoRA를 포함한 효율적 미세조정 방법보다 망각 완화에서 더 근본적이고 강력한 역할을 한다.

## 📖 분석

# optimizer-model-consistency

**카테고리**: 미분류
**생성일**: 2026-05-10

## 정의

사전학습과 동일한 옵티마이저를 사용한 전체 미세조정(full finetuning)이 다른 옵티마이저를 사용한 미세조정보다 동일하거나 더 나은 하류 성능을 달성하면서도 파라미터적 망각을 더 적게 유발하는 현상. 놀랍게도 이는 LoRA를 포함한 효율적 미세조정 방법들보다 우수한 학습-망각 트레이드오프를 달성한다.

## 관련 논문

- [[sources/2026-05-10-optimizer-model-consistency-full-finetuning-with-the-same.md|Optimizer-Model Consistency: Full Finetuning with the Same Optimizer as Pretraining Forgets Less]]

### Optimizer-Model Consistency: Full Finetuning with the Same Optimizer as Pretraining Forgets Less (2026-05-10)

옵티마이저 선택이 미세조정에서의 학습-망각 트레이드오프를 결정하는 핵심 변수임을 최초로 체계적으로 실증한다. LoRA가 항상 망각 완화에 유리하다는 도메인 내 통념을 정량적으로 도전하며, 옵티마이저-모델 간의 일관성이 아키텍처 수준의 적응(LoRA 등)보다 망각 제어에서 더 근본적인 역할을 함을 보여준다.

## 기존 Wiki와의 관계

이 현상은 [[entities/stabilized-knowledge-distillation|안정화 지식 증류]]가 출력 형식 안정성 전이 문제로 다룬 '미세조정 시 행동 안정성'이라는 더 넓은 문제 공간에서, 옵티마이저 선택이라는 훈련 과정 변수가 동일한 문제를 어떻게 해결하는지를 제공한다. 또한 [[entities/post-training|사후학습]]의 자기참조적 취약성(탐색 해킹 등) 논의가 주로 RL 기반 강화학습에 집중했다면, 본 논문은 SFT 단계의 옵티마이저 선택이라는 더 기초적인 축에서 사후학습 안정성을 문제화한다.

## 🔗 관련 논문

- 2026 05 06 standing on the shoulders of giants stabilized kno
- 2026 05 09 crafting reversible sft behaviors in large languag

## 🏷️ 엔티티

- [[entities/optimizer-model-consistency.md|optimizer-model-consistency]]
- [[entities/continual-learning.md|continual-learning]]
- [[entities/post-training.md|post-training]]

## 📐 개념

- [[concepts/optimizer-model-consistency.md|optimizer-model-consistency]]
- [[concepts/learning-forgetting-tradeoff.md|learning-forgetting-tradeoff]]

---
_LLM 분석으로 생성됨_
