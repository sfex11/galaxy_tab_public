# Benchmarks as Software: Terminal-Bench and the Case for Continuous Benchmarks

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-08
**링크**: http://arxiv.org/abs/2611.08417v1

## 💡 핵심 인사이트

벤치마크는 한 번 검증되어 완성되는 정적 도구가 아니라, 모델·인프라·가정의 노후화로 지속적으로 결함이 누적되는 소프트웨어이며, 평가 타당성은 유지보수 절차의 출력이다.

## 📖 분석

## Benchmarks as Software: Terminal-Bench와 지속 벤치마크

이 논문은 코딩 에이전트 평가의 근본 문제를 '벤치마크가 낡아가는 것'으로 재정의한다. 개념의 핵심은 **benchmark-maintenance-debt** — 검증자, 평가 인프라, 암묵적 가정이 노후화하면서 생기는 결함의 누적이다. 기존 Wiki의 living-benchmark(2026-09-26-a-living-benchmark-for-information-retrieval-from-.md)가 EHR 데이터 갱신으로 진부화를 다뤘다면, 본 논문은 병인을 검증자·인프라·가정의 3축으로 분해하고 개념을 측정·관리 대상으로 격상시킨다.

핵심 발견: 개선된 모델이 기존 검증자가 거부하는 '유효한 해'를 발견하는 **verifier-staleness**는 포화·과적합과 다른 기기 자체의 판정 오류다. 고정 벤치마크 전제의 '두 번째 균열'로, verifier-false-negative-rejection과 직결된다.

기존 Wiki와의 연결:
- [[concepts/benchmark-obsolescence.md|benchmark obsolescence]]: 측정 대상 이동 vs 측정기기 고정의 **parasitic-measurement-fixation** 구조를 공유
- [[concepts/adaptive-validity.md|adaptive validity]]: 벤치마크 타당성 자체를 '유지보수 루프의 출력'으로 보는 benchmark-validity-as-maintenance-output 논리를 확장
- [[concepts/black-box-instrument-drift.md|black box instrument drift]]: 측정 도구의 시간적 드리프트라는 공통 위상
- [[entities/agentic-harness-engineering.md|agentic harness engineering]]: '평가 계약으로서의 하네스'가 측정-실행 인프라 결합하에 진부화하는 양상

의미: '지속 벤치마크'는 단순 자동 갱신이 아니라, 갱신·버저닝·재현 절차가 소프트웨어처럼 정식화되어야 한다는 요구다. 이는 dynamic-evaluation-landscape와 evaluator-assumption 비판 계열의 후속 정교화다.

## 🔗 관련 논문

- 2026-09-26-a-living-benchmark-for-information-retrieval-from-.md
- 2026-04-26-mathduels-evaluating-llms-as-problem-posers-and-so.md
- 2026-09-08-does-your-agents-memory-survive-a-model-upgrade-a-.md
- 2026-09-07-clean-engineering-unstable-measurement-a-preregist.md
- 2026-11-07-scientist-world-grow-a-research-world-for-ai-scien.md

## 🏷️ 엔티티

- [[entities/benchmark-maintenance-debt.md|benchmark-maintenance-debt]]
- [[entities/benchmark-as-software.md|benchmark-as-software]]
- [[entities/continuous-benchmark.md|continuous-benchmark]]
- [[entities/verifier-staleness.md|verifier-staleness]]
- [[entities/benchmark-obsolescence.md|benchmark-obsolescence]]
- [[entities/parasitic-measurement-fixation.md|parasitic-measurement-fixation]]
- [[entities/adaptive-validity.md|adaptive-validity]]
- [[entities/benchmark-validity-as-maintenance-output.md|benchmark-validity-as-maintenance-output]]
- [[entities/black-box-instrument-drift.md|black-box-instrument-drift]]
- [[entities/living-benchmark.md|living-benchmark]]
- [[entities/verifier-false-negative-rejection.md|verifier-false-negative-rejection]]
- [[entities/agentic-harness-engineering.md|agentic-harness-engineering]]
- [[entities/dynamic-evaluation-landscape.md|dynamic-evaluation-landscape]]
- [[entities/evaluator-assumption.md|evaluator-assumption]]
- [[entities/meta-level-instrument-drift.md|meta-level-instrument-drift]]

## 📐 개념

- [[concepts/benchmark-maintenance-debt.md|benchmark-maintenance-debt]]
- [[concepts/benchmark-as-software.md|benchmark-as-software]]
- [[concepts/continuous-benchmark.md|continuous-benchmark]]
- [[concepts/verifier-staleness.md|verifier-staleness]]
- [[concepts/benchmark-debt-decomposition.md|benchmark debt decomposition]]
- [[concepts/measurement-validity-as-maintenance-output.md|measurement validity as maintenance output]]
- [[concepts/instrument-drift-in-evaluation-infrastructure.md|instrument drift in evaluation infrastructure]]

---
_LLM 분석으로 생성됨_
