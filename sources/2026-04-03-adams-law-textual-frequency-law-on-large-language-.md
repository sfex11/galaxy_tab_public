# Adam's Law: Textual Frequency Law on Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-03
**링크**: http://arxiv.org/abs/2604.02176v1

## 💡 핵심 인사이트

인간 인지의 텍스트 빈도 효과가 LLM에도 적용되며, 고빈도 텍스트 데이터가 프롬프팅과 파인튜닝 모두에서 성능 향상을 이끈다는 Textual Frequency Law를 제안했다.

## 📖 분석

## Adam's Law: Textual Frequency Law on Large Language Models

본 논문은 인간 인지과학에서 검증된 텍스트 빈도(textual frequency) 개념을 LLM에 적용한 새로운 연구 방향을 제시한다. 저자들은 **Textual Frequency Law (TFL)**을 제안하며, LLM의 프롬프팅과 파인튜닝 모두에서 빈도가 높은 텍스트 데이터가 선호되어야 한다고 주장한다.

프레임워크는 세 가지 구성요소로 이루어진다: (1) TFL 법칙 자체의 정의, (2) 텍스트 빈도 측정 방법론, (3) LLM 성능과의 상관관계 검증. 이는 인간의 읽기 속도에서 빈도 효과가 검증된 것과 유사하게, LLM에서도 고빈도 텍스트가 더 나은 성능을 이끌어낸다는 가설을 실험적으로 입증한다.

이 연구는 LLM의 학습 및 추론 메커니즘을 인지과학적 관점에서 분석한다는 점에서 독특하다. 기존 Wiki의 [[scaling-laws]] 연구가 모델 크기와 데이터 양의 관계에 집중했다면, TFL은 데이터의 **질적 속성**(빈도)이 성능에 미치는 영향을 다룬다. 또한 [[prompt-engineering]] 분야에서 프롬프트 설계 시 텍스트 빈도를 고려해야 한다는 실질적 함의를 제공하며, [[training-data-pruning]] 및 [[knowledge-injection]] 연구와도 연결된다—학습 데이터 선별 시 빈도 기반 기준이 효과적일 수 있음을 시사하기 때문이다. [[curriculum-learning]]의 암묵적 커리큘럼 관점에서도, 빈도순 학습이 LLM의 내재적 학습 순서와 관련될 수 있다는 흥미로운 접점을 형성한다.

## 🔗 관련 논문

- 2026 04 11 what do language models learn and when the implici
- 2026 04 11 cram less to fit more training data pruning improv

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/scaling-laws.md|scaling-laws]]
- [[concepts/prompt-engineering.md|prompt-engineering]]
- [[concepts/training-data-pruning.md|training-data-pruning]]
- [[concepts/knowledge-injection.md|knowledge-injection]]
- [[concepts/curriculum-learning.md|curriculum-learning]]
- [[concepts/cognitive-modeling.md|cognitive-modeling]]

---
_LLM 분석으로 재생성됨_
