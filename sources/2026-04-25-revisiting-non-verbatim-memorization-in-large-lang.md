# Revisiting Non-Verbatim Memorization in Large Language Models: The Role of Entity Surface Forms

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-25
**링크**: http://arxiv.org/abs/2604.21882v1

## 💡 핵심 인사이트

LLM의 비축어적 사실 기억은 엔티티에 대한 정규화된 지식이 아니라 특정 표면 형태와의 빈도 기반 연관성이며, 기존 기억 벤치마크는 이 접근성 편향을 통제하지 못해 사실 지식을 과대평가한다.

## 📖 분석

# RedirectQA: 엔티티 표면 형태가 비축어적 기억 평가에 미치는 영향

## 문제 제기

기존 엔티티 기반 QA 벤치마크는 각 엔티티를 단일 정규 표면 형태(canonical surface form)로만 질의하여, '사실 기억'과 '특정 이름을 통한 접근성'을 분리하지 못하는 근본적 한계를 가진다. 이로 인해 LLM이 사실을 진정으로 기억하는지, 아니면 빈번한 표면 형태와의 연관성을 학습한 것인지 구분이 불가능하다.

## 핵심 방법

RedirectQA는 위키백과 리다이렉트 정보를 활용하여 각 엔티티에 다중 표면 형태를 부여하는 데이터셋이다. 동일 사실에 대해 정규명, 약어, 이명, 대체 표기 등으로 질의하여 응답 일관성을 측정함으로써, 기억의 표면 형태 의존성을 정량화한다.

## 기존 Wiki와의 연결

이 논문은 [[concepts/fact-memorization|fact-memorization]] 개념에 구조적 도전을 제기한다. 기존 연구가 '사실을 안다/모른다'의 이분법으로 접근했다면, RedirectQA는 기억이 표면 형태 빈도에 편향된 연속체임을 보여준다. 이는 [[concepts/shortcut-learning|shortcut-learning]]의 새로운 변형 — 빈번한 표면 형태를 단서로 삼아 정답에 도달하는 패턴 — 으로 해석될 수 있다.

또한 [[concepts/implicit-curriculum|implicit-curriculum]]과도 연결된다: 훈련 코퍼스에서 특정 표면 형태의 빈도가 암묵적 커리큘럼을 형성하며, 이것이 곧 LLM이 '알고 있다고 판단되는' 사실의 범위를 결정한다는 점에서 사실 기억의 상한선이 데이터 분포에 의해 좌우됨을 시사한다.

## 🏷️ 엔티티

- [[entities/llm.md|llm]]
- [[entities/redirectqa.md|redirectqa]]

## 📐 개념

- [[concepts/entity-surface-form.md|entity-surface-form]]
- [[concepts/fact-access-decoupling.md|fact-access-decoupling]]
- [[concepts/fact-memorization.md|fact-memorization]]
- [[concepts/shortcut-learning.md|shortcut-learning]]
- [[concepts/implicit-curriculum.md|implicit-curriculum]]

---
_LLM 분석으로 생성됨_
