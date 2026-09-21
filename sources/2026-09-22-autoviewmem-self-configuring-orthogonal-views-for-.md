# AutoViewMem: Self-Configuring Orthogonal Views for Conversational Long-Term Memory

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-22
**링크**: http://arxiv.org/abs/2609.21940v1

## 💡 핵심 인사이트

기억 스키마 설계는 설계 시점의 고정 선택이 아니라 런타임 자기 설정 대상이며, 이질적 정보 유형의 의미 간섭은 직교 뷰 분해로만 제거 가능하다.

## 📖 분석

## 핵심 기여

고정 입도·정적 스키마에 의존하는 기존 장기 기억 시스템의 한계를 진단한다. 선호·이벤트·제약·시간 갱신 같은 이질적 정보가 단일 혼합 표현에 담기면 **의미 간섭(semantic interference)**이 발생하여 top-K 검색이 노이즈에 취약해지고 관련 증거가 누락된다. 해법으로 기억을 **직교 뷰(orthogonal views)**로 분해하고 뷰 구성 자체를 **자기 설정**하는 AutoViewMem을 제안한다.

## Wiki 축적과의 관계

[[structure-grounded-chunking]] 계열의 기억 도메인 확장이다 — 스프레드시트 QA가 격자 구조 해석을 요구하듯 장기 기억 QA는 뷰 분해를 요구하며, 평면적 표현이 검색에 필요한 구조 정보를 파괴한다는 공통 원리를 강화한다. [[memory-fragmentation-failure]]와의 역관계도 중요하다: 과분절과 과혼합 양쪽이 검색을 저해하며, 직교 뷰는 적정 분해점을 찾는 제3의 길이다. [[query-deferred-representation-contract]]의 연장선에서 뷰 선택이 질의 조건으로 위임되고, [[value-differential-memory-management]]의 차등 관리가 정보 유형별 직교 분해로 구체화된다. [[adaptive-forgetting]]의 시간 갱신도 전용 뷰에서 처리 가능해진다.

핵심 기여는 기억 스키마 설계가 설계 시점 고정 선택이 아니라 런타임 적응 대상임을 보인 점이다 — [[adaptive-inference]] 패턴이 표현 계층까지 확장된 사례다.

## 🔗 관련 논문

- Q&A on Any Spreadsheet Requires Interpreting Its Grid Structure (2026-09-21)
- Caption-once, Frames-on-Demand: Visual-Need Routing for Budget-Aware Agentic Memory (2026-09-12)
- Does Your Agent's Memory Survive a Model Upgrade? A Controlled Study of Model Upgrades (2026-09-08)
- ADEMA: A Knowledge-State Orchestration Architecture for Long-Horizon Knowledge Work (2026-04-30)
- LongSeeker: Elastic Context Orchestration for Long-Horizon Search Agents (2026-05-08)

## 🏷️ 엔티티

- [[entities/orthogonal-memory-views.md|orthogonal-memory-views]]
- [[entities/semantic-interference-decoupling.md|semantic-interference-decoupling]]
- [[entities/self-configuring-memory-schema.md|self-configuring-memory-schema]]
- [[entities/memory-management.md|memory-management]]
- [[entities/structure-grounded-chunking.md|structure-grounded-chunking]]
- [[entities/query-deferred-representation-contract.md|query-deferred-representation-contract]]
- [[entities/value-differential-memory-management.md|value-differential-memory-management]]
- [[entities/adaptive-forgetting.md|adaptive-forgetting]]
- [[entities/memory-fragmentation-failure.md|memory-fragmentation-failure]]
- [[entities/semantic-structure-flattening.md|semantic-structure-flattening]]
- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/memory-representation-spectrum.md|memory-representation-spectrum]]

## 📐 개념

- [[concepts/orthogonal-memory-views.md|orthogonal-memory-views]]
- [[concepts/semantic-interference-decoupling.md|semantic-interference-decoupling]]
- [[concepts/self-configuring-memory-schema.md|self-configuring-memory-schema]]
- [[concepts/fixed-granularity-limitation.md|fixed-granularity-limitation]]

---
_LLM 분석으로 생성됨_
