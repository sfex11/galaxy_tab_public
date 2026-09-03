# Post-Training Language Models for Gold-Medal Performance in Coding Competitions

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-04
**링크**: http://arxiv.org/abs/2609.02849v1

## 💡 핵심 인사이트

동일한 도메인과 파이프라인에서 모델 스케일이 훈련 방법의 필요성을 결정한다 — 550B MoE는 검증된 트레이스의 SFT만으로, 30B MoE는 SFT+RL이 필요하다는 대조는 RL의 역할이 능력 창출이 아니라 사전학습 분포 상한으로의 접근 촉진임을 실증한다.

## 📖 분석

이 논문은 [[nemotron-cascade-2]]의 계보를 잇는 NVIDIA의 경쟁 프로그래밍 특화 post-training 연구로, 22,000개 큐레이션 문제와 합성 추론 트레이스, SFT, RL을 결합한 end-to-end 파이프라인으로 IOI·ICPC 금메달급 성능을 달성했다. 핵심 구조적 발견은 **훈련 방법의 스케일 의존성**이다: 동일 파이프라인에서 30B-A3B MoE(Nemotron-3-Nano-CC)는 SFT+RL이, 550B-A55B MoE(Nemotron-3-Ultra-CC)는 SFT만이 적용되었다.

이 대조는 [[marginal-distribution-ceiling]] 논의를 스케일 축으로 확장한다 — 사전학습 분포 상한이 높은 대형 모델은 검증된 트레이스에 대한 SFT만으로 능력이 실현되지만, 소형 모델은 RL이 상한 도달을 촉진해야 한다. 이는 'scaling near optimal sft rl annotation budget allocation'의 SFT/RL 예산 할당 문제에 스케일 조건부 해를 제공한다.

[[post-training]] 관점에서 본 논문은 문제 큐레이션→합성 트레이스→SFT→RL의 완결적 특화 파이프라인을 제시하여, post-training이 단순 정제가 아닌 도메인 능력 창출 경로임을 실증한다. 코딩 경쟁은 테스트 통과라는 [[rlvr]]의 전형적 검증 환경이며, [[verifier-mediated-goal-delegation]]의 검증기 대행 구조가 작동하는 도메인이다. [[cascade-reinforcement-learning]] 방법론의 응용 확장이자 [[mixture-of-experts]] 활성 파라미터 구조에서의 경쟁급 추론 실현 사례다.

## 🔗 관련 논문

- scaling near optimal sft rl annotation budget allocation
- the rise of verbal reinforcement learning
- nemotron-cascade-2 post training llms with cascade
- reconciling process supervision with outcome based

## 🏷️ 엔티티

- [[entities/post-training.md|post-training]]
- [[entities/nemotron-cascade-2.md|nemotron-cascade-2]]
- [[entities/nvidia.md|nvidia]]
- [[entities/cascade-reinforcement-learning.md|cascade-reinforcement-learning]]
- [[entities/mixture-of-experts.md|mixture-of-experts]]
- [[entities/rlvr.md|rlvr]]
- [[entities/marginal-distribution-ceiling.md|marginal-distribution-ceiling]]
- [[entities/synthetic-data-generation.md|synthetic-data-generation]]
- [[entities/verifier-mediated-goal-delegation.md|verifier-mediated-goal-delegation]]
- [[entities/scale-conditional-training-strategy.md|scale-conditional-training-strategy]]
- [[entities/competitive-programming-benchmark.md|competitive-programming-benchmark]]

## 📐 개념

- [[concepts/verified-reasoning-trace.md|verified-reasoning-trace]]
- [[concepts/scale-conditional-rl-necessity.md|scale-conditional-rl-necessity]]
- [[concepts/problem-curation-pipeline.md|problem-curation-pipeline]]
- [[concepts/competition-grade-inference.md|competition-grade-inference]]
- [[concepts/sft-rl-budget-allocation.md|sft-rl-budget-allocation]]

---
_LLM 분석으로 생성됨_
