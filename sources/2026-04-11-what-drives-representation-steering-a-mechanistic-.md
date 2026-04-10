# What Drives Representation Steering? A Mechanistic Case Study on Steering Refusal

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-11
**링크**: http://arxiv.org/abs/2604.08524v1

## 💡 핵심 인사이트

멀티 토큰 활성화 패칭 프레임워크를 통해 스티어링 벡터가 LLM 내부의 거부 메커니즘에 작용하는 인과적 경로를 최초로 체계적으로 규명하였다.

## 📖 분석

## What Drives Representation Steering? A Mechanistic Case Study on Steering Refusal

스티어링 벡터(steering vectors)를 LLM에 적용하는 것은 효율적인 모델 정렬 기법이지만, 그 내부 메커니즘에 대한 해석 가능한 설명이 부족했다. 본 논문은 거부(refusal) 행동을 사례로 삼아 스티어링 벡터의 인과적 메커니즘을 종합적으로 분석한다.

### 핵심 방법론
저자들은 **멀티 토큰 활성화 패칭(multi-token activation patching)** 프레임워크를 제안하여, 스티어링 벡터가 모델 내부의 어떤 구성 요소에 영향을 미치고 이것이 어떻게 출력 변화로 이어지는지를 추적한다. 기존의 단일 토큰 분석을 넘어 여러 토큰에 걸친 활성화 변화를 체계적으로 패칭함으로써, 스티어링이 작동하는 레이어별·컴포넌트별 인과 경로를 밝혀낸다.

### 주요 발견
- 스티어링 벡터는 모델의 특정 내부 메커니즘(예: 특정 어텐션 헤드, MLP 레이어)에 선택적으로 작용하며, 이 영향이 거부 행동의 활성화/비활성화로 이어진다.
- 서로 다른 스티어링 벡터가 동일한 거부 결과를 만들더라도, 영향을 미치는 내부 경로가 다를 수 있음을 시사한다.

### 기존 Wiki와의 관계
본 연구는 [[reasoning-integrity]]와 밀접하게 관련된다. LLM의 내부 추론 과정을 해석하고 제어하는 메커니즘을 다루기 때문이다. 또한 [[ai-safety]] 개념과 직접 연결되며, 스티어링 벡터를 통한 모델 정렬은 안전한 AI 행동을 보장하기 위한 핵심 기법이다. [[adversarial-prompting]]과도 관련이 있는데, 거부 메커니즘의 이해는 적대적 프롬프트에 대한 방어력 향상에 기여할 수 있다. [[post-training]] 개념과도 연결되며, 스티어링 벡터는 사후 훈련 단계에서의 경량 정렬 방법으로 활용된다.

## 🔗 관련 논문

- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 09 social dynamics as critical vulnerabilities that u

## 🏷️ 엔티티

- [[entities/llm.md|LLM]]

## 📐 개념

- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/reasoning-integrity.md|reasoning-integrity]]
- [[concepts/adversarial-prompting.md|adversarial-prompting]]
- [[concepts/post-training.md|post-training]]
- [[concepts/representation-steering.md|representation-steering]]
- [[concepts/activation-patching.md|activation-patching]]
- [[concepts/mechanistic-interpretability.md|mechanistic-interpretability]]

---
_LLM 분석으로 생성됨_
