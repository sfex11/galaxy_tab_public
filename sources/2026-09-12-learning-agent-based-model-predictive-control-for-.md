# Learning Agent-based Model Predictive Control for Holistic Vehicle Performance

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-12
**링크**: http://arxiv.org/abs/2609.11871v1

## 💡 핵심 인사이트

분산 다중 에이전트 제어의 실용화 병목은 계산 능력이 아니라 '모든 에이전트의 기여를 안다'는 지식 완전성 가정이며, 데이터 기반 학습은 이 가정의 붕괴를 보상하는 하이브리드 구조의 필수 계층이 된다.

## 📖 분석

# Learning Agent-based Model Predictive Control for Holistic Vehicle Performance (LAMPC)

**날짜**: 2026-09-12 | **arXiv**: 2609.11871

## 핵심 기여

Agent-based MPC(AMPC)는 복수 에이전트의 협력으로 차량의 전체(holistic) 성능을 최적화하는 분산 제어 기법이다. 그러나 AMPC의 최적성은 '모든 에이전트와 그 기여를 정확히 아는 예측 모델'에 의존하며, 이 전제는 실제 구현에서 비현실적이다. 본 논문은 모델 기반 AMPC와 데이터 기반 학습을 결합한 하이브리드 제어 기법 LAMPC를 제안한다.

## Wiki 연결

### 분산 MPC 논의의 확장
기존 [[model-predictive-control]] 축(ADMM 기반 분산 MPC, 밀도 구동 최적 제어)은 형식적 보장에 집중했다. LAMPC는 분산 MPC의 실용화 병목이 계산이 아니라 **에이전트 지식 완전성**에 있음을 규명한다.

### 이상화 가정 붕괴의 제어 도메인 발현
'모든 에이전트 기여를 안다'는 전제는 [[pre-existing-data-assumption]]과 동형의 이상화 가정이다. 이상화 전제가 구현에서 붕괴하면 학습이 간극을 흡수한다는 Wiki의 축적 패턴이 제어 도메인에서 재현된다.

### 모델+데이터 하이브리드
해석적 모델의 구조적 보장과 학습의 미지 기여 보상을 결합하는 설계는 [[model-based-rl]] 패러다임과 수렴하며, 순수 모델 기반의 취약성과 순수 데이터 기반의 샘플 비효율을 동시에 완화한다.

## 핵심 인사이트

분산 다중 에이전트 제어의 실용화 병목은 계산이 아닌 완전한 시스템 지식 가정이며, 학습은 미지의 에이전트 기여에 대한 모델 부족을 채우는 보상 계층으로 기능한다.

## 🔗 관련 논문

- ADMM-Based Distributed MPC with Control Barrier Functions
- Density-Driven Optimal Control: Convergence Guarantees
- Model-Based Reinforcement Learning for Control under Time-Varying Dynamics
- Multi-Agent Reinforcement Learning for Autonomous UAV Exploration in Wildfire

## 🏷️ 엔티티

- [[entities/lampc.md|lampc]]
- [[entities/model-predictive-control.md|model-predictive-control]]
- [[entities/distributed-optimization.md|distributed-optimization]]
- [[entities/model-based-rl.md|model-based-rl]]

## 📐 개념

- [[concepts/complete-agent-model-assumption.md|complete-agent-model-assumption]]
- [[concepts/hybrid-model-data-control.md|hybrid-model-data-control]]
- [[concepts/prediction-accuracy-bottleneck.md|prediction-accuracy-bottleneck]]

---
_LLM 분석으로 생성됨_
