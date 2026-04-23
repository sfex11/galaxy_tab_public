# Fail2Drive: Benchmarking Closed-Loop Driving Generalization

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-13
**링크**: http://arxiv.org/abs/2604.08535v1

## 💡 핵심 인사이트

기존 closed-loop 자율주행 벤치마크는 학습 시나리오를 테스트에 재사용하여 memorization을 일반화로 오인할 수 있으며, paired-route 설계를 통해 이를 최초로 정량적으로 분리할 수 있다.

## 📖 분석

## Fail2Drive: Benchmarking Closed-Loop Driving Generalization

Fail2Drive는 CARLA 시뮬레이터 기반의 최초 **paired-route 벤치마크**로, 폐쇄 루프(closed-loop) 자율주행의 일반화 능력을 체계적으로 평가한다. 기존 벤치마크들이 학습 시나리오를 테스트에 재사용하여 memorization과 진정한 일반화를 구분하지 못하는 문제를 지적하며, 200개 경로와 17개 신규 시나리오 클래스를 제공한다.

### 기존 Wiki와의 관계

본 논문은 기존 Wiki의 [[concepts/autonomous-driving.md|autonomous driving]], [[concepts/closed-loop-evaluation.md|closed loop evaluation]], [[concepts/distribution-shift.md|distribution shift]], [[concepts/generalization-gap.md|generalization gap]], [[concepts/world-model.md|world model]] 개념과 직접적으로 연결된다. 특히 2026-04-11에 등록된 동일 제목의 이전 버전(v1 → 업데이트)과 연속선상에 있으며, [[fail2drive]] 시리즈의 확장판이다.

### 핵심 기여

1. **Paired-route 설계**: 동일 경로를 학습/미학습 시나리오로 쌍을 이루어, memorization vs. generalization을 정량적으로 분리
2. **17개 신규 시나리오 클래스**: 학습 분포 외부의 다양한 driving situation을 체계적으로 구성
3. **Distribution shift 정량화**: 기존 모델들이 학습 분포 내에서는 성공하지만 분포 이동 시 급격히 성능이 하락함을 실증

### 다른 논문과의 연결

- [[sources/2026-04-11-fail2drive-benchmarking-closed-loop-driving-genera.md]]: 본 논문의 이전 버전으로 직접적 연속성
- [[sources/2026-03-19-vectorworld-efficient-streaming-world-model-via-di.md]]: world model 기반 자율주행과의 비교 관점
- [[sources/2026-04-10-robust-quadruped-locomotion-via-evolutionary-reinf.md]]: 강화학습 기반 로봇 일반화 문제와 유사한 distribution shift 도전과제 공유

## 🔗 관련 논문

- 2026 04 11 fail2drive benchmarking closed loop driving genera
- 2026 04 12 fail2drive benchmarking closed loop driving genera
- 2026 03 19 vectorworld efficient streaming world model via di
- 2026 04 10 robust quadruped locomotion via evolutionary reinf

## 📐 개념

- [[concepts/autonomous-driving.md|autonomous-driving]]
- [[concepts/closed-loop-evaluation.md|closed-loop-evaluation]]
- [[concepts/distribution-shift.md|distribution-shift]]
- [[concepts/generalization-gap.md|generalization-gap]]
- [[concepts/world-model.md|world-model]]
- [[concepts/paired-route-benchmark.md|paired-route-benchmark]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-04-14-physics-informed-reinforcement-learning-of-spatial]]: 둘 다 자율주행의 일반화 문제를 다루며, 전자는 memorization vs 일반화 분리 벤치마크를, 후자는 물리 정보 기반 RL로 맵 없는 레이싱의 OOD 일반화를 다룬다.
