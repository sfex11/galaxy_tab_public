# VeriCUA: Verification as Agentic Exploration for Computer-Using Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-31
**링크**: http://arxiv.org/abs/2610.40578v1

## 💡 핵심 인사이트

검증의 신뢰성은 판단 모델의 능력이 아니라 증거 수집 방식이 결정하며, 부분 관측 위의 검증은 능동 탐색 위의 검증으로 대체되어야 한다.

## 📖 분석

VeriCUA는 컴퓨터 사용 에이전트(CUA)의 태스크 완료 검증을 '수동 판단'에서 '능동 탐색'으로 전환하는 프레임워크다. 기존 자동 검증은 두 종류의 부분 관측에 의존했다 — VLM judge는 제공된 궤적·관찰만 보고 판정하고, 생성된 프로그램은 접근 가능한 애플리케이션 상태만 검사한다. VeriCUA는 검증기 자체가 에이전트처럼 디지털 환경을 탐색하며 완전한 증거를 수집하도록 검증을 재정의한다.

이는 [[single-surface-signal-insufficiency]]의 검증 도메인 실현이다 — 궤적 스냅샷이든 프로그램적 상태 접근이든, 어떤 단일 표면 신호도 실제 완료의 증거로 충분하지 않다. 동시에 [[non-cognitive-oracle]]과 [[environment-grounded-validity]]의 방향을 심화한다: 검증 근거가 모델의 판단이 아니라 탐색으로 획득한 실제 환경 상태에 위치한다.

CUA 생태계 차원에서 실행 환경(CUA-Universe 계열)과 검증 계층이 분리 공급되어, CUA 인프라가 환경-검증 양축으로 구조화됨을 보여준다. 검증 품질이 [[environment-synthesis-as-data-curation]]과 [[rlvr]]의 보상 신호 품질을 상류에서 결정한다는 점에서, 검증은 RL 파이프라인의 전제조건으로 격상된다. 다만 검증기가 에이전트가 됨으로써 [[audit-oracle-self-reference]]의 긴장이 새 층위로 이동한다 — 탐색 기반 검증의 독립성이 검증자 에이전트 자체의 신뢰성 문제로 환원된다.

## 🔗 관련 논문

- CUA-Universe: A Scalable and Dynamic Environment for Hybrid GUI+CLI Agents
- SWE-Gate: Passing Functional Tests Is Not Enough for Software Engineers
- Failure-Transparent Agents: Benchmarking Post-Failure Reporting in Tool Agents
- Quantifying Overclaiming Propensity in Frontier LLM Agents

## 🏷️ 엔티티

- [[entities/vericua.md|vericua]]
- [[entities/computer-use-agent.md|computer-use-agent]]
- [[entities/execution-verification.md|execution-verification]]

## 📐 개념

- [[concepts/verification-as-agentic-exploration.md|verification-as-agentic-exploration]]
- [[concepts/verifier-as-agent.md|verifier-as-agent]]
- [[concepts/partial-view-verification-limitation.md|partial-view-verification-limitation]]
- [[concepts/single-surface-signal-insufficiency.md|single-surface-signal-insufficiency]]
- [[concepts/non-cognitive-oracle.md|non-cognitive-oracle]]
- [[concepts/environment-grounded-validity.md|environment-grounded-validity]]
- [[concepts/independent-success-adjudication.md|independent-success-adjudication]]
- [[concepts/audit-oracle-self-reference.md|audit-oracle-self-reference]]

---
_LLM 분석으로 생성됨_
