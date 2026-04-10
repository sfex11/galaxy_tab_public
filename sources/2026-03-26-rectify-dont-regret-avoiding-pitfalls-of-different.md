# Rectify, Don't Regret: Avoiding Pitfalls of Differentiable Simulation in Trajectory Prediction

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-26
**링크**: http://arxiv.org/abs/2603.23393v1

## 💡 핵심 인사이트

완전 미분 가능한 클로즈드루프 시뮬레이터는 역전파 경로를 통해 미래 정보가 누출되는 숏컷 학습 문제를 야기하며, 기울기 경로의 선택적 차단이 이를 해결하는 핵심 전략이다.

## 📖 분석

## Rectify, Don't Regret: Avoiding Pitfalls of Differentiable Simulation in Trajectory Prediction

본 논문은 자율주행 궤적 예측에서 미분 가능한 시뮬레이션(differentiable simulation)의 근본적 함정을 분석하고 이를 해결하는 방법을 제안한다.

### 문제 정의
기존 오픈루프(open-loop) 궤적 모델은 초기의 작은 편차가 누적되어 분포 외(out-of-distribution) 상태로 빠지는 **복합 오류(compounding error)** 문제를 겪는다. 이를 해결하기 위해 완전 미분 가능한 클로즈드루프 시뮬레이터가 제안되었으나, **숏컷 학습(shortcut learning)** 이라는 새로운 문제가 발생한다. 손실 기울기가 유도된 상태 입력을 통해 역전파되면서, 미래의 ground truth 정보가 모델의 이전 예측으로 누출되는 현상이다.

### 핵심 기여
논문은 이 기울기 누출 문제를 이론적으로 분석하고, 역전파 경로를 선택적으로 차단(rectify)하는 방식으로 숏컷 학습을 방지하면서도 클로즈드루프 학습의 이점을 유지하는 접근법을 제시한다. 이는 [[closed-loop-evaluation]]에서 논의된 클로즈드루프 평가의 중요성을 학습 단계로 확장하면서도, 미분 가능 시뮬레이션 고유의 함정을 체계적으로 다룬다는 점에서 차별화된다.

### 연결점
- **autonomous-driving**: 자율주행 궤적 예측의 핵심 과제인 분포 이동 문제를 다루며, [[Fail2Drive]]가 벤치마킹한 클로즈드루프 일반화 실패 사례와 직접적으로 관련된다.
- **world-model**: 미분 가능 시뮬레이터는 일종의 월드 모델로 기능하며, [[VectorWorld]]의 스트리밍 월드 모델 접근과 보완적 관계에 있다.
- **differentiable-rendering**: 미분 가능 렌더링과 유사하게 시뮬레이션 전체를 미분 가능하게 만드는 패러다임의 한계를 탐구한다.

## 🔗 관련 논문

- 2026 04 11 fail2drive benchmarking closed loop driving genera
- 2026 03 19 vectorworld efficient streaming world model via di

## 📐 개념

- [[concepts/differentiable-simulation.md|differentiable-simulation]]
- [[concepts/shortcut-learning.md|shortcut-learning]]
- [[concepts/compounding-error.md|compounding-error]]
- [[concepts/trajectory-prediction.md|trajectory-prediction]]
- [[concepts/closed-loop-training.md|closed-loop-training]]

---
_LLM 분석으로 재생성됨_
