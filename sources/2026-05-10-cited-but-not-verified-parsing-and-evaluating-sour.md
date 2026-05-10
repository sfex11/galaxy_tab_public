# Cited but Not Verified: Parsing and Evaluating Source Attribution in LLM Deep Research Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-10
**링크**: http://arxiv.org/abs/2605.06635v1

## 💡 핵심 인사이트

딥 리서치 에이전트가 생성하는 인용은 구문론적으로 완벽해 보이나 의미론적 지지 관계는 검증 불가능하며, 이 간극을 AST 기반 파서로 처음 정량화한 결과 자기 인용 신뢰와 RAG 무검증이라는 기존 양극단이 모두 부적절함이 실증된다.

## 📖 분석

# Cited but Not Verified: 딥 리서치 에이전트의 인용 검증 불가능성

딥 리서치 에이전트가 수백 개의 웹 소스에서 정보를 종합하여 인용된 보고서를 생성하지만, 그 인용은 신뢰성 있게 검증될 수 없다. 기존 접근법은 모델이 정확하게 자기 인용하도록 신뢰하거나(편향 위험), RAG를 사용하되 소스의 접근 가능성·관련성·사실적 일관성을 검증하지 않는다.

본 논문은 재현 가능한 AST 기반 파서를 도입하여 인용 속성을 추출하고 평가하는 최초의 프레임워크를 제시한다. 이는 [[concepts/citation-claim-decoupling|인용-주장 탈동기화]]가 개념적으로만 기술되던 문제에 정량적 측정 도구를 부여하며, [[entities/output-epistemic-reliability|출력물 인식론적 신뢰성]]이라는 에이전트 안전성의 제3축에 구체적 평가 방법론을 제공한다.

## 기존 Wiki와의 연결

- [[entities/autoresearch|autoresearch]]: 자동연구가 '연구 발견→실행'에 집중했다면, 본 논문은 '산출물 검증'을 자동연구 파이프라인의 필수 단계로 끌어올린다.
- [[entities/evidence-traceability|evidence-traceability]]: 임상 QA의 근거 추적성을 넘어 연구 보고서라는 복합 아티팩트 도메인으로 확장한다.
- [[concepts/artifact-bound-optimization|아티팩트 결합 최적화]]의 한계를 구체화한다 — 에이전트가 아티팩트(보고서)의 형식적 사양(인용 포맷)에는 최적화되나, 인용의 의미론적 유효성은 외부에 방치한다.
- [[entities/execution-verification|execution-verification]]: 코드 실행 검증을 넘어 인용 구조의 구문론적·의미론적 검증으로 확장하는 병렬 경로를 제시한다.

## 🔗 관련 논문

- 2026 05 09 why global llm leaderboards are misleading small p
- 2026 05 09 cited but not verified parsing and evaluating sour

## 🏷️ 엔티티

- [[entities/autoresearch.md|autoresearch]]
- [[entities/output-epistemic-reliability.md|output-epistemic-reliability]]
- [[entities/evidence-traceability.md|evidence-traceability]]
- [[entities/execution-verification.md|execution-verification]]
- [[entities/source-attribution-evaluation.md|source-attribution-evaluation]]
- [[entities/ast-citation-parsing.md|ast-citation-parsing]]

## 📐 개념

- [[concepts/citation-claim-decoupling.md|citation-claim-decoupling]]
- [[concepts/citation-hallucination.md|citation-hallucination]]
- [[concepts/artifact-bound-optimization.md|artifact-bound-optimization]]
- [[concepts/citation-verifiability-gap.md|citation-verifiability-gap]]
- [[concepts/epistemic-artifact-bound-optimization.md|epistemic-artifact-bound-optimization]]

---
_LLM 분석으로 생성됨_
