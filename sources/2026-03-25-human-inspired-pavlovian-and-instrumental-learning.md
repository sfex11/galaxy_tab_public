# Human-Inspired Pavlovian and Instrumental Learning for Autonomous Agent Navigation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-25
**링크**: http://arxiv.org/abs/2603.22170v1

## 💡 핵심 인사이트

신경과학의 Pavlovian/Instrumental 이중 학습 체계를 강화학습에 통합하여, 안전한 반사적 반응과 목표 지향적 계획을 동시에 달성하는 하이브리드 아키텍처를 제안한다.

## 📖 분석

## Human-Inspired Pavlovian and Instrumental Learning for Autonomous Agent Navigation

본 논문은 신경과학에서 영감을 받은 하이브리드 강화학습 아키텍처를 제안한다. 핵심은 인간의 학습 메커니즘을 세 가지 구성요소로 분해한 것이다: (1) **Pavlovian 학습** — 자극-반응 기반의 빠른 반사적 행동으로, 위험 회피 등 즉각적 반응을 담당, (2) **Instrumental Model-Free (MF)** — 경험 기반의 습관적 행동 학습, (3) **Instrumental Model-Based (MB)** — 환경 모델을 활용한 목표 지향적 계획 수립.

이 세 시스템의 통합은 기존 강화학습의 근본적 딜레마를 해결하려는 시도이다. 순수 MF 방법은 수렴이 느리고 탐색 과정에서 안전하지 않을 수 있으며, MB 방법은 계산 비용이 높고 모델 불일치(model mismatch)에 취약하다. Pavlovian 구성요소를 추가함으로써 안전한 탐색을 보장하면서도, MF/MB의 장점을 상황에 따라 적응적으로 활용할 수 있다.

이 연구는 [[concepts/reinforcement-learning.md|reinforcement learning]]의 새로운 방향을 제시하며, 특히 [[concepts/embodied-ai.md|embodied ai]] 분야의 자율 내비게이션 과제와 직접적으로 연결된다. Pavlovian 학습의 반사적 안전 메커니즘은 [[concepts/ai-safety.md|ai safety]] 관점에서도 의미가 있으며, 모델 기반/모델 프리의 적응적 전환은 [[concepts/meta-learning.md|meta learning]]의 아이디어와 맥을 같이 한다. 또한 인간 인지 모델링에 기반한 설계는 [[concepts/cognitive-modeling.md|cognitive modeling]]과 [[concepts/theory-of-mind.md|theory of mind]] 연구와도 접점을 형성한다. 탐색-활용 균형 문제는 [[decoupling-exploration-and-policy-optimization]] 연구와 상보적 관계에 있다.

## 🔗 관련 논문

- 2026 04 10 robust quadruped locomotion via evolutionary reinf
- 2026 04 09 maestro adapting guis and guiding navigation with 

## 📐 개념

- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/embodied-ai.md|embodied-ai]]
- [[concepts/cognitive-modeling.md|cognitive-modeling]]
- [[concepts/meta-learning.md|meta-learning]]
- [[concepts/ai-safety.md|ai-safety]]

---
_LLM 분석으로 재생성됨_
