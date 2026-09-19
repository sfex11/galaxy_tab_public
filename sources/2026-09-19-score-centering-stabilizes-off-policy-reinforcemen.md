# Score Centering Stabilizes Off-policy Reinforcement Learning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-19
**링크**: http://arxiv.org/abs/2609.20807v1

## 💡 핵심 인사이트

TIM 하 오프폴리시 RL 불안정의 본질은 무작위 노이즈가 아닌 매 스텝 누적되는 엔진 간 지속 편향이며, TIM 제거 없이도 점수 중심화로 편향 성분만 제거해 안정성을 확보할 수 있다.

## 📖 분석

Score Centering Stabilizes Off-policy Reinforcement Learning (2026-09-19)은 LLM 강화학습의 훈련-추론 엔진 불일치(Training-Inference Mismatch, TIM)가 야기하는 불안정의 병인을 규명한다. TIM 완전 제거는 롤아웃 효율에 과대 비용을 부과하므로 비현실적인데, 불안정의 주범은 우연한 노이즈가 아니라 매 훈련 스텝마다 누적되는 엔진 간 지속 편향(drift)이다. 점수 중심화(score centering)는 이 편향 성분만 선택적으로 제거하여 TIM을 수용한 채 오프폴리시 RL의 안정성을 확보한다.

Wiki 관점의 세 축 기여가 있다. (1) TIM은 [[algorithm-system-translation-gap]]의 수치 계층 발현이다 — 커널·정밀도 차이라는 시스템 최적화의 산물이 알고리즘 계층(RL 수렴)의 불안정으로 번역되며, 간극 제거가 아닌 번역 손상의 국소 보정 전략이 유효함을 보여준다. (2) [[negative-rollout-noise]]나 [[exploration-hacking]]이 학습 신호의 모델 내부 오염을 다뤘다면, 본 논문은 인프라 기원의 신호 오염이라는 대척점 병인을 추가하여 훈련 안정성 문제의 원인 지형을 이원화한다. (3) [[cumulative-drift]]의 drift 개념을 연속학습의 데이터 기원에서 엔진 간 수치 누적 편향이라는 시스템 기원으로 확장한다. 비동기 롤아웃(효율)과 엔진 일치성(정확성)의 트레이드오프를 '편향-노이즈 분리'로 타결하는 것이 핵심 설계 통찰이다.

## 🔗 관련 논문

- Bellman Policy Optimization
- Beyond Negative Rollouts: Positive-Only Policy Optimization with Implicit Negative Gradient
- Post-Training Language Models for Gold-Medal Performance in Coding Competition

## 🏷️ 엔티티

- [[entities/reinforcement-learning.md|reinforcement-learning]]
- [[entities/training-inference-mismatch.md|training-inference-mismatch]]
- [[entities/score-centering.md|score-centering]]
- [[entities/post-training.md|post-training]]
- [[entities/algorithm-system-translation-gap.md|algorithm-system-translation-gap]]
- [[entities/cumulative-drift.md|cumulative-drift]]
- [[entities/negative-rollout-noise.md|negative-rollout-noise]]

## 📐 개념

- [[concepts/systemic-engine-drift.md|systemic-engine-drift]]
- [[concepts/bias-noise-decoupling.md|bias-noise-decoupling]]
- [[concepts/rollout-efficiency-exactness-tradeoff.md|rollout-efficiency-exactness-tradeoff]]

---
_LLM 분석으로 생성됨_
