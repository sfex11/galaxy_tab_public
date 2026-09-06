# Knowledge Acquisition During Pre-training? Large Language Models Learn Better With Auxiliary Views

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-06
**링크**: http://arxiv.org/abs/2609.04180v1

## 💡 핵심 인사이트

동일 문서 반복은 지식 습득의 필요조건이지만, 고정 토큰 예산 내에서 반복을 지식의 재구성(보조 뷰)으로 재할당하면 학습이 더 잘 된다 — '같은 형태를 여러 번'보다 '다른 형태로 한 번 더'가 인과적으로 우월하다.

## 📖 분석

# Auxiliary Views: 사전학습 지식 습득의 보조 뷰

**핵심 발견**: 사전학습 중 LLM의 지식 습득에서 '동일 문서 반복'은 필요조건이지만, 고정 토큰 예산 내에서 반복 토큰 일부를 **보조 뷰(지식의 재구성·의역)**로 재할당하면 학습이 인과적으로 향상된다. 즉 "같은 형태를 여러 번 보는 것"보다 "다른 형태로 한 번 더 보는 것"이 효과적이다.

**두 정량적 결과**:
1. 반복은 습득에 필수이나, 의역(paraphrasing)의 이득은 소규모 배치에서만 나타남 — 대규모 배치에서는 의역의 그래디언트 신호가 원본과 중복됨
2. 토큰 예산 고정 조건에서 반복→보조 뷰 재할당이 순수 반복 대비 학습을 개선

**Wiki 연결**:
- [[concepts/entity-surface-form.md|entity surface form]]과의 인과적 대응: RedirectQA가 평가 단계에서 표면 형식 접근성과 사실 저장의 혼재를 진단했다면, 본 논문은 사전학습 단계에서 다중 표면 형식(보조 뷰)의 인과적 기여를 통제 실험으로 입증한다. 평가-훈련 양 단계를 잇는 사슬이 완성된다.
- [[concepts/fact-access-decoupling.md|fact access decoupling]]: 동일 형태 반복이 저장 강건성을, 보조 뷰가 다양한 접근 경로를 공급함을 시사
- [[concepts/implicit-curriculum.md|implicit curriculum]]: '무엇을 언제 학습하는가'에 데이터 구성의 인과적 축 추가
- [[concepts/training-data-pruning.md|training data pruning]]: 데이터 최적화를 '빼기'에서 '고정 예산 내 재구성으로 채우기'로 확장

**시사점**: 반복률 최적화와 재구성률 최적화는 분리 가능한 독립 제어 변수이며, Adam's Law의 텍스트 빈도 법칙 위에 표현 다양성 차원이 추가된다.

## 🔗 관련 논문

- What do Language Models Learn and When? The Implicit Curriculum
- Revisiting Non-Verbatim Memorization in Large Language Models
- Cram Less to Fit More: Training Data Pruning Improves Memorization
- Adam's Law: Textual Frequency Law on Large Language Models

## 🏷️ 엔티티

- [[entities/auxiliary-views.md|auxiliary-views]]
- [[entities/llm.md|llm]]
- [[entities/implicit-curriculum.md|implicit-curriculum]]
- [[entities/training-data-pruning.md|training-data-pruning]]
- [[entities/synthetic-data-generation.md|synthetic-data-generation]]

## 📐 개념

- [[concepts/entity-surface-form.md|entity-surface-form]]
- [[concepts/fact-access-decoupling.md|fact-access-decoupling]]
- [[concepts/token-budget-reallocation.md|token-budget-reallocation]]
- [[concepts/batch-size-gradient-redundancy.md|batch-size-gradient-redundancy]]

---
_LLM 분석으로 생성됨_
