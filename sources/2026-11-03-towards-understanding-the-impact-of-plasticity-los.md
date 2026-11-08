# Towards Understanding the Impact of Plasticity Loss on Reinforcement Learning in Stochastic Environments

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-03
**링크**: http://arxiv.org/abs/2610.42100v1

## 💡 핵심 인사이트

환경 확률성은 엔진 드리프트와 별개로 네트워크의 학습 가능성 자체를 침식하는 표상 층위 병리를 유발하므로, 심층 RL 안정성 분석은 수치·표상의 이중 층위에서 수행되어야 한다.

## 📖 분석

## 개요

심층 강화학습의 취약성(brittleness)을 플라스티시티 손실로 설명하는 최근 연구 흐름에서 환경 확률성 요인을 최초로 체계적으로 분리한 연구. SAC 에이전트를 세 개의 DeepMind Control 태스크에서 통제된 수준의 관측·보상 노이즈로 증강하여 훈련함으로써, 환경 확률성과 네트워크 학습 가능성 상실의 상호작용을 인과적으로 측정한다.

## Wiki 내 위치: 안정성 논의의 표상 층위 확장

기존 wiki의 RL 안정성 논의는 알고리즘-인프라 층에 집중했다. [[entities/score-centering.md|score centering]]이 훈련-추론 엔진 간 계통적 편향(drift)을 제거했고 [[concepts/cumulative-drift.md|cumulative drift]]가 그 누적 동역학을 규명했다. 본 논문은 이 구도에 **표상 층**의 제3 축을 추가한다 — 확률적 노이즈가 엔진 드리프트와 별개로 네트워크의 적응 능력 자체를 침식하는 plasticity-loss를 유발함. [[concepts/bias-noise-decoupling.md|bias noise decoupling]]의 노이즈-편향 구분이 알고리즘 층을 넘어 네트워크 층까지 확장된다.

## 연결점

- [[concepts/continual-learning.md|continual learning]]: 플라스티시티 손실은 연속 학습 실패의 기제론적 병인이다. 문제가 '망각 관리'에서 '학습 가능성 보존'으로 확장됨을 RL 도메인에서 확정한다.
- [[concepts/false-positive-convergence.md|false positive convergence]]: 낮은 수준의 안정적 보상에 정착한 상태가 환경 이해의 성과가 아니라 플라스티시티 붕괴의 발현일 수 있어, 수렴 판정에 학습 가능성 진단이 전제된다.
- [[concepts/training-inference-mismatch.md|training inference mismatch]]: TIM(수치 층)과 플라스티시티 손실(표상 층)은 상이한 원인과 처방을 가지는 병렬 병리로, 훈련 불안정의 이중 층위 구조를 완성한다.
- [[concepts/negative-rollout-noise.md|negative rollout noise]]: 환경 노이즈(외부 기인)와 롤아웃 노이즈(상호작용 기인)는 서로 다른 오염 경로이지만 학습 신호 품질을 침식한다는 공통점을 공유한다.

## 🔗 관련 논문

- Score Centering Stabilizes Off-policy Reinforcement Learning
- Beyond Negative Rollouts: Positive-Only Policy Optimization with Implicit Negative Gradient

## 🏷️ 엔티티

- [[entities/plasticity-loss.md|plasticity-loss]]
- [[entities/score-centering.md|score-centering]]
- [[entities/cumulative-drift.md|cumulative-drift]]
- [[entities/continual-learning.md|continual-learning]]
- [[entities/false-positive-convergence.md|false-positive-convergence]]
- [[entities/training-inference-mismatch.md|training-inference-mismatch]]
- [[entities/negative-rollout-noise.md|negative-rollout-noise]]

## 📐 개념

- [[concepts/plasticity-loss.md|plasticity-loss]]
- [[concepts/environmental-stochasticity.md|environmental-stochasticity]]
- [[concepts/rl-brittleness.md|rl-brittleness]]
- [[concepts/bias-noise-decoupling.md|bias-noise-decoupling]]

---
_LLM 분석으로 생성됨_
