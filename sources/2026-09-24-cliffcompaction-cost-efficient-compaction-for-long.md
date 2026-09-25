# CliffCompaction: Cost-Efficient Compaction for Long-Horizon Coding Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-24
**링크**: http://arxiv.org/abs/2609.26779v1

## 💡 핵심 인사이트

세션 간 자동 압축은 정보 손실 비용이 아니라 성능 유지·향상과 비용 절감을 동시에 실현하는 제1급 최적화 축이며, 세션 경계를 넘는 상태 이월의 실질 매개체다.

## 📖 분석

**CliffCompaction**은 장기 코딩 에이전트가 수백만 토큰 규모 컨텍스트를 다룰 때 직면하는 컨텍스트 창 한계를 세션 간 자동 압축(autocompaction)으로 해결하는 기법이다. 제한된 컨텍스트 예산 하에서 비용을 최대 50% 절감하면서 Terminal-Bench 성능을 유지·향상시키고, KernelBench에서 최고 수준 결과와 test-time scaling의 새로운 효율 지평을 달성한다.

**기존 Wiki와의 관계**: 이 논문은 concepts/non-selective-context-accumulation과 concepts/retry-context-accumulation-loop가 진단한 '무차별적 컨텍스트 축적 → 비용 폭주' 문제의 실용적 해법 측을 제공한다. CompactionRL이 압축 정책을 RL로 학습 최적화하는 방향이었다면 본 논문은 세션 경계를 넘는 자동 압축이라는 운영 차원을 추가해 압축 연구의 스펙트럼을 완성한다. ConvMem(2026-09-11)이 고정 크기 메모리의 병렬 합성곱 갱신으로 동일 문제를 풀었다면, 본 논문은 그 축을 세션 간 압축으로 확장한다. concepts/episodic-persistent-state-gap과 concepts/cross-episode-reuse-failure가 지적한 세션 간 상태 단절에서 압축 결과물이 사실상 상태 이월의 운반 단위로 기능함을 보여준다.

**핵심 시사**: 성능이 유지·향상된다는 점에서 압축은 정보 손실 비용이 아니라 내재적 큐레이션이다. concepts/descriptive-decisional-memory-divergence의 예측대로 결정적 가치를 보존하는 압축은 묘사적 충실도의 희생을 허용하며, bounded context가 탐색 분포를 정제해 concepts/test-time-scaling 효율을 높인다.

## 🔗 관련 논문

- ConvMem: Convolutional Memory for Long-Context Reasoning
- Terminal-Universe: Turning Agent Trajectories into Scalable Terminal Environments
- An Interpretable Memory Decision Controller for LLM Agents Based on Markov Decision Processes

## 🏷️ 엔티티

- [[entities/autocompaction.md|autocompaction]]
- [[entities/non-selective-context-accumulation.md|non-selective-context-accumulation]]
- [[entities/retry-context-accumulation-loop.md|retry-context-accumulation-loop]]
- [[entities/test-time-scaling.md|test-time-scaling]]
- [[entities/episodic-persistent-state-gap.md|episodic-persistent-state-gap]]
- [[entities/cross-episode-reuse-failure.md|cross-episode-reuse-failure]]
- [[entities/compactionrl.md|compactionrl]]
- [[entities/convmem.md|convmem]]
- [[entities/token-efficiency.md|token-efficiency]]

## 📐 개념

- [[concepts/cross-session-compaction.md|cross-session-compaction]]
- [[concepts/descriptive-decisional-memory-divergence.md|descriptive-decisional-memory-divergence]]
- [[concepts/consolidation-extinction-cycle.md|consolidation-extinction-cycle]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-24-grow-the-harness-not-the-context-from-strategy-fre]]: 장기 코딩 에이전트의 컨텍스트 팽창 문제를 자동 압축과 하네스 컴파일이라는 상호 보완적 전략으로 다루며, 컨텍스트를 계속 키우는 대신 구조로 전환한다는 관점을 공유한다.
- → [[sources/2026-09-24-speakermem-r1-speaker-centered-dual-track-memory-f]]: 무한정 늘어나는 세션·대화 이력을 구조화된 메모리(자동 압축, 화자 중심 분해 트랙)로 이월하는 장기 기억 관리라는 공통 문제를 다룬다.
- → [[sources/2026-09-24-the-sirens-song-when-proximal-background-context-o]]: 장기 컨텍스트의 정보 과잉이 성능을 저하한다는 진단을 공유하며, 내용 기반 주의 정렬과 자동 압축이라는 상호 보완적 컨텍스트 관리 기법을 제시한다.
- → [[sources/2026-09-25-agent-editing-world-model-rethinking-world-modelin]]: 장기 과업에서 오염된 에이전트 상태(낡은 계획, 누적 컨텍스트)의 정제를 세계 모델 개입과 자동 압축으로 각각 수행하는 에이전트 상태 관리 연구로 연결된다.
