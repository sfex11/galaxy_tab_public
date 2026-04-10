# Fail2Drive: Benchmarking Closed-Loop Driving Generalization

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-11
**링크**: http://arxiv.org/abs/2604.08535v1

## 💡 핵심 인사이트

기존 자율주행 벤치마크는 학습 시나리오를 테스트에 재사용하여 암기를 일반화로 오인할 수 있으며, paired-route 설계를 통해 분포 변화 하의 진정한 일반화 능력을 측정해야 한다.

## 📖 분석

## Fail2Drive: Benchmarking Closed-Loop Driving Generalization

**분류**: 자율주행 벤치마크, 일반화 평가

### 개요
Fail2Drive는 CARLA 시뮬레이터 기반의 폐루프(closed-loop) 자율주행 일반화 벤치마크로, 기존 벤치마크가 학습 시나리오를 테스트에 재사용하여 암기(memorization)를 측정할 수 있다는 문제를 지적한다. 200개의 경로와 17개의 새로운 시나리오 클래스를 포함하는 최초의 paired-route 벤치마크를 제안하여, 분포 변화(distribution shift) 하에서의 진정한 일반화 능력을 측정한다.

### 핵심 기여
- **Paired-route 설계**: 학습 분포와 체계적으로 다른 테스트 시나리오를 구성하여, 모델의 암기 vs 일반화를 명확히 구분
- **17개 신규 시나리오 클래스**: 분포 변화의 다양한 축(날씨, 교통 밀도, 도로 유형 등)을 체계적으로 커버
- **일반화 병목 진단**: 폐루프 자율주행에서 분포 변화가 여전히 핵심 병목임을 실증적으로 확인

### 기존 Wiki와의 관계
- **[[autonomous-driving]]**: 자율주행 분야의 핵심 벤치마크 연구로, VectorWorld 등 기존 자율주행 연구와 직접적으로 연결된다. VectorWorld가 효율적 세계 모델 생성에 초점을 맞췄다면, Fail2Drive는 평가 방법론 자체의 신뢰성을 문제 삼는다.
- **[[llm-benchmark]]**: LLM 벤치마크의 일반화 문제(데이터 오염, 암기 등)와 유사한 문제의식을 자율주행 도메인에서 제기한다.
- **[[world-model]]**: 폐루프 평가는 세계 모델의 예측 정확도와 직결되며, 일반화 실패가 세계 모델의 한계에서 기인할 수 있음을 시사한다.
- **[[reinforcement-learning]]**: 폐루프 주행 정책의 일반화는 강화학습의 sim-to-real transfer 문제와 밀접하게 관련된다.

## 🔗 관련 논문

- 2026 04 10 robust quadruped locomotion via evolutionary reinf
- 2026 04 10 cadence context adaptive depth estimation for navi

## 📐 개념

- [[concepts/autonomous-driving.md|autonomous-driving]]
- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/world-model.md|world-model]]
- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/closed-loop-evaluation.md|closed-loop-evaluation]]
- [[concepts/distribution-shift.md|distribution-shift]]

---
_LLM 분석으로 생성됨_
