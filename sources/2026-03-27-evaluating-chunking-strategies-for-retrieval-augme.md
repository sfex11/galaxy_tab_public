# Evaluating Chunking Strategies For Retrieval-Augmented Generation in Oil and Gas Enterprise Documents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-27
**링크**: http://arxiv.org/abs/2603.24556v1

## 💡 핵심 인사이트

RAG 파이프라인에서 청킹 전략의 선택이 검색 품질의 핵심 결정 요인이며, 도메인 특화 구조 인식 청킹이 단순 고정 크기 분할보다 기업 문서 환경에서 우수한 성능을 보인다.

## 📖 분석

## Evaluating Chunking Strategies For Retrieval-Augmented Generation in Oil and Gas Enterprise Documents

본 논문은 RAG(Retrieval-Augmented Generation) 파이프라인에서 문서 청킹(chunking) 전략이 검색 품질에 미치는 영향을 정량적으로 평가한 실증 연구이다. 석유·가스 산업의 기업 문서 코퍼스를 대상으로, 고정 크기 슬라이딩 윈도우, 재귀적(recursive), 브레이크포인트 기반 시맨틱, 구조 인식(structure-aware) 등 네 가지 청킹 전략의 성능 차이를 비교 분석하였다.

RAG의 효과는 궁극적으로 LLM에 전달되는 컨텍스트의 품질에 의존하며, 이는 청킹 단계에서 결정된다는 점에서 본 연구는 RAG 파이프라인 설계의 핵심 병목을 직접 다룬다. 특히 도메인 특화 문서(기술 보고서, 규정, 매뉴얼 등)에서 구조 인식 청킹이 단순 고정 크기 분할 대비 어떤 이점을 갖는지를 실험적으로 보여준다.

기존 Wiki의 [[retrieval-augmented-generation]] 개념과 직접적으로 연결되며, RAG에서 '검색 품질'이라는 근본 문제를 청킹 관점에서 조명한다. 또한 [[A Systematic Study of Retrieval Pipeline Design for RAG]] 논문과 상호 보완적 관계에 있다—해당 논문이 검색 파이프라인의 전체 설계를 다루었다면, 본 논문은 청킹이라는 특정 단계에 집중한다. 도메인 특화 지식 처리 측면에서 [[knowledge-injection]] 개념과도 관련이 있으며, 기업 문서 처리라는 실용적 맥락에서 LLM 활용의 실질적 과제를 부각시킨다.

## 🔗 관련 논문

- 2026 04 10 a systematic study of retrieval pipeline design fo

## 🏷️ 엔티티

- [[entities/llm.md|LLM]]

## 📐 개념

- [[concepts/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[concepts/text-embedding.md|text-embedding]]

---
_LLM 분석으로 재생성됨_
