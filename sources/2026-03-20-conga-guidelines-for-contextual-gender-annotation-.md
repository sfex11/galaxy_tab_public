# ConGA: Guidelines for Contextual Gender Annotation. A Framework for Annotating Gender in Machine Translation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-20
**링크**: http://arxiv.org/abs/2603.17962v1

## 💡 핵심 인사이트

성별 중립 언어에서 성별 표지 언어로의 번역 시 발생하는 체계적 편향 문제를 해결하기 위해, 문맥 기반의 구조화된 성별 주석 프레임워크가 필요하다.

## 📖 분석

## ConGA: 문맥적 성별 주석을 위한 가이드라인 프레임워크

본 논문은 기계 번역(MT)과 대규모 언어 모델(LLM)에서 언어 간 성별 처리 문제를 다루는 체계적인 주석 프레임워크 **ConGA**를 제안한다. 특히 영어(문법적 성별이 거의 없음)에서 이탈리아어(명사, 형용사 등에 성별 일치가 필수)로의 번역 시 발생하는 비대칭 문제에 초점을 맞춘다.

### 핵심 문제
MT 시스템은 성별 정보가 부족할 때 남성형을 기본값으로 사용하는 경향이 있어, **성별 편향**을 강화하고 번역 정확도를 떨어뜨린다. 이는 단순한 기술적 문제가 아니라 사회적 공정성과 직결되는 이슈이다.

### ConGA 프레임워크
ConGA는 번역 맥락에서 성별을 체계적으로 주석하기 위한 가이드라인을 제공한다. 문맥(context)에 기반한 성별 판단을 강조하며, 형태론적으로 풍부한 목표 언어로의 번역 시 성별 정보를 어떻게 결정하고 표현할지에 대한 구조화된 접근법을 제시한다.

### 연구 맥락
이 연구는 LLM의 **평가(evaluation)** 및 **편향(bias)** 문제와 밀접하게 연결된다. 기존 Wiki의 [[Appear2Meaning]] 연구가 다루는 교차문화적 구조화 벤치마크와 유사하게, 언어 간 의미 전달의 비대칭성을 체계적으로 분석한다. 또한 [[Evaluating In-Context Translation with Synchronous Bilingual Texts]]와 번역 품질 평가라는 공통 관심사를 공유하며, [[Syntax is Easy, Semantics is Hard]]의 의미론적 이해 평가와도 맥을 같이 한다. 데이터 주석 품질과 가이드라인 설계라는 측면에서는 벤치마크 구축 연구들과도 연결점이 있다.

## 🔗 관련 논문

- 2026 04 10 appear2meaning a cross cultural benchmark for stru
- 2026 04 10 evaluating in context translation with synchronous
- 2026 04 10 syntax is easy semantics is hard evaluating llms f

## 📐 개념

- [[concepts/machine-translation.md|machine-translation]]
- [[concepts/gender-bias.md|gender-bias]]

---
_LLM 분석으로 재생성됨_
