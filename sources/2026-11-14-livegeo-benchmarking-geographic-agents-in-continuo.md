# LiveGeo: Benchmarking Geographic Agents in Continuously Evolving Worlds

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-14
**링크**: http://arxiv.org/abs/2611.17267v1

## 💡 핵심 인사이트

평가 환경의 진화를 벤치마크 설계자의 갱신 작업이 아니라 외부 세계의 내재적 시간 프로세스로 위임하면, 실세계 수렴과 순환 타당성 회피를 동시에 달성할 수 있다는 것 — 단, 그 대가로 검증 가능한 상태 이력의 보존이 필수 전제가 된다.

## 📖 분석

# LiveGeo: Benchmarking Geographic Agents in Continuously Evolving Worlds

LiveGeo는 외부 세계 상태가 자체 시간 프로세스를 따라 진화하는 GeoWorld 환경 위에서 지리 에이전트의 신뢰성 있는 의사결정을 평가하는 벤치마크다. 핵심은 기존 에이전트 평가의 두 전제를 동시에 해체하는 것이다. 첫째, 지리 구조를 고정 상태로 두는 관행([[continual-arc]]의 작업 수명 관점에서도 세계는 정적이었다)을 '에이전트와 무관하게 흐르는 외부 시간축'으로 대체한다. 둘째, 검증 가능한 상태 이력(verbatim state history)을 보존하므로 진화하는 세계에서도 판정의 감사 가능성이 유지된다.

이는 [[refreshable-signal-layer]]와 environment-evolution-for-terminal-agents 계열의 자가 갱신 벤치마크 논의를 지리 도메인으로 확장하되, 중요한 차이를 만든다. Claw-Eval-Live의 신호 갱신이 벤치마크 설계자가 주기적으로 수행했다면, LiveGeo의 세계 진화는 외생적(exogenous)이다. 즉 [[exogenous-evolution]]의 평가 버전으로, 세계가 에이전트의 능력이나 평가 의도와 무관하게 변하므로 순환적 타당성 문제([[circular-validity-problem]])에 구조적으로 덜 취약하다.

또한 verifiable state history 요구는 retrace-distilling-tool-using-agents-into-planner-free-workflows가 보여준 실행 로그의 학습 코퍼스화([[execution-record-as-learning-corpus]])와 맞닿는다 — 진화하는 세계에서의 상태 이력은 곧 시간 조건부 의사결정의 훈련·평가 자원이 된다. 장기 관점에서는 [[continual-compoundability]]의 측정 문제(시간이 지나며 축적되는 능력)에 '세계도 축적된다'는 제2의 축을 추가하여, 작업 수명 평가가 에이전트 내부 변화와 외부 세계 변화의 결합 함수임을 시사한다.

## 🔗 관련 논문

- 2026-11-12-continual-arc-measuring-skill-acquisition-over-a-w
- 2026-11-12-retrace-distilling-tool-using-agents-into-planner-free-workflows
- 2026-05-03-claw-eval-live-a-live-agent-benchmark-for-evolving
- 2026-09-06-environment-evolution-for-terminal-agents
- 2026-11-07-swarmevolve-latent-agent-swarms-for-evolutionary-d

## 🏷️ 엔티티

- [[entities/continual-arc.md|continual-arc]]
- [[entities/refreshable-signal-layer.md|refreshable-signal-layer]]
- [[entities/environment-evolution-for-terminal-agents.md|environment-evolution-for-terminal-agents]]
- [[entities/exogenous-evolution.md|exogenous-evolution]]
- [[entities/circular-validity-problem.md|circular-validity-problem]]
- [[entities/execution-record-as-learning-corpus.md|execution-record-as-learning-corpus]]
- [[entities/continual-compoundability.md|continual-compoundability]]

## 📐 개념

- [[concepts/continuously-evolving-world.md|continuously-evolving-world]]
- [[concepts/exogenous-world-evolution.md|exogenous-world-evolution]]
- [[concepts/verifiable-state-history.md|verifiable-state-history]]
- [[concepts/temporal-ground-truth-drift.md|temporal-ground-truth-drift]]
- [[concepts/live-geographic-agent-evaluation.md|live-geographic-agent-evaluation]]

---
_LLM 분석으로 생성됨_
