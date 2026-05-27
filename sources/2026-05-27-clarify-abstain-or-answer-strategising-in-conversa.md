# Clarify, Abstain or Answer? Strategising in Conversation with Belief-Augmented Generation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-27
**링크**: http://arxiv.org/abs/2605.25831v1

## 💡 핵심 인사이트

LLM의 신념 상태(P(belief|prompt))를 사후 평가 지표가 아닌 추론 시점의 생성 제약으로 재정의한다. 기존 연구가 외부 드래프 모델의 분포를 추정치지로 삼아 문제를 해결했듯이, BAG은 모델 자신의 분포 P(y|prompt) 내에서 신념 상태를 조작하여 제약을 가하는 방식으로, 외부 의존성을 원천적으로 제거한다.

## 📖 분석

# belief-augmented-generation

**카테고리**: 미분류
**생성일**: 2026-05-27

## 정의
LLM이 정의한 텍스트 분포 P(y)는 K번 샘플링으로 추출 가능한 **신념 상태(belief state)** P(belief|prompt)의 확률적 표현이다. Belief-Augmented Generation (BAG)은 이 신념 상태를 사후 평가 대상이 아닌 **추론 시점의 생성 제약**으로 직접 사용하는 방법론이다. 베이즈ian 인자화 P(response|prompt) = P(response|belief) × P(belief|prompt)의 분해를 통해, 기존의 추측 디코딩(예: speculative decoding)이 외부 드래프 모델에 의존하던 문제를 해결한다.

## 공통 주제: 신념 상태의 생성 제약으로의 전환
기존 연구는 LLM의 신념 상태를 (1) 사후 평가용 지표, (2) 추론 시점 선택적 토큰 선택, (3) 도구 호출 시 프롬프트 기반 제약이라는 세 가지로만 취급한다. 이 세 경로 모두 외부 개입(수동 검증, 도구 사용, 프롬프트 엔지니어링)을 요구한다. BAG은 신념 상태를 추론 시점의 내부 제약으로 격상시킴으로, 외부 루프라인 대신 프롬프트 변형 없이 생성을 직접 제어한다.

## 관련 논문
- sources/2026-05-27-clarify-abstain-or-answer-strategising-in-conversation-with-belief.md

## 관련 엔티티
- [[entities/output-epistemic-reliability|output-epistemic-reliability]]: BAG은 모델의 신념 상태 기반 생성 제어를 통해 산출물의 인식론적 신뢰도를 직접 향상시킨다.

## 관련 개념
- concepts/belief-state-as-constraint: LLM의 내부 불확실성을 사후 평가 대상이 아닌 추론 시점의 생성 제약으로 전환하는 패러다임이다.
- concepts/inference-time-behavior-control: BAG은 외부 검증자나 가드레일이 아닌 모델 자신의 신념 상태에 기반하여 생성을 직접 제어하는 inference-time behavior control의 구체적 구현이다.
- concepts/distribution-internal-optimization: BAG은 P(y) 내부에서 신념 상태를 조작하여 제약을 가하는 방식으로, 분포 외부 탐색 없이도 분포 내부에서 정확도와 다양성을 동시 달성하는 구조적 메커니즘을 제공한다.
- concepts/speculative-decoding: 기존 추측 디코딩이 외부 드래프 모델의 분포 P(belief|prompt)를 추정치지로 삼는 데 반해, BAG은 모델 자신의 분포 P(y|prompt) 내에서 신념 상태를 직접 활용하여 외부 의존성을 원천적으로 제거한다.
- concepts/template-constrained-decoding: 기존 방식이 고정된 템플릿으로 생성을 제약하는 데 반해, BAG은 확률적 신념 상태(응답 가능성 분포)를 통해 훨씬하지만 유연하게 생성을 유도하는 확률적 제약으로 대비된다.

## 🏷️ 엔티티

- [[entities/belief-augmented-generation.md|belief-augmented-generation]]
- [[entities/belief-state-grounding.md|belief-state-grounding]]

## 📐 개념

- [[concepts/belief-state-as-constraint.md|belief-state-as-constraint]]

---
_LLM 분석으로 생성됨_
