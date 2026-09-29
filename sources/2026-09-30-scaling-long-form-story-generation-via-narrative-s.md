# Scaling Long-Form Story Generation via Narrative State Tracking

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-30
**링크**: http://arxiv.org/abs/2609.35759v1

## 💡 핵심 인사이트

장편 생성의 스케일링 병목은 컨텍스트 길이가 아니라 명시적 서사 상태의 부재이며, training-free 상태 추적 에이전트 루프가 일관성 문제를 상태 관리 문제로 전환한다.

## 📖 분석

### NstAgent: Scaling Long-Form Story Generation via Narrative State Tracking (2026-09-30)

LLM 장편 소설 생성의 병목을 컨텍스트 용량이 아닌 명시적 서사 상태의 부재로 재규정한다. training-free 에이전틱 프레임워크 NstAgent는 등장인물·사건·설정·인과 구조를 구조화된 서사 상태로 추적하여, 생성이 상태를 갱신하고 상태가 후속 생성을 구속하는 폐루프를 형성한다. 이는 [[agent-loop-as-training-time]] 원리의 창작 도메인 실현이다 — 미세조정 없이 에이전트 루프의 반복만으로 일관성 능력이 확보됨을 보여준다.

동시에 [[knowledge-state-orchestration]]의 서사 특화 변형이다. ADEMA가 장기 태스크의 지식 상태를 오케스트레이션 계층으로 통합했다면, 본 논문은 창작에서 동일 패턴이 작동함을 확인시켜 지식 상태 관리가 도메인 불변 원리임을 강화한다. 추적된 서사 상태는 [[structured-intermediate-representation]]의 제3 유형(RAPID의 태스크 명세, SAG의 공유 그래프에 이은 서사 상태)이며, [[non-selective-context-accumulation]]의 해법이 된다 — 소설 규모에서 원문 축적 대신 선택적 구조 요약이 스케일링의 조건임을 입증한다.

[[dual-process-agent]] 관점에서 추적기(사고)와 생성기(행동)의 분리는 [[thought-action-separation]]의 창작 버전이다. 1만 단어 한계의 극복은 [[harness-methodology-embodiment-migration]]이 예고한 에이전틱 방법론의 도메인 확장이 코딩·로보틱스에 이어 창작으로 착지한 세 번째 사례다.

## 🔗 관련 논문

- ADEMA: A Knowledge-State Orchestration Architecture for Long-Horizon Knowledge
- CliffCompaction: Cost-Efficient Compaction for Long-Horizon Coding Agents
- RAPID: Robot Agentic Programming from Demonstrations
- Cognitive Extensions for Dual-Process Language Agents: Memory and Self
- Jev-Mobile: Jev as an Executor for Mobile GUI Agents

## 🏷️ 엔티티

- [[entities/knowledge-state-orchestration.md|knowledge-state-orchestration]]
- [[entities/agent-loop-as-training-time.md|agent-loop-as-training-time]]
- [[entities/structured-intermediate-representation.md|structured-intermediate-representation]]
- [[entities/non-selective-context-accumulation.md|non-selective-context-accumulation]]
- [[entities/dual-process-agent.md|dual-process-agent]]
- [[entities/thought-action-separation.md|thought-action-separation]]
- [[entities/harness-methodology-embodiment-migration.md|harness-methodology-embodiment-migration]]
- [[entities/narrative-state-tracking.md|narrative-state-tracking]]
- [[entities/long-form-story-generation.md|long-form-story-generation]]

## 📐 개념

- [[concepts/narrative-state-tracking.md|narrative-state-tracking]]
- [[concepts/long-form-story-generation.md|long-form-story-generation]]
- [[concepts/narrative-consistency.md|narrative-consistency]]
- [[concepts/training-free-agentic-scaffolding.md|training-free-agentic-scaffolding]]

---
_LLM 분석으로 생성됨_
