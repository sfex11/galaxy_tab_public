# Reward-Based Online LLM Routing via NeuralUCB

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-02
**링크**: http://arxiv.org/abs/2603.30035v1

## 💡 핵심 인사이트

NeuralUCB 기반 contextual bandit을 LLM 라우팅에 적용하면, 온라인 환경에서 탐색-활용 균형을 자동 조절하여 비용 대비 품질을 최적화할 수 있다.

## 📖 분석

## Reward-Based Online LLM Routing via NeuralUCB

본 논문은 NeuralUCB 알고리즘을 활용한 비용 인식(cost-aware) LLM 라우팅 문제를 다룬다. 여러 LLM이 존재할 때, 주어진 쿼리에 대해 어떤 모델을 호출할지 온라인으로 결정하는 라우팅 정책을 학습하는 것이 핵심이다.

### 배경 및 동기
기존 LLM 라우팅 접근법은 크게 두 갈래로 나뉜다: (1) 지도학습 기반 라우팅(supervised routing)은 사전 수집된 데이터로 라우터를 학습하지만 분포 변화에 취약하고, (2) 부분 피드백(partial-feedback) 기반 방법은 적응성이 높으나 효율성에서 트레이드오프가 존재한다. 본 연구는 NeuralUCB라는 신경망 기반 contextual bandit 알고리즘을 라우팅에 적용하여, 탐색(exploration)과 활용(exploitation)의 균형을 자동으로 조절한다.

### 핵심 방법론
NeuralUCB는 각 LLM을 bandit의 arm으로 모델링하고, 쿼리의 컨텍스트 표현을 입력으로 받아 각 모델의 기대 유틸리티(품질 대비 비용)를 예측한다. UCB(Upper Confidence Bound) 전략으로 불확실성이 높은 모델도 적절히 탐색하면서, 점진적으로 최적 라우팅 정책을 학습한다. RouterBench 시뮬레이션 환경에서 랜덤 및 최소비용(min-cost) 베이스라인을 일관되게 상회하는 성능을 보였다.

### 기존 연구와의 연결
이 연구는 [[Nemotron-Cascade 2]]의 cascade RL 기반 모델 선택 전략과 상보적이다. Nemotron-Cascade가 큰 모델과 작은 모델 간의 정적 cascade를 학습하는 반면, NeuralUCB 라우팅은 온라인 적응형으로 다수 모델 중 최적을 동적 선택한다. 또한 [[FinTradeBench]]처럼 LLM 성능을 비용 효율적으로 평가하는 벤치마크 연구와도 맥락을 공유하며, 비용-성능 트레이드오프 최적화라는 실용적 과제를 다룬다는 점에서 공통점이 있다.

## 🔗 관련 논문

- Nemotron-Cascade 2: Post-Training LLMs with Cascade RL and M
- FinTradeBench: A Financial Reasoning Benchmark for LLMs
- Box Maze: A Process-Control Architecture for Reliable LLM Re
- Chimera: Latency-and Performance-

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/speculative-decoding.md|speculative-decoding]]
- [[concepts/cascade-reinforcement-learning.md|cascade-reinforcement-learning]]

---
_LLM 분석으로 재생성됨_
