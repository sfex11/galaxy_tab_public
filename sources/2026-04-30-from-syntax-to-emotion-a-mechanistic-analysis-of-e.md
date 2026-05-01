# From Syntax to Emotion: A Mechanistic Analysis of Emotion Inference in LLMs

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-30
**링크**: http://arxiv.org/abs/2604.25866v1

## 💡 핵심 인사이트

LLM 내부에서 감정 추론은 논리적 추론과 시간적으로 분리된 후기 처리 경로를 가지며, 이는 감정 인식이 논리 파싱의 부산물이 아니라 독립적인 후속 계산 단계임을 기계론적으로 보여준다.

## 📖 분석

# From Syntax to Emotion: A Mechanistic Analysis of Emotion Inference in LLMs

**카테고리**: 기계론적 해석가능성 / 감정 인식
**날짜**: 2026-04-30

## 핵심 발견

SAE(Sparse Autoencoder)를 활용한 기계론적 분석 결과, LLM의 감정 추론은 층간 **3단계 정보 흐름**을 따르며, 감정 관련 특징이 **최종 단계에서만 출현**한다는 사실을 최초로 실증했다.

## 기존 Wiki와의 관계

기존 [[entities/reasoning-integrity|reasoning-integrity]] 연구가 논리적 추론의 무결성에 집중했다면, 본 논문은 비논리적 인지 과정(감정 추론)의 내부 구조를 최초로 기계론적으로 해명하여 추론 무결성 연구의 대상을 논리→감정으로 확장한다. 특히 [[entities/mechanistic-interpretability|mechanistic-interpretability]] 엔티티의 도구(SAE)를 논리가 아닌 감정 도메인에 적용한 선구적 사례다.

[[concepts/shared-logical-subspace|공유된 논리 부분공간]]이 중간 층에서 활성화되는 것과 대비되게, 감정 특징의 후기 출현은 논리와 감정이 LLM 내부에서 **시간적으로 분리된 처리 경로**를 가짐을 시사한다.

## 3단계 정보 흐름 구조

1. **초기 위상**: 구문/어휘적 특징 추출
2. **중간 위상**: 의미론적 특징 구성
3. **최종 위상**: 감정 관련 희소 특징만 집중적으로 출현

이 구조는 [[concepts/implicit-curriculum|암묵적 커리큘럼]]이 감정 인식을 학습의 가장 후순위에 배치한다는 가설과 일치한다.

## 🔗 관련 논문

- 2026-04-23-discovering-a-shared-logical-subspace-steering-llm.md
- 2026-04-11-what-drives-representation-steering-a-mechanistic-.md
- 2026-04-12-what-do-language-models-learn-and-when-the-implici.md

## 🏷️ 엔티티

- [[entities/sparse-autoencoder.md|sparse-autoencoder]]
- [[entities/emotion-inference-mechanism.md|emotion-inference-mechanism]]
- [[entities/late-emerging-feature.md|late-emerging-feature]]
- [[entities/reasoning-integrity.md|reasoning-integrity]]
- [[entities/mechanistic-interpretability.md|mechanistic-interpretability]]
- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/three-phase-information-flow.md|three-phase-information-flow]]
- [[concepts/late-emerging-emotion-feature.md|late-emerging-emotion-feature]]
- [[concepts/emotion-recognition-latency.md|emotion-recognition-latency]]
- [[concepts/syntax-emotion-temporal-separation.md|syntax-emotion-temporal-separation]]
- [[concepts/sparse-autoencoder.md|sparse-autoencoder]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-05-01-morfi-monotonic-sparse-autoencoder-feature-identif]]: 두 논문 모두 희소 오토인코더(SAE)를 활용하여 LLM 내부에서 발생하는 특정 현상(감정 추론 경로, SFT 환발 발생)의 인과적 메커니즘을 기계론적으로 해명한다.
