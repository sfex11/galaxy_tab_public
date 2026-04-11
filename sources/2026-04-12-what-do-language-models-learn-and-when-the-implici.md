# What do Language Models Learn and When? The Implicit Curriculum Hypothesis

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-12
**링크**: http://arxiv.org/abs/2604.08510v1

## 💡 핵심 인사이트

LLM 사전학습은 모델 크기와 데이터 믹스처에 관계없이 구성적이고 예측 가능한 암묵적 커리큘럼(Implicit Curriculum)을 따르며, 스킬 습득 순서에 일관된 패턴이 존재한다.

## 📖 분석

## What do Language Models Learn and When? The Implicit Curriculum Hypothesis

본 논문은 LLM 사전학습 과정에서 능력이 어떤 순서로 습득되는지를 체계적으로 분석한 연구다. 저자들은 **Implicit Curriculum Hypothesis**를 제안하며, 사전학습이 모델과 데이터 믹스처에 걸쳐 구성적(compositional)이고 예측 가능한 커리큘럼을 따른다고 주장한다.

### 핵심 기여
- 기존 스케일링 법칙(scaling laws)이 검증 손실의 총량적 개선만 설명하는 반면, 본 연구는 **어떤 스킬이 어떤 순서로** 습득되는지를 세분화하여 추적
- 모델 크기와 데이터 믹스처가 달라도 스킬 습득 순서에 일관된 패턴이 존재함을 실증
- 사전학습의 암묵적 커리큘럼이 구성적(compositional) 구조를 가짐을 보임

### 기존 Wiki와의 관계
- **[[scaling-laws]]**: 본 논문은 스케일링 법칙을 보완하는 위치에 있으며, 손실 감소의 '무엇'을 밝히는 연구
- **[[curriculum-learning]]**: Implicit Curriculum은 명시적 커리큘럼 학습과 대비되는 개념으로, 자연스럽게 발생하는 학습 순서를 분석
- **[[multi-token-prediction]]**: 토큰 수준의 예측 능력이 어떤 순서로 발전하는지와 직접 관련
- **[[training-data-pruning]]** / **[[knowledge-injection]]**: 데이터 구성이 스킬 습득 순서에 미치는 영향과 연결

### 시사점
사전학습 데이터 믹스처 설계 시 스킬 습득 순서를 고려한 최적화가 가능함을 시사하며, LLM의 emergent abilities 연구에 새로운 분석 프레임워크를 제공한다.

## 🔗 관련 논문

- 2026 04 11 what do language models learn and when the implici
- 2026 04 11 cram less to fit more training data pruning improv
- 2026 04 09 toward consistent world models with multi token pr

## 🏷️ 엔티티

- [[entities/llm.md|LLM]]

## 📐 개념

- [[concepts/scaling-laws.md|scaling-laws]]
- [[concepts/curriculum-learning.md|curriculum-learning]]
- [[concepts/multi-token-prediction.md|multi-token-prediction]]
- [[concepts/training-data-pruning.md|training-data-pruning]]
- [[concepts/knowledge-injection.md|knowledge-injection]]
- [[concepts/implicit-curriculum.md|implicit-curriculum]]
- [[concepts/emergent-abilities.md|emergent-abilities]]

---
_LLM 분석으로 생성됨_
