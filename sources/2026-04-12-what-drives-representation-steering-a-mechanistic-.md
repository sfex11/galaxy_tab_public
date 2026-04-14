# What Drives Representation Steering? A Mechanistic Case Study on Steering Refusal

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-12
**링크**: http://arxiv.org/abs/2604.08524v1

## 💡 핵심 인사이트

멀티토큰 활성화 패칭 프레임워크를 통해 스티어링 벡터가 LLM 내부에서 거부 행동을 유발하는 인과적 메커니즘 경로를 최초로 체계적으로 규명하였다.

## 📖 분석

## What Drives Representation Steering? A Mechanistic Case Study on Steering Refusal

본 논문은 대형 언어 모델(LLM)에 스티어링 벡터(steering vector)를 적용하는 정렬 기법의 내부 인과 메커니즘을 체계적으로 분석한 연구다. 특히 거부(refusal) 행동을 사례로 삼아, 스티어링 벡터가 모델 내부의 어떤 메커니즘에 영향을 미치고 이것이 어떻게 다른 출력으로 이어지는지를 규명한다.

### 핵심 방법론
저자들은 **멀티토큰 활성화 패칭(multi-token activation patching)** 프레임워크를 제안하여, 단일 토큰이 아닌 여러 토큰에 걸친 인과적 효과를 추적한다. 이를 통해 스티어링 벡터가 영향을 미치는 내부 컴포넌트와 경로를 식별하였다.

### 기존 연구와의 관계
- **representation-steering**: 본 논문은 이 개념의 핵심 메커니즘 연구로, 스티어링 벡터의 작동 원리에 대한 인과적 설명을 최초로 제시한다.
- **mechanistic-interpretability**: 활성화 패칭 기반 해석 방법론을 스티어링 벡터 분석에 확장 적용한 사례다.
- **activation-patching**: 기존 단일 토큰 패칭을 멀티토큰으로 확장한 새로운 프레임워크를 제안한다.
- **llm-alignment**: 스티어링 벡터가 정렬 기법으로서 왜 효과적인지에 대한 해석 가능한 근거를 제공한다.

### 연결점
[[2026-04-11-what-drives-representation-steering-a-mechanistic-]] 이전 버전과 동일 논문의 업데이트로 보이며, [[2026-03-27-analysing-the-safety-pitfalls-of-steering-vectors]] 논문이 스티어링 벡터의 안전성 함정을 분석한 것과 상호보완적이다. 본 논문은 '왜 작동하는가'를, 후자는 '어디서 실패하는가'를 다룬다.

## 🔗 관련 논문

- 2026 04 11 what drives representation steering a mechanistic case stud
- 2026 03 27 analysing the safety pitfalls of steering vectors
- 2026 04 02 aligned orthogonal or in conflict when can we safe

## 📐 개념

- [[concepts/representation-steering.md|representation-steering]]
- [[concepts/mechanistic-interpretability.md|mechanistic-interpretability]]
- [[concepts/activation-patching.md|activation-patching]]
- [[concepts/llm-alignment.md|llm-alignment]]
- [[concepts/multi-token-activation-patching.md|multi-token-activation-patching]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-04-13-what-drives-representation-steering-a-mechanistic-]]: 동일 논문의 다른 날짜 요약으로, 스티어링 벡터의 내부 인과 메커니즘을 다룬다.
- → [[sources/2026-04-14-large-language-models-generate-harmful-content-usi]]: 둘 다 LLM 내부의 안전성/정렬 메커니즘을 기계적으로 분석하며, 전자는 거부 스티어링의 인과 경로를, 후자는 유해 콘텐츠 생성의 통합 메커니즘을 규명한다.
