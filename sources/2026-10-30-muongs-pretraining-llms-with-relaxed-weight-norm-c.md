# MuonGS: Pretraining LLMs with Relaxed Weight-Norm Control

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-30
**링크**: http://arxiv.org/abs/2610.37647v1

## 💡 핵심 인사이트

가중치 감쇠와 노름 제약의 효과는 누적 유효 학습률 C_T의 상한 보장으로 통일되며, norm control의 필요량은 이 누적량의 경계 조건에서 계산 가능하므로 과잉 제약을 완화할 정량적 여지가 존재한다.

## 📖 분석

Muon 사전학습에서 weight decay와 명시적 가중치 노름 제약이 왜 도움이 되고 얼마나 필요한지를 단일 수량으로 통일 분석한다: **누적 유효 학습률**([[accumulated-effective-learning-rate]]) C_T = Σ_t η_t/||W_t||_F. 명목 학습률을 가중치 노름으로 정규화한 유효 학습률([[effective-learning-rate]])을 전체 훈련 궤적에 걸쳐 누적하면, norm control([[optimizer-norm-control]])의 기능이 C_T의 상한 보장으로 환원된다.

세 가지 함의가 있다. 첫째, **'왜'의 통일** — 감쇠와 노름 제약이라는 상이한 메커니즘이 동일 목적(C_T 경계 유지)의 두 구현 경로로 재해석된다. 둘째, **'얼마나'의 계산 가능성** — 필요 제약 강도가 누적량의 경계 조건에서 유도되므로 상한 이상으로 강한 제약은 낭비이며, MuonGS는 최소 충분 강도로 제약을 완화해 사전학습을 가속한다. 셋째, **궤적 수준 분석** — 안정성 판정이 '지금 무엇이 일어나는가'에서 '지금까지 얼마나 쌓였는가'([[training-trajectory-analysis]])로 이동한다.

[[score-centering]]이 오프폴리시 RL의 스텝별 누적 편향(drift)을 중심화로 제거해 안정화했다면, 본 논문은 사전학습의 궤적 누적 이동량을 norm control로 경계한다 — 즉시 상태가 아닌 누적 수량의 예산 설계라는 동일 원리가 RL 훈련과 사전학습 양축에서 독립 수렴한 사례다. 균일 제어가 구조 이질성과 충돌한다는 [[component-aware-clipping]] 논의와 병렬하여, 제어 강도의 파라미터별 크기 조정 필요성도 시사한다.

## 🔗 관련 논문

- Score Centering Stabilizes Off-policy Reinforcement Learning
- Component-Aware Differential Privacy for Federated Multilingual Speech

## 🏷️ 엔티티

- [[entities/muongs.md|muongs]]
- [[entities/optimizer-norm-control.md|optimizer-norm-control]]
- [[entities/accumulated-effective-learning-rate.md|accumulated-effective-learning-rate]]
- [[entities/effective-learning-rate.md|effective-learning-rate]]
- [[entities/weight-norm-control.md|weight-norm-control]]
- [[entities/optimizer-design.md|optimizer-design]]
- [[entities/training-trajectory-analysis.md|training-trajectory-analysis]]
- [[entities/score-centering.md|score-centering]]

## 📐 개념

- [[concepts/accumulated-effective-learning-rate.md|accumulated-effective-learning-rate]]
- [[concepts/effective-learning-rate.md|effective-learning-rate]]
- [[concepts/optimizer-norm-control.md|optimizer-norm-control]]
- [[concepts/weight-norm-control.md|weight-norm-control]]
- [[concepts/accumulation-budget-design.md|accumulation-budget-design]]

---
_LLM 분석으로 생성됨_
