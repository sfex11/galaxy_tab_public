# What do Language Models Learn and When? The Implicit Curriculum Hypothesis

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-11
**링크**: http://arxiv.org/abs/2604.08510v1

## 💡 핵심 인사이트

LLM 사전학습은 모델 크기와 데이터 혼합에 관계없이 구성적이고 예측 가능한 암묵적 커리큘럼을 따르며, 기술 습득 순서가 일관된 패턴을 보인다.

## 📖 분석

## What do Language Models Learn and When? The Implicit Curriculum Hypothesis

대규모 언어 모델(LLM)이 사전학습 과정에서 어떤 능력을 어떤 순서로 습득하는지를 체계적으로 분석한 연구이다. 기존 스케일링 법칙(scaling laws)이 검증 손실의 양적 개선만을 설명하는 데 반해, 본 논문은 **암묵적 커리큘럼 가설(Implicit Curriculum Hypothesis)**을 제안한다. 이 가설에 따르면 사전학습은 모델과 데이터 혼합에 걸쳐 구성적(compositional)이고 예측 가능한(predictable) 커리큘럼을 따른다.

### 핵심 기여
- 사전학습 중 기술 습득 순서가 모델 크기나 데이터 구성에 관계없이 일관된 패턴을 보임을 실증
- 검증 손실이라는 단일 지표를 넘어, 세분화된(fine-grained) 능력 출현 시점을 추적하는 방법론 제시
- 스케일링 법칙 연구의 확장으로, '얼마나' 개선되는지뿐 아니라 '무엇이 언제' 학습되는지를 설명

### 기존 Wiki와의 연결
- **LLM 엔티티**: LLM 사전학습 역학에 대한 근본적 이해를 제공하는 연구로, LLM의 학습 메커니즘 이해에 직접 기여
- **reasoning-chain / reasoning-integrity 개념**: 추론 능력이 사전학습의 어느 단계에서 출현하는지에 대한 시사점 제공
- **knowledge-distillation / on-policy-distillation**: 커리큘럼 순서 이해는 효율적 지식 증류 전략 설계에 활용 가능
- **multi-token-prediction**: 다중 토큰 예측 능력의 출현 시점 연구와 보완적 관계

이 연구는 LLM의 '블랙박스'적 학습 과정을 해석 가능하게 만드는 중요한 진전으로, 향후 효율적 사전학습 설계와 커리큘럼 학습 전략 최적화에 기여할 수 있다.

## 🔗 관련 논문

- 2026 04 09 toward consistent world models with multi token pr
- 2026 04 10 how much llm does a self revising agent actually n

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/scaling-laws.md|scaling-laws]]
- [[concepts/curriculum-learning.md|curriculum-learning]]
- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/multi-token-prediction.md|multi-token-prediction]]
- [[concepts/knowledge-distillation.md|knowledge-distillation]]

---
_LLM 분석으로 생성됨_
