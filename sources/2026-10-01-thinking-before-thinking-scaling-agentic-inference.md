# Thinking Before Thinking: Scaling Agentic Inference Through Meta-Reasoning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-01
**링크**: http://arxiv.org/abs/2609.38147v1

## 💡 핵심 인사이트

실행 제어 선택(계승·재시작·중단)을 명시적 메타추론으로 격상하면 제어 자체가 태스크 연산과 분리된 일급 추론 대상이 되어, 에이전틱 추론이 '태스크 컴퓨트 + 제어 컴퓨트'의 이원 구조로 확장된다.

## 📖 분석

본 논문은 장기·복잡한 과제에서 실행 제어 선택(부분 작업 계승, 새로 시작, 중단 시점)을 암묵적 하네스 휴리스틱에서 명시적·구조적 추론 과정으로 격상하는 '에이전틱 메타추론(agentic meta-reasoning)'을 제안한다. Worker가 태스크 수준 연산을 담당하고 Controller가 실행이 확립한 내용을 통합하며 다음 선택지를 탐색하는 이원 구조는 사고-행동 분리([[thought-action-separation]])를 한 단계 더 정교화한다 — 사고 계층 내부가 태스크 사고(Worker)와 제어 사고(Controller)로 재분할된다.

Wiki 축적 논의와의 세 접점이 핵심이다. 첫째, [[artificial-id]]가 계속/정지/변경 판단을 내부 지속 구동으로 내면화했다면 본 논문은 동일 삼단 판단을 외부 Controller의 명시적 추론으로 유지하여, 제어 판단의 내면화-외면화 스펙트럼([[internal-external-control-continuum]])에서 대칭 극점을 형성한다. 둘째, [[harness-learning]]이 제어를 학습된 하네스 능력으로 내재화했다면 본 논문은 제어를 매 실행의 추론 대상으로 삼는 상보 경로로, '학습 대비 추론'이라는 하네스 설계의 새 선택 축을 부여한다. 셋째, Controller의 상태 통합은 지식 상태 오케스트레이션([[knowledge-state-orchestration]])의 런타임 실현이며, '어떤 부분 작업을 계승할까'의 명시적 판단은 재시도-컨텍스트 누적 루프([[retry-context-accumulation-loop]])의 비용 폭주를 구조적으로 제어하는 해법이 된다. 종료 판단이 추론 산출물로 이동하는 점에서 종료성 보장 문제([[termination-guarantee-problem]]), 옵션 간 예산 배분 관점에서 추론 예산 점진적 투입([[inference-budget-progressive-investment]])과도 연결된다.

## 🔗 관련 논문

- Artificial Id: Drive and Persistent Alignment in Agentic AI
- Harness Learning Enables Generalizable Test-Time Adaptation
- Grow the Harness, Not the Context: From Strategy-Free Scaffolds to Reu
- Stellar Colosseum: A Many-Agent Harness for Long-Horizon Research in M
- TokenCast: Forecasting Token Consumption During LLM Agent Execution
- Crab: A Semantics-Aware Checkpoint/Restore Runtime for Agent Sandboxes

## 🏷️ 엔티티

- [[entities/agentic-meta-reasoning.md|agentic-meta-reasoning]]
- [[entities/controller-worker-architecture.md|controller-worker-architecture]]
- [[entities/thought-action-separation.md|thought-action-separation]]
- [[entities/artificial-id.md|artificial-id]]
- [[entities/internal-external-control-continuum.md|internal-external-control-continuum]]
- [[entities/harness-learning.md|harness-learning]]
- [[entities/knowledge-state-orchestration.md|knowledge-state-orchestration]]
- [[entities/retry-context-accumulation-loop.md|retry-context-accumulation-loop]]
- [[entities/metacognition.md|metacognition]]
- [[entities/termination-guarantee-problem.md|termination-guarantee-problem]]
- [[entities/inference-budget-progressive-investment.md|inference-budget-progressive-investment]]
- [[entities/test-time-scaling.md|test-time-scaling]]

---
_LLM 분석으로 생성됨_
