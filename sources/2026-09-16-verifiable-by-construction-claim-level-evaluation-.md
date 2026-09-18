# Verifiable by Construction: Claim-Level Evaluation of Verbatim Citation in Clinical Question Answering

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-16
**링크**: http://arxiv.org/abs/2609.15964v1

## 💡 핵심 인사이트

인용의 검증 가능성은 사후 평가로 확보하는 것이 아니라, 주장 단위 verbatim 재현이라는 구성 제약으로 원천적으로 달성할 수 있다 — 인용-근거 탈동기화를 감지하는 대신 구조적으로 불가능하게 만드는 것이다.

## 📖 분석

## Verifiable by Construction: Claim-Level Verbatim Citation

임상 QA에서 인용의 검증 가능성을 '사후 검증 대상'에서 '구성 시점 보장'으로 전환하는 논문. 기존 LLM 시스템의 인용이 광범위한 텍스트를 가리켜 검증 비용이 시간에 쫓기는 임상의에게 전가되었다면, 본 논문은 주장 단위(claim-level)의 verbatim 인용을 참조 자료에서 제공함으로써 사용자가 다른 문서를 열 필요 없이 답변을 검증하게 한다.

### 기존 Wiki와의 관계

**[[citation-claim-decoupling]]**의 해법 스펙트럼을 확장한다. Cited but Not Verified가 평가 측 진단(AST 파싱 기반 접근성·관련성·사실 일관성 검사), ReCite가 생성 시점 에이전틱 추론 검증이었다면, 본 논문은 제3의 경로 — verbatim 재현 제약 — 를 제시한다. 인용을 원문의 부분 집합으로 강제하면 인용과 참조 문서의 탈동기화가 구조적으로 불가능해지며, 인용 환각 탐지도 원문 대조로 단순화된다.

**[[source-attribution-evaluation]]**의 접근성 축을 극단화한다. 3차원 프레임에서 '접근성'을 '문서 열기'가 아닌 '인용 자체가 근거의 실체'로 재정의하여, 평가 단위를 문서 수준에서 주장 수준으로 세분화한다.

**[[grounded-clinical-qa]]**에 사용자 모델 차원을 추가한다. HealthNLP_Retrievers가 파이프라인 구조로 근거 추적성을 확보했다면, 본 논문은 '시간 제약 하 임상의'라는 수신자 제약을 평가 설계에 직접 내장한다.

### 남는 문제

verbatim 인용도 절삭(문맥 제거)에 의한 왜곡 가능성은 남는다. [[single-surface-signal-insufficiency]] 관점에서 claim-level 세분화가 표면 신호의 충분성을 어디까지 높이는지는 향후 검증 과제다.

## 🔗 관련 논문

- Cited but Not Verified: Parsing and Evaluating Source Attribution in L
- ReCite: Agentic Reasoning for Faithful Citation
- HealthNLP_Retrievers at ArchEHR-QA 2026: Cascaded LLM Pipeline for Gro
- Can "AI" Be a Doctor? A Study of Empathy, Readability, and A

## 🏷️ 엔티티

- [[entities/grounded-clinical-qa.md|grounded-clinical-qa]]
- [[entities/medical-ai.md|medical-ai]]
- [[entities/evidence-grounded-diagnosis.md|evidence-grounded-diagnosis]]
- [[entities/evidence-traceability.md|evidence-traceability]]
- [[entities/output-epistemic-reliability.md|output-epistemic-reliability]]
- [[entities/clinical-readability-evaluation.md|clinical-readability-evaluation]]

## 📐 개념

- [[concepts/citation-claim-decoupling.md|citation-claim-decoupling]]
- [[concepts/source-attribution-evaluation.md|source-attribution-evaluation]]
- [[concepts/single-surface-signal-insufficiency.md|single-surface-signal-insufficiency]]
- [[concepts/claim-support-verification.md|claim-support-verification]]
- [[concepts/citation-verifiability-gap.md|citation-verifiability-gap]]
- [[concepts/citation-hallucination.md|citation-hallucination]]
- [[concepts/ast-citation-parsing.md|ast-citation-parsing]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-17-verifiable-social-reasoning-for-llm-assistants]]: ground truth가 부재하거나 검증 비용이 큰 영역(임상 인용, 사회적 추론)에서 검증 가능성을 평가 설계 단계에서 구축한다는 공통 전략을 취한다.
- → [[sources/2026-09-17-enhancing-accessibility-of-medical-texts-through-l]]: 임상 텍스트를 대상으로 LLM을 적용하며, 각각 검증 가능한 인용과 환자 접근성이라는 신뢰성 요건을 충족시키려 한다.
