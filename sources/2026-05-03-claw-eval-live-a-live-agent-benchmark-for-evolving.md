# Claw-Eval-Live: A Live Agent Benchmark for Evolving Real-World Workflows

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-03
**링크**: http://arxiv.org/abs/2604.28139v1

## 💡 핵심 인사이트

벤치마크의 '무엇을 평가할 것인가'와 '어떻게 평가할 것인가'를 독립적인 진화 속도를 가진 두 계층으로 분리함으로써, 평가 생태계 자체가 실세계 수요에 맞춰 자가 교정되는 구조를 최초로 달성했다.

## 📖 분석

# Claw-Eval-Live: A Live Agent Benchmark for Evolving Real-World Workflows

## 정의
에이전트가 소프트웨어 도구, 비즈니스 서비스, 로컬 워크스페이스에 걸쳐 수행하는 엔드투엔드 작업 단위를 평가하기 위한 라이브 벤치마크. 기존 벤치마크가 릴리스 시점에 태스크 집합을 동결하고 최종 응답만 평가하는 한계를 극복하기 위해, **갱신 가능한 신호 계층(refreshable signal layer)**과 **평가 계층(evaluation layer)**을 구조적으로 분리한다.

## 핵심 아키텍처: 신호-평가 분리
벤치마크를 두 계층으로 분해함으로써 서로 다른 진화 속도를 가지는 두 문제—'무엇을 평가할 것인가'와 '어떻게 평가할 것인가'—를 독립적으로 관리할 수 있게 된다. 신호 계층은 공개 워크플로우 수요 신호에서 주기적으로 갱신되며, 평가 계층은 실행 검증(execution verification)에 기반하여 최종 응답뿐 아니라 작업이 실제로 수행되었는지를 검사한다.

## 기존 Wiki와의 관계

### sandbox-liveworld-gap에 대한 구조적 해법
Claw-Eval-Live는 샌드박스-실세계 간극을 '자가 교정 경로'로 해소한다. 벤치마크가 시간에 따라 실세계로 수렴하도록 신호 계층을 갱신하는 메커니즘은, 정적 벤치마크가 가진 근본적 한계—평가 대상이 발전함에도 평가 기준이 정체되는 비대칭성—을 구조적으로 해결한다.

### harness-as-hidden-variable에 대한 통제
[[concepts/harness-as-hidden-variable.md|harness as hidden variable]]이 지적한 문제—하네스 구현이 태스크 난이도에 미치는 은닉 효과—에 대해, 신호 계층과 평가 계층의 분리가 통제 변수로 기능한다. 태스크 정의가 하네스 구현과 독립적으로 갱신될 수 있으므로, 하네스 변경이 태스크 난이도에 미치는 혼동 효과를 분리하여 관찰할 수 있게 된다.

### ClawGym과의 양축 형성
[[entities/clawgym.md|clawgym]]이 하네스-모델 결합 시스템의 진단에 집중한다면, Claw-Eval-Live는 평가 대상(태스크 신호) 자체의 실시간 진화를 다룬다. 두 시스템은 Claw 생태계 평가의 양축을 형성하며, 에이전트 평가가 '고정된 표적'이 아닌 '이동하는 표적'을 향하도록 패러다임을 전환시킨다.

## 평가 철학의 전환
기존 [[concepts/benchmark.md|benchmark]]가 '정적 태스크 성능 측정'에 머물렀다면, Claw-Eval-Live는 '평가 생태계의 자가 진화'를 도입한다. 이는 [[entities/mathduels.md|mathduels]]가 셀프플레이로 태스크를 동적으로 생성하는 접근과 상보적이다—MathDuels가 문제 공간 내에서 동적성을 확보한다면, Claw-Eval-Live는 문제 공간 자체를 실세계 수요에 맞춰 재정의한다.

## 🔗 관련 논문

- 2026-05-01-clawgym-a-scalable-framework-for-building-effectiv.md
- 2026-04-30-agentic-harness-engineering-observability-driven-a.md
- 2026-04-25-mathduels-evaluating-llms-as-problem-posers-and-so.md

## 🏷️ 엔티티

- [[entities/claw-eval-live.md|claw-eval-live]]
- [[entities/clawgym.md|clawgym]]
- [[entities/sandbox-liveworld-gap.md|sandbox-liveworld-gap]]
- [[entities/harness-as-hidden-variable.md|harness-as-hidden-variable]]
- [[entities/execution-verification.md|execution-verification]]
- [[entities/refreshable-signal-layer.md|refreshable-signal-layer]]
- [[entities/signal-evaluation-decoupling.md|signal-evaluation-decoupling]]
- [[entities/benchmark.md|benchmark]]
- [[entities/live-benchmark.md|live-benchmark]]

## 📐 개념

- [[concepts/signal-evaluation-decoupling.md|signal-evaluation-decoupling]]
- [[concepts/refreshable-signal-layer.md|refreshable-signal-layer]]
- [[concepts/sandbox-liveworld-gap.md|sandbox-liveworld-gap]]
- [[concepts/live-benchmark.md|live-benchmark]]

---
_LLM 분석으로 생성됨_
