# Revisiting Non-Verbatim Memorization in Large Language Models: The Role of Entity Surface Forms

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-26
**링크**: http://arxiv.org/abs/2604.21882v1

## 💡 핵심 인사이트

LLM 사실 기억 평가가 측정한 것은 '사실에 대한 지식'이 아니라 '정규 표면 형식에 대한 반응성'이며, 동일 사실이라도 표면 형식에 따라 검출 가능성이 비약적으로 달라진다.

## 📖 분석

## RedirectQA: 표면 형식에 의존하는 LLM 사실 기억의 근본적 재검토

이 논문은 엔티티 기반 QA가 LLM의 '사실 기억'을 측정한다는 암묵적 전제를 해체한다. 기존 평가는 각 엔티티를 단일 정규 표면 형식(canonical surface form)으로만 질의하므로, 사실 자체의 기억과 특정 이름을 통한 접근성을 분리할 수 없다. RedirectQA는 Wikipedia 리다이렉트 정보를 활용해 각 엔티티에 대해 다중 표면 형식(별칭, 이전 명칭, 변형 등)을 연결함으로써 이 두 축을 분리한다.

### 기존 Wiki와의 관계

Wiki의 [[shortcut-learning]] 개념이 이 논문을 부분적으로 인용하며 "정규 표면 형식이 단축경로로 작동할 가능성"을 제기했으나, RedirectQA가 이를 정량적으로 실증하는 구체적 도구를 제공한다. [[implicit-curriculum]]과의 연결에서도, 사전학습 코퍼스에서 표면 형식의 빈도 분포가 암묵적 커리큘럼을 형성하여 특정 형식에 대한 접근성을 편향시킬 수 있음을 시사한다.

### 핵심 발견과 연결점

[[fact-access-decoupling]]은 단순한 개념적 구분이 아니라 RedirectQA가 최초로 정량화하는 실증적 현상이다. [[training-data-pruning]](Cram Less to Fit More)의 맥락에서도 중요한 시사점을 준다: 훈련 데이터를 가지치기할 때 저빈도 표면 형식이 먼저 제거되면, 사실 기억 자체는 유지되더라도 접근 가능성이 비대칭적으로 저하될 수 있다. [[entity-surface-form]]이 LLM 사실 기억의 검출 가능성을 결정하는 핵심 변수임을 체계적으로 입증한다.

### 방법론적 기여

RoboGrid가 구문·행동·의미를 분리한 것과 유사하게, RedirectQA는 '사실 지식'과 '표면 형식 접근성'을 분리하는 새로운 평가 차원을 제시한다. 기존 벤치마크가 측정하던 것은 '사실 기억'이 아니라 '정규 형식에 대한 반응성'이었을 가능성을 구조적으로 노출한다.

## 🔗 관련 논문

- 2026-04-11-cram-less-to-fit-more-training-data-pruning-improv.md
- 2026-04-12-what-do-language-models-learn-and-when-the-implici.md
- 2026-04-24-diagnosing-cfg-interpretation-in-llms.md
- 2026-04-25-mathduels-evaluating-llms-as-problem-posers-and-so.md

## 🏷️ 엔티티

- [[entities/redirectqa.md|redirectqa]]
- [[entities/llm.md|llm]]
- [[entities/shortcut-learning.md|shortcut-learning]]
- [[entities/fact-access-decoupling.md|fact-access-decoupling]]
- [[entities/entity-surface-form.md|entity-surface-form]]
- [[entities/training-data-pruning.md|training-data-pruning]]

## 📐 개념

- [[concepts/entity-surface-form.md|entity-surface-form]]
- [[concepts/fact-access-decoupling.md|fact-access-decoupling]]
- [[concepts/shortcut-learning.md|shortcut-learning]]
- [[concepts/evaluator-assumption.md|evaluator-assumption]]

---
_LLM 분석으로 생성됨_
