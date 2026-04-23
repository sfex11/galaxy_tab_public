# Failure of contextual invariance in gender inference with large language models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-26
**링크**: http://arxiv.org/abs/2603.23485v1

## 💡 핵심 인사이트

LLM의 성별 추론에서 이론적으로 무정보적인 최소 맥락 도입만으로도 출력이 체계적으로 변화하며, 탈맥락화된 설정에서의 성별 고정관념 상관이 사라져 기존 편향 평가 방법론의 맥락적 불변성 가정이 무효함을 실증한다.

## 📖 분석

## Failure of Contextual Invariance in Gender Inference with Large Language Models

본 논문은 LLM의 출력이 과제의 맥락적으로 동등한 표현(contextually equivalent formulations) 하에서 안정적이라는 표준 평가 관행의 가정을 검증한다. 성별 추론(gender inference) 과제에서 통제된 대명사 선택 과제(controlled pronoun selection task)를 사용하여, 이론적으로 무정보적인(theoretically uninformative) 최소한의 담화 맥락을 도입했을 때 모델 출력에 크고 체계적인 변화가 발생함을 보인다.

### 핵심 발견

탈맥락화된(decontextualized) 설정에서 관찰되던 문화적 성별 고정관념과의 상관관계가, 맥락이 도입되면 약화되거나 사라진다. 이는 **맥락적 불변성(contextual invariance)**의 실패를 의미하며, LLM 평가에서 단순한 프롬프트 변형이 결과를 근본적으로 바꿀 수 있음을 시사한다.

### 연구 의의

이 결과는 LLM의 성별 편향 평가 방법론에 중요한 함의를 갖는다. 기존 벤치마크가 탈맥락화된 설정에서 편향을 측정하는 경우가 많은데, 실제 사용 환경에서는 맥락에 따라 편향 패턴이 질적으로 달라질 수 있다. 이는 [[concepts/gender-bias.md|gender bias]] 연구의 평가 프레임워크 자체를 재고해야 할 필요성을 제기한다.

### 기존 Wiki와의 연결

- **[[concepts/gender-bias.md|gender bias]]**: ConGA 프레임워크가 기계번역에서의 성별 편향 주석 가이드라인을 다뤘다면, 본 논문은 LLM의 성별 추론 자체의 맥락 민감성을 다루어 편향 연구의 다른 측면을 조명한다.
- **[[concepts/prompt-engineering.md|prompt engineering]]**: 프롬프트의 미세한 변형이 출력을 크게 바꾼다는 발견은 프롬프트 엔지니어링의 견고성(robustness) 문제와 직결된다.
- **[[concepts/llm-benchmark.md|llm benchmark]]**: 벤치마크 설계 시 맥락적 불변성 가정의 위험성을 경고하는 사례로, 평가 방법론 연구에 기여한다.

## 🔗 관련 논문

- 2026 04 10 appear2meaning a cross cultural benchmark for stru
- 2026 04 10 syntax is easy semantics is hard evaluating llms f

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/gender-bias.md|gender-bias]]
- [[concepts/prompt-engineering.md|prompt-engineering]]
- [[concepts/llm-benchmark.md|llm-benchmark]]

---
_LLM 분석으로 재생성됨_
