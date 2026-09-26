# A Living Benchmark for Information Retrieval from Electronic Health Records

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-26
**링크**: http://arxiv.org/abs/2609.30205v1

## 💡 핵심 인사이트

수동 큐레이션 벤치마크의 구식화는 도메인 불변의 구조적 결함이며, 실세계 데이터 원천(EHR)에서 QA 쌍을 자동 생성하는 'living benchmark'로 해결 가능함을 임상 도메인에서 실증한다.

## 📖 분석

## 라이브 벤치마크 원리의 임상 도메인 확장

LLM 기반 임상 어시스턴트가 EHR에 통합되는 가운데, 기존 수동 큐레이션 벤치마크의 구조적 한계 — 높은 갱신 비용과 빠른 구식화 — 를 자동 QA 쌍 생성으로 해결한다. 긴 입원 기록에서 질문-답변 쌍을 확장 가능하게 자동 생성하여, 벤치마크가 기술 발전과 함께 지속 갱신되는 'living benchmark'를 구현한다.

### 기존 Wiki와의 관계

[[live-benchmark]]·[[claw-eval-live]] 계열의 신호 갱신 원리가 임상 도메인으로 확장된 사례다. Claw-Eval-Live가 실세계 워크플로우 수요에서 신호를 주기 갱신했다면, 본 논문은 환자 기록이라는 실제 데이터 원천에서 QA 쌍을 자동 생성하여 동일한 자가 교정 경로를 [[refreshable-signal-layer]]에 추가한다. 신호 갱신의 소스가 '실세계 수요'에서 '실세계 데이터'로 다양화된다.

ArchEHR-QA 계열([[archehr-qa]], [[grounded-clinical-qa]], [[ehr-question-answering]])에 대해, 고정 큐레이션 벤치마크에서 자동 갱신 벤치마크로의 전환 경로를 제공한다. [[benchmark-domain-specialization]]의 수직 도메인 트렌드에 '임상 기록 라이브 벤치마크'라는 새 축을 추가하며, [[benchmark-format-blindspot]]이 지적한 수동 큐레이션의 시효성 문제에 대한 구조적 해법이 된다.

## 🔗 관련 논문

- 2026-05-01-healthnlp_retrievers-at-archehr-qa-2026-cascaded-llm-pipeline
- 2026-09-16-verifiable-by-construction-claim-level-evaluation-of-verbatim-citation
- 2026-05-02-claw-eval-live-a-live-agent-benchmark-for-evolving
- 2026-05-03-claw-eval-live-a-live-agent-benchmark-for-evolving
- 2026-09-24-swe-serve-benchmarking-agentic-engineering-for-production-inference-serving

## 🏷️ 엔티티

- [[entities/live-benchmark.md|live-benchmark]]
- [[entities/claw-eval-live.md|claw-eval-live]]
- [[entities/refreshable-signal-layer.md|refreshable-signal-layer]]
- [[entities/archehr-qa.md|archehr-qa]]
- [[entities/grounded-clinical-qa.md|grounded-clinical-qa]]
- [[entities/ehr-question-answering.md|ehr-question-answering]]
- [[entities/medical-ai.md|medical-ai]]
- [[entities/benchmark-domain-specialization.md|benchmark-domain-specialization]]
- [[entities/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[entities/automatic-benchmark-generation.md|automatic-benchmark-generation]]

## 📐 개념

- [[concepts/living-benchmark.md|living-benchmark]]
- [[concepts/benchmark-obsolescence.md|benchmark-obsolescence]]
- [[concepts/automatic-question-generation.md|automatic-question-generation]]
- [[concepts/long-document-qa.md|long-document-qa]]
- [[concepts/benchmark-auto-renewal.md|benchmark-auto-renewal]]

---
_LLM 분석으로 생성됨_
