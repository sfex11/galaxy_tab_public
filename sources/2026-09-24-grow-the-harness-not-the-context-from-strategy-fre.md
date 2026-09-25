# Grow the Harness, Not the Context: From Strategy-Free Scaffolds to Reusable Specialist Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-24
**링크**: http://arxiv.org/abs/2609.26760v1

## 💡 핵심 인사이트

관련 태스크 스트림에서 반복되는 제어 결정은 매번 컨텍스트 안에서 재구성하지 말고, task feedback으로 하네스 자체를 성장시켜 재사용 가능한 실행 코드로 컴파일해야 하며 LLM은 태스크별 의미 추론에만 예약되어야 한다.

## 📖 분석

# Grow the Harness, Not the Context (2026-09-24)

표준 하네스는 관련 태스크 스트림을 처리할 때마다 동일한 제어 결정을 각 태스크의 컨텍스트 안에서 재구성하도록 강제한다. 본 논문은 이 반복 제어를 task feedback으로 학습해 재사용 가능한 실행 코드로 전환하고, LLM 호출은 태스크별 의미 추론에만 예약하는 **Growing Harness**를 제시한다 — strategy-free scaffold에서 고칠 수 있는 실패 신호를 따라 하네스 자체가 성장하는 failure-guided 훈련 패러다임이다.

## 기존 Wiki와의 관계
- [[harness-model-co-evolution]]: SafeEvolve(안전), Co-Evolving Harnesses(온폴리시 정정)에 이은 제3의 공진화 사례로, 하네스 진화가 실패 신호 기반 훈련 패러다임으로 체계화된다.
- [[retry-context-accumulation-loop]]: 제목 자체가 이 루프의 구조적 대안 — 컨텍스트 대신 하네스를 킨다.
- [[experience-infrastructuralization]]: 궤적·경험·코드에 이어 task feedback이 실행 인프라로 재질화되는 새 경로.
- [[failure-as-causal-data]]: 고칠 수 있는 실패가 하네스 코드 컴파일의 선택 압력으로 소비된다.
- [[skill-lifecycle-management]]: Designer-RSI의 '태스크 스트림→절차 메모리' 진화와 대응되되 재사용 단위가 하네스 코드라는 차이.
- [[harness-distillation]]과 대비: 하네스 이득을 가중치로 흡수하는 대신 실행 코드에 유지하는 반대 방향 선택.

## 새 인사이트
하네스가 설계 산출물에서 훈련 대상으로 이동한다. [[harness-mutability]] 변이 축(MOSS 소스 재작성, Procedural Graphs 궤적 변이)에 '누적적 성장'이 추가되고, [[thought-action-separation]]의 분리 기준이 인지 계층이 아닌 '안정적 반복 제어 vs 태스크별 의미'라는 하네스-모델 분업으로 재정의된다. [[designer-foresight-boundary]] 관점에서 strategy-free 출발은 설계자 전략 사전 주입을 실패 기반 유도로 대체한다.

## 🔗 관련 논문

- SafeEvolve: Harness-Policy Co-Evolution from Agent Experience for Safe
- Co-Evolving Harnesses and Models: On-Policy Correction Helps Weaker Mo
- Agentic Harness Engineering: Observability-Driven Automatic Evolution
- Procedural Graphs: Self-Evolving Execution Structures for LLM Agents
- Designer-RSI: Evolving Procedural Memory from User Traffic for Agentic
- Terminal-Universe: Turning Agent Trajectories into Scalable Terminal E
- MOSS: Self-Evolution through Source-Level Rewriting in Auton
- CodeMidas: Scaling Agentic Coding RL Environments from Code Itself

## 🏷️ 엔티티

- [[entities/growing-harness.md|growing-harness]]
- [[entities/harness-model-co-evolution.md|harness-model-co-evolution]]
- [[entities/agentic-harness-engineering.md|agentic-harness-engineering]]
- [[entities/harness-mutability.md|harness-mutability]]
- [[entities/retry-context-accumulation-loop.md|retry-context-accumulation-loop]]
- [[entities/experience-infrastructuralization.md|experience-infrastructuralization]]
- [[entities/failure-as-causal-data.md|failure-as-causal-data]]
- [[entities/code-as-agent-harness.md|code-as-agent-harness]]
- [[entities/skill-lifecycle-management.md|skill-lifecycle-management]]

## 📐 개념

- [[concepts/failure-guided-harness-growth.md|failure-guided-harness-growth]]
- [[concepts/strategy-free-scaffold.md|strategy-free-scaffold]]
- [[concepts/control-semantic-division.md|control-semantic-division]]
- [[concepts/observability-driven-evolution.md|observability-driven-evolution]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-23-rrsi-regularized-recursive-self-improvement-of-age]]: 두 논문 모두 에이전트 하네스를 일급 최적화 대상으로 보고, 태스크 피드백으로부터 프롬프트·제어 흐름·도구 구성을 자동으로 개선·컴파일하는 하네스 자동화 축을 공유한다.
- → [[sources/2026-09-24-cliffcompaction-cost-efficient-compaction-for-long]]: 장기 코딩 에이전트의 컨텍스트 팽창 문제를 자동 압축과 하네스 컴파일이라는 상호 보완적 전략으로 다루며, 컨텍스트를 계속 키우는 대신 구조로 전환한다는 관점을 공유한다.
