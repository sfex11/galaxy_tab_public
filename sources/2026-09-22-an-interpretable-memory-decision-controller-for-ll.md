# An Interpretable Memory Decision Controller for LLM Agents Based on Three-Signal Complementarity: Decoupling Confidence and Consistency

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-22
**링크**: http://arxiv.org/abs/2609.22043v1

## 💡 핵심 인사이트

메모리 신뢰 판단은 검색 효율과 분리된 독립 결정 계층이어야 하며, 신뢰도(모델 내부 확신)와 정합성(기억 간 일치)은 서로를 대체할 수 없는 직교 신호다.

## 📖 분석

이 논문은 LLM 에이전트 메모리 연구의 사각지대 — 검색 효율에 집중한 나머지 '검색된 메모리를 신뢰할 것인가'의 판단이 누락된 문제 — 를 정면으로 다룬다. 충돌하는 입장이 저장소에 공존할 때 표준 RAG는 맹목적으로 주입해 환각을 증폭시키며, 메모리 주입에 취약한 모델에서는 메모리-free 기준선보다 환각률이 높다는 역설적 실증을 제공한다. 해법으로 신뢰도(confidence)와 정합성(consistency)을 분리한 3신호 보완성 기반의 해석 가능한 메모리 결정 컨트롤러를 제안한다.

Wiki 지형에서의 위치는 명확하다. [[adaptive-validity]]가 메모리의 '현재 타당성'을 개념화했다면 본 논문은 이를 사용 직전 판정 계층으로 구현한다. [[consistency-correctness-divergence]]의 정합성-올바름 분리 원리가 기억-기억 모순 판단으로 이식되며, [[agreement-based-reliability]]의 다중 신호 보완성이 신뢰도·정합성·제3신호의 삼중 구조로 실현된다. [[multi-signal-hallucination-detection]]의 사후 감지형 다중 신호와 대비되어 예방적 배치라는 점이 결정적 차이다. [[closed-book-qa-hallucination]] 관점에서 충돌 메모리 RAG가 메모리 없는 기준선보다 나쁘다는 역설은 오염된 외부 지식이 내부 파라미터 지식보다 해로울 수 있음을 시사한다. [[prewrite-validation]]의 저장 전 검증을 사용 전 검증으로 확장하여, 검증이 쓰기 시점 일회성 이벤트가 아닌 읽기 시점 반복 판단임을 확립한다. [[memory-management]]의 결정 축을 저장·검색·망각에 이어 '수용'이라는 네 번째 축으로 확장한다.

## 🔗 관련 논문

- Domain-Specific Hallucination Detection in Large Language Models
- Quantifying Overclaiming Propensity in Frontier LLM Agents

## 🏷️ 엔티티

- [[entities/adaptive-validity.md|adaptive-validity]]
- [[entities/consistency-correctness-divergence.md|consistency-correctness-divergence]]
- [[entities/agreement-based-reliability.md|agreement-based-reliability]]
- [[entities/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[entities/prewrite-validation.md|prewrite-validation]]
- [[entities/closed-book-qa-hallucination.md|closed-book-qa-hallucination]]
- [[entities/multi-signal-hallucination-detection.md|multi-signal-hallucination-detection]]
- [[entities/memory-management.md|memory-management]]
- [[entities/memory-trust-adjudication.md|memory-trust-adjudication]]
- [[entities/confidence-consistency-decoupling.md|confidence-consistency-decoupling]]

## 📐 개념

- [[concepts/memory-trust-adjudication.md|memory-trust-adjudication]]
- [[concepts/confidence-consistency-decoupling.md|confidence-consistency-decoupling]]
- [[concepts/three-signal-complementarity.md|three-signal-complementarity]]
- [[concepts/use-time-memory-validation.md|use-time-memory-validation]]
- [[concepts/memory-injection-vulnerability.md|memory-injection-vulnerability]]

---
_LLM 분석으로 생성됨_
