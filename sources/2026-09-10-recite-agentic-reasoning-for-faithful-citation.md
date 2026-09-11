# ReCite: Agentic Reasoning for Faithful Citation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-10
**링크**: http://arxiv.org/abs/2609.09156v1

## 💡 핵심 인사이트

인용 연구의 병목이 '조작'에서 '잘못된 귀속'으로 이동한 가운데, 의미 유사도라는 표면 신호를 에이전틱 추론 기반 주장-지지 검증으로 대체하는 것이 신뢰할 수 있는 인용의 조건이다.

## 📖 분석

ReCite는 학술 인용 자동화의 문제 지형이 '존재하지 않는 논문 조작(fabrication)'에서 '실존 논문의 잘못된 귀속(misattribution)'으로 이동했음을 진단하고, 의미 유사도 기반 선택을 에이전틱 추론 기반 검증으로 대체하는 프레임워크를 제시한다.

본 논문은 [[citation-claim-decoupling]]의 생성 측 해법이다. 'Cited but Not Verified'([[citation-verifiability-gap]], [[source-attribution-evaluation]])가 평가 측에서 인용-주장 탈동기화를 진단했다면, ReCite는 검증을 생성 파이프라인 내부로 이동시켜 사후 평가와 사전 예방의 양축을 완성한다. 의미 유사도는 화제 근접성만 측정할 뿐 주장 지지를 보장하지 못한다는 점에서 [[single-surface-signal-insufficiency]]의 인용 도메인 발현이며, 이를 [[reasoning-conditioned-retrieval]]로 극복하는 구체적 구현이기도 하다.

또한 '진짜 논문을 인용했지만 근거가 아닌' 실패가 행동 제어·능력 평가로 포착 불가능한 산출물 수준 결함임을 보여 [[output-epistemic-reliability]]를 강화하고, [[autoresearch]] 파이프라인의 인용 품질 병목을 직접 공략하며, RAG([[retrieval-augmented-generation]])가 조작은 해소했으나 귀속 정확성은 남긴다는 한계 정밀화를 제공한다.

## 🔗 관련 논문

- Cited but Not Verified: Parsing and Evaluating Source Attribution in LLMs

## 🏷️ 엔티티

- [[entities/citation-claim-decoupling.md|citation-claim-decoupling]]
- [[entities/citation-verifiability-gap.md|citation-verifiability-gap]]
- [[entities/source-attribution-evaluation.md|source-attribution-evaluation]]
- [[entities/output-epistemic-reliability.md|output-epistemic-reliability]]
- [[entities/reasoning-conditioned-retrieval.md|reasoning-conditioned-retrieval]]
- [[entities/single-surface-signal-insufficiency.md|single-surface-signal-insufficiency]]
- [[entities/autoresearch.md|autoresearch]]
- [[entities/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[entities/citation-hallucination.md|citation-hallucination]]

## 📐 개념

- [[concepts/misattribution-over-fabrication-shift.md|misattribution-over-fabrication-shift]]
- [[concepts/claim-support-verification.md|claim-support-verification]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-09-molecular-déjà-vu-digit-level-retrieval-of-publish]]: 모두 검색·인용이 실제 이해나 근거를 담보하지 않는 문제를 다루며, 분자 특성 값의 축자적 검색 감사와 인용의 주장-지지 검증이라는 두 도메인 발현이다.
- → [[sources/2026-09-09-necessary-or-sufficient-evaluating-llm-explanation]]: 둘 다 명시된 근거(설명·인용)와 실제 증거의 정합을 의미 유사도 같은 표면 신호 대신 행동적·에이전틱 검증으로 확인해야 한다고 주장한다.
