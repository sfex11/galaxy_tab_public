# Benchmarks as Software: Terminal-Bench and the Case for Continuous Benchmarks

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-07
**링크**: http://arxiv.org/abs/2611.08417v1

## 💡 핵심 인사이트

벤치마크의 진부화는 우연한 고장이 아니라 유한한 유지보수 투자 하에서 필연적으로 누적하는 '부채'이며, 이를 다루는 올바른 체계는 일회성 정밀 검증이 아니라 소프트웨어 공학적 지속 유지보수(CI·회귀테스트·버전관리)의 벤치마크 이식이다.

## 📖 분석

# Benchmarks as Software: 벤치마크 유지보수 부채

본 논문은 코딩 에이전트 평가에서 출시 시점에 정밀 검증된 벤치마크조차 시간이 지나며 결함이 누적되는 현상을 **벤치마크 유지보수 부채(benchmark-maintenance-debt)**로 명명하고, 벤치마크를 **소프트웨어로서(benchmark-as-software)** 지속 관리해야 한다고 주장한다.

부채의 두 병인: (1) 모델이 개선되며 기존 검증자가 거부하는 유효한 해법을 발견하는 **검증자 진부화(verifier-staleness)** — 능력 성장이 평가 신뢰성을 훼손하는 역설, (2) 평가 인프라 변화가 태스크·테스트에 내장된 가정을 무효화하는 인프라 유발 무효화.

## 기존 Wiki와의 관계

- [[concepts/benchmark-obsolescence.md|benchmark obsolescence]]: EHR 라이브 벤치마크가 데이터 갱신으로 진부화를 다뤘다면, 본 논문은 검증자·인프라·가정의 3축으로 병인을 확장하고 진부화를 '부채'라는 관리 대상으로 격상시킨다.
- [[concepts/benchmark-specification-gap.md|benchmark specification gap]]: SWE-Gate의 '테스트 통과≠수용' 간극의 시간축 버전 — 출시 시 정합하던 명세가 모델·인프라 변화로 동적으로 괴리함을 보여 명세 간극이 정적 결함이 아니라 성장하는 속성임을 확립한다.
- [[concepts/living-benchmark.md|living benchmark]] / continuous-benchmark: living benchmark가 실세계 데이터 축의 갱신이라면, 지속 벤치마크는 CI·회귀테스트·버전관리라는 유지보수 체계의 이식이다.
- [[concepts/certification-monitoring-discontinuity.md|certification monitoring discontinuity]]: 출시 검증 이후 유효기간 미보장 문제가 피평가자에서 측정 기기 자체로 확장되는 사례.
- [[concepts/refreshable-signal-layer.md|refreshable signal layer]]: Claw-Eval-Live의 신호 주기 갱신 원리를 벤치마크 전 수명주기 유지보수로 일반화한다.
- [[entities/terminal-universe.md|terminal universe]]: 터미널/코딩 에이전트 환경이 생성(공급)과 유지(존속)의 이중 수명주기를 갖음을 시사한다.

## 핵심 통찰

진부화는 우연한 고장이 아니라 유한 유지보수 투자 하에서 필연적으로 누적하는 부채다. 해법은 벤치마크를 한 번 완성하는 것이 아니라, 결함 추적→수정→재검증의 반복 사이클을 벤치마크 생애에 내장하는 소프트웨어 공학적 제도화다.

## 🔗 관련 논문

- A Living Benchmark for Information Retrieval from Electronic Health Records
- Claw-Eval-Live: A Live Agent Benchmark for Evolving Real-World Workflows
- SWE-Gate: Passing Functional Tests Is Not Enough for Software Engineering
- Terminal-Universe: Turning Agent Trajectories into Scalable Terminal Environments
- Clean Engineering, Unstable Measurement: A Preregistered Reliability Framework

## 🏷️ 엔티티

- [[entities/benchmark-maintenance-debt.md|benchmark-maintenance-debt]]
- [[entities/benchmark-as-software.md|benchmark-as-software]]
- [[entities/continuous-benchmark.md|continuous-benchmark]]
- [[entities/verifier-staleness.md|verifier-staleness]]
- [[entities/benchmark-obsolescence.md|benchmark-obsolescence]]
- [[entities/benchmark-specification-gap.md|benchmark-specification-gap]]
- [[entities/living-benchmark.md|living-benchmark]]
- [[entities/certification-monitoring-discontinuity.md|certification-monitoring-discontinuity]]
- [[entities/refreshable-signal-layer.md|refreshable-signal-layer]]
- [[entities/terminal-universe.md|terminal-universe]]
- [[entities/evaluator-assumption.md|evaluator-assumption]]

## 📐 개념

- [[concepts/benchmark-maintenance-debt.md|benchmark-maintenance-debt]]
- [[concepts/benchmark-as-software.md|benchmark-as-software]]
- [[concepts/continuous-benchmark.md|continuous-benchmark]]
- [[concepts/verifier-staleness.md|verifier-staleness]]

---
_LLM 분석으로 생성됨_
