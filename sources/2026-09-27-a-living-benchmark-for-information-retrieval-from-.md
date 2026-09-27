# A Living Benchmark for Information Retrieval from Electronic Health Records

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-27
**링크**: http://arxiv.org/abs/2609.30205v1

## 💡 핵심 인사이트

벤치마크의 시효성은 갱신 비용이 아니라 표현 구조의 문제다 — 정적 아티팩트 대신 원천 데이터에서 파생되는 뷰로 재정의하면 진부화가 관리 대상에서 구조적으로 소멸한다.

## 📖 분석

# A Living Benchmark for Information Retrieval from Electronic Health Records (2026-09-27)

## 핵심 기여

LLM 임상 어시스턴트의 EHR 정보 검색·종합 능력 평가를 위한 라이브 벤치마크. 수동 큐레이션 벤치마크의 갱신 비용과 진부화 문제를, 환자 기록 원천 데이터로부터 QA 쌍을 자동 생성하는 확장 가능한 프레임워크로 해결한다.

## 기존 Wiki와의 관계

**ArchEHR-QA 계보의 후속 경로**: [[entities/archehr-qa.md|archehr qa]]가 수동 큐레이션의 시효성 한계를 드러냈다면, 본 논문은 동일 EHR QA 도메인에서 자동 생성으로 갱신 비용을 구조적으로 절감한다. 고정 벤치마크와 라이브 벤치마크의 비교 기준을 제공한다.

**라이브 벤치마크 패러다임의 도메인 확장**: [[entities/claw-eval-live.md|claw eval live]]가 에이전트 도메인에서 실세계 워크플로우 수요로 신호 계층을 주기 갱신했다면, 본 논문은 임상 도메인에서 원천 기록 기반 자동 생성으로 동일 원리([[concepts/refreshable-signal-layer.md|refreshable signal layer]])를 실현한다. 라이브 벤치마크가 단일 도메인 방법론이 아니라 벤치마크 설계의 일반 원리임을 확정한다.

**자동 생성의 접지 조건**: 자동 생성 QA가 갖는 순환적 타당성 위험은 실제 임상 기록이라는 원천 접지로 완화된다. 이는 검증 가능한 데이터 합성([[concepts/rlvr.md|rlvr]], [[concepts/verifiable-training-data-synthesis.md|verifiable training data synthesis]]) 계열과 접속되며, 생성 기반 평가가 성립하려면 생성 근거가 외부 실재에 고정되어야 함을 시사한다.

## 시사점

벤치마크의 시효성 문제는 갱신 비용의 문제가 아니라 표현 구조의 문제다. 벤치마크를 정적 아티팩트가 아닌 원천 데이터로부터 파생되는 뷰로 재정의하면, 진부화가 반복 관리의 대상에서 구조적으로 발생하지 않는 속성으로 전환된다.

## 🔗 관련 논문

- Claw-Eval-Live: A Live Agent Benchmark for Evolving Real-World Workflo
- HealthNLP_Retrievers at ArchEHR-QA 2026: Cascaded LLM Pipeli

## 🏷️ 엔티티

- [[entities/living-benchmark.md|living-benchmark]]
- [[entities/ehr-question-answering.md|ehr-question-answering]]
- [[entities/automatic-benchmark-generation.md|automatic-benchmark-generation]]
- [[entities/benchmark-obsolescence.md|benchmark-obsolescence]]
- [[entities/benchmark-auto-renewal.md|benchmark-auto-renewal]]
- [[entities/long-document-qa.md|long-document-qa]]

## 📐 개념

- [[concepts/refreshable-signal-layer.md|refreshable-signal-layer]]
- [[concepts/signal-evaluation-decoupling.md|signal-evaluation-decoupling]]
- [[concepts/verifiable-training-data-synthesis.md|verifiable-training-data-synthesis]]
- [[concepts/benchmark-domain-specialization.md|benchmark-domain-specialization]]

---
_LLM 분석으로 생성됨_
