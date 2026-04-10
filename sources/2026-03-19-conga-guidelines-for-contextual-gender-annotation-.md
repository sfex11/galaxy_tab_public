# ConGA: Guidelines for Contextual Gender Annotation. A Framework for Annotating Gender in Machine Translation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-19
**링크**: http://arxiv.org/abs/2603.17962v1

## 💡 핵심 인사이트

성별-중립 언어에서 성별-명시 언어로의 번역 시 발생하는 체계적 남성형 편향을 맥락적 주석 프레임워크로 해결하려는 시도로, MT/LLM의 공정성 평가에 실질적 기준을 제공한다.

## 📖 분석

## ConGA: 맥락적 성별 주석을 위한 가이드라인 프레임워크

본 논문은 기계 번역(MT)과 대규모 언어 모델(LLM)에서 언어 간 성별 처리 문제를 다루는 체계적인 주석 프레임워크 **ConGA**를 제안한다. 특히 영어처럼 문법적 성별이 거의 없는 언어에서 이탈리아어처럼 형태론적 성별 일치가 필수인 언어로 번역할 때 발생하는 비대칭 문제에 주목한다.

### 핵심 문제

MT 시스템은 성별 정보가 불충분할 때 남성형을 기본값으로 사용하는 경향이 있어, 번역 정확도 저하와 성별 편향 강화라는 이중 문제를 야기한다. 이는 단순한 기술적 오류를 넘어 사회적 편향의 재생산이라는 윤리적 문제와 직결된다.

### ConGA 프레임워크의 기여

ConGA는 번역 시 성별 주석을 맥락적으로 수행하기 위한 가이드라인을 제시한다. 문맥에서 성별 정보를 추론할 수 있는 경우와 그렇지 않은 경우를 체계적으로 구분하며, 이를 통해 MT 시스템의 성별 처리 품질을 평가하고 개선할 수 있는 기반을 마련한다.

### 연구 맥락에서의 위치

이 연구는 LLM 기반 번역 시스템의 공정성과 신뢰성 평가라는 측면에서, 기존 Wiki의 **ai-safety** 개념과 밀접하게 연결된다. LLM의 출력 편향을 체계적으로 측정하고 교정하려는 시도이기 때문이다. 또한 평가 벤치마크 구축이라는 관점에서 Appear2Meaning 등 교차문화 벤치마크 연구와도 방법론적 유사성을 공유한다. NLP 평가의 언어적 다양성과 공정성을 동시에 추구한다는 점에서, LLM 평가 연구의 중요한 한 축을 형성한다.

## 🔗 관련 논문

- 2026 04 10 appear2meaning a cross cultural benchmark for stru
- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 10 evaluating in context translation with synchronous

## 📐 개념

- [[concepts/machine-translation.md|machine-translation]]
- [[concepts/gender-bias.md|gender-bias]]

---
_LLM 분석으로 재생성됨_
