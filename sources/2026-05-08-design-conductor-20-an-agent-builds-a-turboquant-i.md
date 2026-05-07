# Design Conductor 2.0: An agent builds a TurboQuant inference accelerator in 80 hours

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-08
**링크**: http://arxiv.org/abs/2605.05170v1

## 💡 핵심 인사이트

하네스와 기저 모델의 공진화가 복합적 성능 향상을 낳아, 하네스 엔지니어링은 모델 발전 주기와 동기화된 진화적 과정으로 재설계되어야 한다.

## 📖 분석

# design-conductor

**카테고리**: 하드웨어 설계 자동화
**생성일**: 2026-05-08

## 정의

Design Conductor는 LLM 기반 다중 에이전트 하네스가 복잡한 하드웨어 설계를 자율적으로 수행하는 시스템이다. 2025년 12월 버전에서 5단계 Linux-capable RISC-V CPU를 12시간에 설계했으며, 2026년 5월 버전(2.0)에서는 80배 더 큰 작업인 TurboQuant 추론 가속기를 80시간에 완성했다.

## 하네스-모델 공진화

이 시스템의 핵심 발견은 하네스와 기저 모델의 **공진화(co-evolution)**가 복합적 성능 향상을 낳는다는 것이다. 2025년 12월~2026년 4월 사이 프론티어 모델의 진화만으로도 성능이 향상되었지만, 하네스 자체를 동시에 개선하면 두 축의 개선이 곱셈적으로 결합한다. 이는 [[agentic-harness-engineering|하네스 엔지니어링]]이 정적 최적화가 아닌 모델 발전과 동기화된 진화적 과정이어야 함을 실증한다.

## 작업 규모의 비선형 확장

CPU 설계(12시간)에서 추론 가속기 설계(80시간)로의 80배 규모 확장이 시간 측면에서는 ~6.7배 증가에 그친다. 이는 하네스가 작업 규모에 대해 아임(linear) 이하의 시간 증가를 달성함을 시사하며, [[harness-as-hidden-variable|하네스를 은닉 변수로 처리]]하는 기존 벤치마크가 하네스 설계 품질이 작업 규모 확장성을 어떻게 결정하는지를 보여준다.

## 관련 문제

- 하드웨어 설계는 [[sandbox-liveworld-gap|샌드박스-실세계 격차]]의 극단적 사례—설계의 검증이 실제 패브리케이션에서만 완료됨
- [[autoresearch|오토리서치]]의 스코프를 소프트웨어에서 하드웨어 아티팩트로 확장하며, [[artifact-bound-optimization|아티팩트 구속 최적화]]가 반드시 나쁜 것은 아님을 보여줌

## 🔗 관련 논문

- 2026-04-30-agentic-harness-engineering-observability-driven-a.md
- 2026-05-01-clawgym-a-scalable-framework-for-building-effectiv.md
- 2026-04-25-from-research-question-to-scientific-workflow-leve.md

## 🏷️ 엔티티

- [[entities/agentic-harness-engineering.md|agentic-harness-engineering]]
- [[entities/harness-as-hidden-variable.md|harness-as-hidden-variable]]
- [[entities/autoresearch.md|autoresearch]]
- [[entities/sandbox-liveworld-gap.md|sandbox-liveworld-gap]]
- [[entities/artifact-bound-optimization.md|artifact-bound-optimization]]
- [[entities/design-conductor.md|design-conductor]]

## 📐 개념

- [[concepts/harness-model-co-evolution.md|harness-model-co-evolution]]
- [[concepts/autonomous-hardware-design.md|autonomous-hardware-design]]
- [[concepts/non-linear-task-scaling.md|non-linear-task-scaling]]

---
_LLM 분석으로 생성됨_
