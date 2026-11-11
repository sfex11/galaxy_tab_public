# Continual-ARC: Measuring Skill Acquisition over a Working Lifetime

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-12
**링크**: http://arxiv.org/abs/2611.14505v1

## 💡 핵심 인사이트

메모리 기반 하네스 학습과 가중치 기반 학습을 동일 척도에서 비교 가능하게 하는 것은 '학습'의 정의를 기판 불문 기능으로 재정의하는 측정 인프라다.

## 📖 분석

Continual-ARC는 에이전트 하네스([[harness-engineering]])를 파라메트릭 학습과 병렬되는 지속학습 메커니즘으로 격상시키는 평가 프레임워크다. 세 ARC-AGI 에디션을 도메인 지식이 불필요한 종생 스트림으로 재구성하여, 단일 도메인·일회성 인스턴스·단일 학습자 계열이라는 기존 벤치마크의 3대 한계를 동시에 해소한다.

핵심 기여는 메모리 기반(하네스) 학습과 가중치 기반 학습을 동일 척도에서 비교 가능하게 만든 것이다. 이는 [[functional-learning-criterion]]의 경험적 실현이며, [[phase-to-substrate-axis-shift]]가 예측한 위상 축→학습 기판 축 치환을 측정 인프라 수준에서 확정한다. 작업 수명 전체의 스킬 획득 곡선은 [[agent-loop-as-training-time]]의 관점에서 에이전트 루프 반복의 학습 가치를 그래디언트 스텝과 동격으로 정량화한다.

일회성 정확도 대신 복리적 능력 누적을 측정하려는 [[continual-compoundability]]에 도메인 불변 벤치마크를 제공하고, [[cross-episode-reuse-failure]]를 측정 가능한 축으로 만든다. 각 인스턴스의 일회성 제시는 [[data-contamination-resistance]]의 암기 우회를 구조적으로 차단하며, 세계 모델 지속학습 벤치마크([[continual-learning]]) 계열과 함께 지속학습 평가가 '무엇을 학습 기판으로 삼는가'의 비교 문제로 이동하고 있음을 보여준다.

## 🔗 관련 논문

- Benchmarking World Models for Continual Learning on Composit
- Harness Learning Enables Generalizable Test-Time Adaptation
- Grow the Harness, Not the Context: From Strategy-Free Scaffolds to Reu
- Learning Meta-Skills for Agent Harness Design in Test-Time A

## 🏷️ 엔티티

- [[entities/continual-arc.md|continual-arc]]
- [[entities/continual-learning.md|continual-learning]]
- [[entities/continual-compoundability.md|continual-compoundability]]
- [[entities/functional-learning-criterion.md|functional-learning-criterion]]
- [[entities/phase-to-substrate-axis-shift.md|phase-to-substrate-axis-shift]]
- [[entities/agent-loop-as-training-time.md|agent-loop-as-training-time]]
- [[entities/cross-episode-reuse-failure.md|cross-episode-reuse-failure]]
- [[entities/data-contamination-resistance.md|data-contamination-resistance]]
- [[entities/agentic-harness-engineering.md|agentic-harness-engineering]]
- [[entities/learning-task-curation.md|learning-task-curation]]

## 📐 개념

- [[concepts/memory-weight-learning-parity.md|memory-weight-learning-parity]]
- [[concepts/single-use-instance-presentation.md|single-use-instance-presentation]]
- [[concepts/working-lifetime-evaluation-horizon.md|working-lifetime-evaluation-horizon]]
- [[concepts/functional-learning-criterion.md|functional-learning-criterion]]
- [[concepts/lifelong-task-stream.md|lifelong-task-stream]]

---
_LLM 분석으로 생성됨_
