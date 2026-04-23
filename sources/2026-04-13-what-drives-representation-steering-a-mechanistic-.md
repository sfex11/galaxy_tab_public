# What Drives Representation Steering? A Mechanistic Case Study on Steering Refusal

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-13
**링크**: http://arxiv.org/abs/2604.08524v1

## 💡 핵심 인사이트

Steering vector의 효과는 단일 메커니즘이 아닌 다수의 내부 구성 요소에 분산되어 있으며, multi-token activation patching을 통해 토큰 위치별로 서로 다른 인과 경로가 refusal 행동을 매개함을 밝혔다.

## 📖 분석

## What Drives Representation Steering? A Mechanistic Case Study on Steering Refusal

본 논문은 **steering vector**(조향 벡터)가 LLM 내부에서 어떤 인과적 메커니즘을 통해 모델 출력을 변화시키는지를 거부(refusal) 사례를 중심으로 체계적으로 분석한 연구이다.

### 핵심 기여

기존 representation steering 연구가 '효과가 있다'는 것은 보였지만, **왜 작동하는지**에 대한 해석 가능한 설명이 부족했다. 본 연구는 **multi-token activation patching** 프레임워크를 제안하여, steering vector가 영향을 미치는 내부 구성 요소(attention head, MLP 등)와 그 결과로 출력이 달라지는 경로를 인과적으로 추적한다.

### 기존 Wiki와의 관계

- **[[concepts/representation-steering.md|representation steering]]**: 본 논문의 직접적 연구 대상. 기존 개념 문서에 이미 2026-04-11 동일 논문의 이전 버전이 등록되어 있으며, 이번 v1 분석이 메커니즘 수준의 설명을 추가한다.
- **[[concepts/mechanistic-interpretability.md|mechanistic interpretability]]**: activation patching을 활용한 인과적 분석 방법론으로, 기존 개념과 직결된다.
- **[[concepts/activation-patching.md|activation patching]]**: 본 논문이 기존 단일 토큰 patching을 **multi-token**으로 확장한 점이 방법론적 기여이다.
- **[[concepts/llm-alignment.md|llm alignment]]**: steering vector는 모델 정렬 기법의 일종으로, 안전성(refusal) 조정과 직접 연결된다.
- **[[concepts/ai-safety.md|ai safety]]**: refusal 메커니즘의 이해는 guardrail 설계에 핵심적 시사점을 제공한다.

### 새로운 인사이트

steering vector의 효과가 단일 경로가 아닌 **다수의 내부 메커니즘에 분산**되어 있으며, 토큰 위치에 따라 서로 다른 구성 요소가 활성화된다는 발견은 향후 정밀한 모델 제어 연구의 기반이 된다.

## 🔗 관련 논문

- 2026 04 11 what drives representation steering a mechanistic
- 2026 04 12 what drives representation steering a mechanistic

## 🏷️ 엔티티

- [[entities/llm.md|LLM]]

## 📐 개념

- [[concepts/representation-steering.md|representation-steering]]
- [[concepts/mechanistic-interpretability.md|mechanistic-interpretability]]
- [[concepts/activation-patching.md|activation-patching]]
- [[concepts/multi-token-activation-patching.md|multi-token-activation-patching]]
- [[concepts/llm-alignment.md|llm-alignment]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/reasoning-integrity.md|reasoning-integrity]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-04-12-what-drives-representation-steering-a-mechanistic-]]: 동일 논문의 다른 날짜 요약으로, 스티어링 벡터의 내부 인과 메커니즘을 다룬다.
