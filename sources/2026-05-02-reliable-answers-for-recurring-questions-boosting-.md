# Reliable Answers for Recurring Questions: Boosting Text-to-SQL Accuracy with Template Constrained Decoding

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-02
**링크**: http://arxiv.org/abs/2604.28028v1

## 💡 핵심 인사이트

실제 워크로드에서 질의 패턴이 반복된다는 도메인 특성을 활용해, LLM의 자유로운 생성을 템플릿 구조로 제약함으로써 정확성과 유효성을 동시에 확보하는 접근은, 출력 공간의 구조적 설계가 번역 품질 향상에 모델 능력 향상과 동등한 기여를 할 수 있음을 보여준다.

## 📖 분석

# Template Constrained Decoding (TeCoD)

**카테고리**: AI/ML — 구조화된 출력 생성
**생성일**: 2026-05-02

## 정의

TeCoD는 레이블된 워크로드에서 질의 패턴의 반복성(recurrence)을 활용하여, 역사적 쿼리를 템플릿으로 변환하고 이를 LLM 디코딩의 구조적 제약으로 사용하는 Text-to-SQL 시스템이다. 복잡하거나 미경험 스키마에서의 부정확성과 무효 SQL 생성 문제를 해결한다.

## 기존 Wiki와의 관계

### natural-language-to-formal-language에의 기여
기존에 '의미론적 번역의 어려움'으로만 진단되던 [[concepts/natural-language-to-formal-language|NL→형식언어 변환]] 문제에 대해, TeCoD는 정적 템플릿 추출을 통해 출력 공간을 사전 제약하는 구조적 해법을 제공한다. [[entities/from-research-question-to-scientific-workflow-leve|3층 아키텍처]]가 '의도→명세→실행'으로 번역을 분해했다면, TeCoD는 실행 계층의 출력 공간 자체를 템플릿으로 좁혀 번역 간극을 물리적으로 축소한다.

### algorithm-system-translation-gap과의 연결
[[entities/unifying-sparse-attention-with-hierarchical-memory|알고리즘-시스템 변환 간극]]이 희소 어텐션 분야에서 문제시되던 것과 동일한 구조 — 알고리즘적 이상과 시스템 구현 사이의 간극 — 이 NL→SQL에서도 현현한다. TeCoD는 템플릿 제약을 통해 이 간극을 '허용된 출력의 집합'으로 좁힘으로써, 간극 자체를 해소하기보다 간극이 치명적이 되지 않도록 출력 공간을 재설계하는 전략을 취한다.

### token-efficiency 및 speculative-decoding과의 관계
[[entities/select-to-think-unlocking-slm-potential-with-local|토큰 선택 전략]]이 SLM에서 토큰 수준에서 효율화를 달성했다면, TeCoD는 템플릿 수준에서 디코딩 공간을 사전 축소하여 유효 토큰 탐색 범위 자체를 구조적으로 제한한다. [[entities/speculative-decoding|사양적 디코딩]]이 드래프트 모델로 탐색 공간을 줄이는 것과 유사하지만, TeCoD는 모델이 아닌 도메인 특화 템플릿을 제약원으로 사용한다는 점이 차별적이다.

## 핵심 메커니즘

1. **패턴 마이닝**: 레이블된 워크로드에서 반복되는 SQL 구조를 템플릿으로 추출
2. **템플릿 매칭**: 입력 자연어 질의를 가장 유사한 템플릿에 매핑
3. **제약 디코딩**: 템플릿이 허용하는 구조적 위치에만 LLM이 토큰을 생성하도록 강제

## 관련 논문

- [[sources/2026-05-02-reliable-answers-for-recurring-questions-boosting-t.md|Reliable Answers for Recurring Questions: Boosting Text-to-SQL Accuracy with Template Constrained Decoding]]

## 🔗 관련 논문

- 2026 04 26 from research question to scientific workflow leve
- 2026 05 01 select to think unlocking slm potential with local
- 2026 05 01 unifying sparse attention with hierarchical memory

## 🏷️ 엔티티

- [[entities/template-constrained-decoding.md|template-constrained-decoding]]
- [[entities/text-to-sql.md|text-to-sql]]
- [[entities/natural-language-to-formal-language.md|natural-language-to-formal-language]]
- [[entities/algorithm-system-translation-gap.md|algorithm-system-translation-gap]]
- [[entities/token-efficiency.md|token-efficiency]]
- [[entities/speculative-decoding.md|speculative-decoding]]

## 📐 개념

- [[concepts/query-pattern-recurrence.md|query-pattern-recurrence]]
- [[concepts/template-constrained-decoding.md|template-constrained-decoding]]
- [[concepts/constrained-decoding.md|constrained-decoding]]
- [[concepts/output-space-pruning.md|output-space-pruning]]

---
_LLM 분석으로 생성됨_
