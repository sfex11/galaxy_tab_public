# score-centering

**카테고리**: 미분류
**생성일**: 2026-09-19

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-09-19-score-centering-stabilizes-off-policy-reinforcemen.md|Score Centering Stabilizes Off-policy Reinforcement Learning]]

### Score Centering Stabilizes Off-policy Reinforcement Learning (2026-09-21)

본 논문이 원천 정의를 확립한다 — 스코어 센터링이 매 학습 스텝마다 누적되는 훈련-추론 엔진 간 계통적 편향(drift)을 제거하여 오프폴리시 RL을 안정화하는 메커니즘이며, TIM 완전 제거의 롤아웃 효율 비용 없이 안정성을 확보하는 알고리즘 측 경로를 제공한다.

### MuonGS: Pretraining LLMs with Relaxed Weight-Norm Control (2026-10-29)

훈련 역학의 계통적 변수를 누적량으로 진단하는 방법론 계보에 사전학습 측 사례를 추가한다. Score Centering이 drift의 누적 편향을 스코어 중심화로 제거했다면, MuonGS는 노름 제어의 효과가 누적 유효 학습률로 환원됨을 보여, 훈련 안정성 분석의 단위가 스텝에서 궤적 적분으로 이동하는 공통 방향을 강화한다.

→ [[sources/2026-10-29-muongs-pretraining-llms-with-relaxed-weight-norm-c.md|상세 보기]]

### MuonGS: Pretraining LLMs with Relaxed Weight-Norm Control (2026-10-30)

스코어 센터링이 오프폴리시 RL의 스텝별 누적 편향(drift)을 제거하는 것과 방법론적으로 동형이다. 두 논문 모두 즉시 상태가 아닌 궤적 누적 수량의 경계를 제어하는 알고리즘 측 개입으로 안정성을 확보하며, 누적 수량 분석 원리가 사전학습과 RL 훈련 양축에서 독립 수렴했음을 확정한다.

→ [[sources/2026-10-30-muongs-pretraining-llms-with-relaxed-weight-norm-c.md|상세 보기]]
