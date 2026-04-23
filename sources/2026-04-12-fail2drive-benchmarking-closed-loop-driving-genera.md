# Fail2Drive: Benchmarking Closed-Loop Driving Generalization

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-12
**링크**: http://arxiv.org/abs/2604.08535v1

## 💡 핵심 인사이트

자율주행 벤치마크에서 학습-테스트 시나리오 중복으로 인한 암기 효과를 배제하기 위해, paired-route 설계를 통해 분포 이동 하의 진정한 일반화 능력을 최초로 체계적으로 측정하는 벤치마크를 제안한다.

## 📖 분석

## Fail2Drive: Benchmarking Closed-Loop Driving Generalization

Fail2Drive는 CARLA 시뮬레이터 기반의 **최초의 paired-route 벤치마크**로, 폐루프(closed-loop) 자율주행의 일반화 능력을 체계적으로 평가한다. 200개 루트와 17개의 새로운 시나리오 클래스를 포함하며, 학습 시나리오를 테스트 시 재사용하는 기존 벤치마크의 한계를 지적한다.

### 핵심 문제의식
기존 자율주행 벤치마크는 학습과 동일한 시나리오를 테스트에 사용하여, 높은 성능이 **암기(memorization)**의 결과일 수 있다는 근본적 문제가 있다. Fail2Drive는 분포 이동(distribution shift) 조건에서의 진정한 일반화를 측정하는 데 초점을 맞춘다.

### 기존 Wiki와의 관계
- **[[concepts/autonomous-driving.md|autonomous driving]]**: CARLA 기반 자율주행 평가의 새로운 표준을 제안하며, VectorWorld 등 기존 월드 모델 연구와 상호보완적
- **[[concepts/closed-loop-evaluation.md|closed loop evaluation]]**: 폐루프 평가 방법론의 핵심 발전으로, 기존 UniDriveVLA, YC-Bench와 함께 에이전트 평가 체계를 확장
- **[[concepts/distribution-shift.md|distribution shift]]**: 분포 이동 하에서의 강건성 평가라는 점에서 세그멘테이션, 제어 분야의 연구들과 연결
- **[[concepts/world-model.md|world model]]**: 월드 모델의 일반화 한계를 드러내는 실증적 벤치마크로 기능

### 방법론적 기여
paired-route 설계를 통해 동일 루트에서 학습 조건과 새로운 조건을 직접 비교할 수 있어, 일반화 실패 지점을 정밀하게 진단할 수 있다. 이는 단순 성공률이 아닌 **일반화 격차(generalization gap)**를 정량화하는 새로운 평가 패러다임이다.

## 🔗 관련 논문

- 2026 04 11 fail2drive benchmarking closed loop driving genera
- 2026 04 09 toward consistent world models with multi token pr
- 2026 04 10 robust quadruped locomotion via evolutionary reinf

## 📐 개념

- [[concepts/autonomous-driving.md|autonomous-driving]]
- [[concepts/closed-loop-evaluation.md|closed-loop-evaluation]]
- [[concepts/distribution-shift.md|distribution-shift]]
- [[concepts/world-model.md|world-model]]
- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/generalization-gap.md|generalization-gap]]

---
_LLM 분석으로 생성됨_
