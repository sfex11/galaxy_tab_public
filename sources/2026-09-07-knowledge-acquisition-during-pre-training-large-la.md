# Knowledge Acquisition During Pre-training? Large Language Models Learn Better With Auxiliary Views

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-07
**링크**: http://arxiv.org/abs/2609.04180v1

## 💡 핵심 인사이트

사전학습 지식 습득은 토큰 총량의 문제가 아니라 고정 예산 내 반복과 보조 뷰의 배분 문제이며, 보조 뷰의 이득은 배치 크기라는 옵티마이저 조건에 의존한다.

## 📖 분석

## 핵심 발견

LLM이 사전학습에서 지식을 습득하는 메커니즘을 통제 실험으로 인과적으로 분리한다. 반복(repetition)은 지식 습득의 필요조건이지만, 의역(paraphrasing)의 이득은 작은 배치 크기에서만 유의미하다 — 의역의 한계 효용이 옵티마이저 그래디언트 동역학과 결합되어 나타남을 의미한다. 더 중요하게, 토큰 예산을 고정한 상태에서 문서 반복에 할당된 토큰을 보조 뷰로 재배분하면 학습이 향상된다.

## 기존 Wiki와의 관계

- [[auxiliary-views]]: 이 논문이 최초 정의를 제공한다 — 지식의 재구성된 뷰가 단순 데이터 증강이 아닌 인과적 학습 원천이라는 조작적 정의.
- [[training-data-pruning]]: 데이터 최적화 축을 '무엇을 뺄 것인가'에서 '고정 예산 내 무엇으로 채울 것인가'로 전환.
- [[token-budget-reallocation]]: 토큰을 '소비량'이 아닌 '뷰 구성의 설계 변수'로 재정의하는 최초의 인과 근거.
- [[batch-size-gradient-redundancy]]: 의역 효과의 배치 크기 조건부성이 이 개념의 직접적 실증 근거.
- [[fact-access-decoupling]]: 보조 뷰가 사실 저장이 아닌 접근 경로의 다각화 메커니즘임을 시사.
- [[entity-surface-form]]: 비엄격 기억 연구의 다중 표면 형식 개념과 훈련 데이터 구성 차원에서 수렴.
- [[implicit-curriculum]]: '모델이 무엇을 언제 배우는가'라는 사전학습 커리큘럼 문제의 인과적 후속.

## 핵심 통찰

토큰 예산은 균질한 자원이 아니라 뷰의 구성 문제다 — 같은 토큰이라도 반복과 재구성 중 어디에 배분되는가가 지식 습득의 인과 경로를 결정한다.

## 🔗 관련 논문

- Revisiting Non-Verbatim Memorization in Large Language Model
- Knowledge Acquisition During Pre-training? Large Language Models Learn

## 🏷️ 엔티티

- [[entities/auxiliary-views.md|auxiliary-views]]
- [[entities/training-data-pruning.md|training-data-pruning]]
- [[entities/token-budget-reallocation.md|token-budget-reallocation]]
- [[entities/synthetic-data-generation.md|synthetic-data-generation]]

## 📐 개념

- [[concepts/implicit-curriculum.md|implicit-curriculum]]
- [[concepts/batch-size-gradient-redundancy.md|batch-size-gradient-redundancy]]
- [[concepts/fact-access-decoupling.md|fact-access-decoupling]]
- [[concepts/entity-surface-form.md|entity-surface-form]]

---
_LLM 분석으로 생성됨_
