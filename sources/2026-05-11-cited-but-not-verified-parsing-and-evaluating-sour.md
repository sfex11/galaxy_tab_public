# Cited but Not Verified: Parsing and Evaluating Source Attribution in LLM Deep Research Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-11
**링크**: http://arxiv.org/abs/2605.06635v1

## 💡 핵심 인사이트

인용 구조가 문법적으로 완비되더라도 검증 가능성을 보장하지 못하는 것이 LLM 연구 에이전트의 인식론적 신뢰성의 근본적 결함이며, 이를 해결하기 위해서는 RAG 이전 단계가 아닌 산출물 후 단계에서 재현 가능한 구문 분석 기반 귀속 검증이 필요하다.

## 📖 분석

# Cited but Not Verified: Parsing and Evaluating Source Attribution in LLM Deep Research Agents


LLM 기반 심층 연구 에이전트가 수백 개의 웹 소스를 종합하여 인용을 포함한 보고서를 생성하지만, 그 인용의 검증 가능성은 근본적으로 보장되지 않는다. 기존 접근법은 모델의 자기 인용을 신뢰하거나 RAG를 통해 소스를 검색하되 접근성·관련성·사실 일관성을 검증하지 않는다.

본 논문은 **재현 가능한 AST 파서**를 활용하여 인용 구조를 추출하고, 접근성(accessibility)·관련성(relevance)·사실 일관성(factual consistency)의 3차원에서 출처 귀속을 평가하는 최최초의 프레임워크를 제시한다. 이는 [[ast-citation-parsing]]에 구체적 방법론을 제공하여 기존 빈약한 정의를 '재현 가능한 구문 분석 기반 인용 추출'로 구체화한다.

기존 RAG의 한계를 [[retrieval-as-black-box]] 관점에서 구체화한다 — 검색 전의 문서 품질은 관리하더라도, 검색 후 인용-주장 간의 의미론적 일관성 검증은 블랙박스로 남는다. 또한 [[epistemic-artifact-bound-optimization]]의 인식론적 차원을 확장한다 — 에이전트가 산출물의 형식뿐 아니라 인용의 지식적 유효성 검증마저 외면화하는 구조적 편향을 실증한다. [[output-epistemic-reliability]]의 실패 모드를 구체화하며, [[citation-claim-decoupling]]이 AST 파싱을 통해 실증적으로 측정 가능한 현상임을 보여준다. [[evidence-traceability]]의 한계를 인용 체인의 파서 분석을 통해 노출한다.

## 🔗 관련 논문

- AI Co-Mathematician: Accelerating Mathematicians with Agentic AI

## 🏷️ 엔티티

- [[entities/ast-citation-parsing.md|ast-citation-parsing]]
- [[entities/source-attribution-evaluation.md|source-attribution-evaluation]]
- [[entities/output-epistemic-reliability.md|output-epistemic-reliability]]
- [[entities/citation-claim-decoupling.md|citation-claim-decoupling]]
- [[entities/epistemic-artifact-bound-optimization.md|epistemic-artifact-bound-optimization]]
- [[entities/retrieval-as-black-box.md|retrieval-as-black-box]]
- [[entities/evidence-traceability.md|evidence-traceability]]

## 📐 개념

- [[concepts/citation-verifiability-gap.md|citation-verifiability-gap]]

---
_LLM 분석으로 생성됨_
