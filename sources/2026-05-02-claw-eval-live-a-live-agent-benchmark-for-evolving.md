# Claw-Eval-Live: A Live Agent Benchmark for Evolving Real-World Workflows

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-02
**링크**: http://arxiv.org/abs/2604.28139v1

## 💡 핵심 인사이트

벤치마크를 '고정된 표적'에서 '신호 계층과 평가 계층이 분리된 살아 있는 시스템'으로 재설계함으로써, 정적 벤치마크의 근본적 한계(천장 성능·태스크-현실 간극)를 아키텍처 수준에서 해소한다.

## 📖 분석

# Claw-Eval-Live

**카테고리**: 미분류
**생성일**: 2026-05-02

## 정의

Claw-Eval-Live는 정적 태스크 집합을 고정하지 않고, 공개 워크플로우 수요 신호에서 주기적으로 갱신되는 신호 계층(signal layer)과 안정적인 평가 계층을 분리한 라이브 에이전트 벤치마크다. 소프트웨어 도구, 비즈니스 서비스, 로컬 워크스페이스를 아우르는 end-to-end 워크플로우 에이전트를 대상으로, 최종 응답 평가뿐 아니라 태스크 실행 여부 자체를 검증한다.

## 기존 Wiki와의 관계

### sandbox-liveworld-gap에 대한 구조적 해법
기존 벤치마크들이 샌드박스 고정 태스크로 인해 실세계 격차를 구조적으로 내재하고 있던 문제에 대해, Claw-Eval-Live는 신호 계층의 주기적 갱신으로 벤치마크 자체를 '살아 있는' 시스템으로 만들어 격차를 동적으로 축소하는 경로를 제공한다.

### ClawGym과의 상보적 관계
ClawGym이 하네스 설계의 진단과 자동 진화에 집중한다면, Claw-Eval-Live는 평가 대상 자체(태스크 신호)의 진화를 다룬다. 두 논문이 합쳐 Claw 생태계에서 '하네스 진화'와 '태스크 진화'의 양축을 형성한다.

### evaluator-assumption의 우회
정적 문제 공간이라는 평가자의 근본적 가정을 신호-평가 분리 아키텍처로 해체한다: 평가 기준은 안정적이되, 평가 대상(태스크)은 실세계 수요에 따라 유동적으로 갱신된다.

## 관련 논문

- [[sources/2026-05-02-claw-eval-live-a-live-agent-benchmark-for-evolvin.md|Claw-Eval-Live: A Live Agent Benchmark for Evolving Real-World Workflows]]

## 🔗 관련 논문

- 2026 05 01 clawgym a scalable framework for building effectiv
- 2026 04 24 swe chat coding agent interactions from real users
- 2026 04 30 dv world benchmarking data visualization agents in
- 2026 04 13 clawbench can ai agents complete everyday online t

## 🏷️ 엔티티

- [[entities/claw-eval-live.md|claw-eval-live]]
- [[entities/clawgym.md|clawgym]]
- [[entities/sandbox-liveworld-gap.md|sandbox-liveworld-gap]]
- [[entities/harness-as-hidden-variable.md|harness-as-hidden-variable]]
- [[entities/evaluator-assumption.md|evaluator-assumption]]
- [[entities/computer-use-agent.md|computer-use-agent]]
- [[entities/benchmark.md|benchmark]]

## 📐 개념

- [[concepts/live-benchmark.md|live-benchmark]]
- [[concepts/refreshable-signal-layer.md|refreshable-signal-layer]]
- [[concepts/signal-evaluation-decoupling.md|signal-evaluation-decoupling]]
- [[concepts/execution-verification.md|execution-verification]]

---
_LLM 분석으로 생성됨_
