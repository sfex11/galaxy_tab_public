# Exploring Language-Agnosticity in Function Vectors: A Case Study in Machine Translation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-23
**링크**: http://arxiv.org/abs/2604.19678v1

## 💡 핵심 인사이트

Function vector는 언어 간 작업 전이를 지원하는 부분적 언어 비의존성을 보이지만, 언어별 크기 변동이 존재하여 작업 추상화가 언어 특정 표현과 완전히 분리되지 않음을 시사한다.

## 📖 분석

# Function Vector의 언어 비의존성: 기계 번역 사례 연구

## 핵심 발견

Function Vector(FV)는 in-context learning 중 모델 활성화에서 추출된 작업의 벡터 표현이다. 본 논문은 다국어 LLM 3종(디코더 전용)에서 번역 FV가 언어 비의존성(language-agnosticity)을 보이는지 기계 번역을 사례로 검증한다.

### 부분적 언어 비의존성

단일 영어→목표어 방향에서 추출한 번역 FV가 역방향 및 제로샷 번역 방향으로 일반화됨을 확인했다. 그러나 FV의 크기(magnitude)와 효과성은 언어에 따라 변동하며, 완전한 언어 독립성은 관찰되지 않았다. 이는 작업 추상화가 언어 특정 표현과 부분적으로 결합되어 있음을 시사한다.

## Wiki와의 연결

### mechanistic-interpretability와의 관계
기존 Wiki의 `representation-steering`이 활성화 스티어링의 안전성 한계(사후적 가드레일 한계, 에이전트 간 공격 증폭)를 강조했다면, 본 논문은 FV가 캡처하는 작업 표현 자체가 언어적으로 완전히 분리되지 않음을 보여준다. 이는 `inter-agent-attack-amplification` 맥락에서 다국어 환경에서의 스티어링 전파가 언어별로 비대칭적으로 작동할 수 있음을 시사한다.

### marginal-distribution-ceiling과의 연결
FV의 언어별 크기 변동은 주변 분포 P(y)가 언어마다 다른 지형을 가진다는 `주변 분포 성능 상한선` 개념과 일치한다. FV가 P(y)의 구조에 의존한다면, 언어 간 FV 전이의 한계는 본질적으로 P(y) 차이에서 기인할 수 있다.

### in-context-learning과의 관계
Wiki의 `in-context-learning` 개념을 메커니스틱 관점에서 구체화한다. ICL이 작업을 수행하는 메커니즘이 단일 방향의 데모에서 추출한 FV로 교차 방향 전이가 가능하다는 것은, ICL이 언어 구문보다 의미적 작업 구조를 더 강하게 인코딩함을 의미한다.

## 🔗 관련 논문

- 2026-04-11-what-drives-representation-steering-a-mechanistic-.md
- 2026-03-27-analysing-the-safety-pitfalls-of-steering-vectors.md
- 2026-04-10-evaluating-in-context-translation-with-synchronous.md

## 🏷️ 엔티티

- [[entities/llm.md|llm]]
- [[entities/transformer.md|transformer]]

## 📐 개념

- [[concepts/function-vector.md|function-vector]]
- [[concepts/language-agnostic-function-vector.md|language-agnostic-function-vector]]
- [[concepts/mechanistic-interpretability.md|mechanistic-interpretability]]
- [[concepts/in-context-learning.md|in-context-learning]]
- [[concepts/machine-translation.md|machine-translation]]
- [[concepts/multilingual-nlp.md|multilingual-nlp]]
- [[concepts/representation-steering.md|representation-steering]]
- [[concepts/activation-patching.md|activation-patching]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-04-22-dual-alignment-between-language-model-layers-and-h]]: 둘 다 LLM 내부 표현의 구조적 특성을 조사하며, 하나는 층별 활성화와 인간 문장 처리의 정렬을, 다른 하나는 함수 벡터의 언어 비의존성을 분석한다.
