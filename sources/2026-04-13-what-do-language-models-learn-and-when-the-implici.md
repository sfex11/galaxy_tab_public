# What do Language Models Learn and When? The Implicit Curriculum Hypothesis

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-13
**링크**: http://arxiv.org/abs/2604.08510v1

## 💡 핵심 인사이트

LLM 사전학습은 모델과 데이터 믹스에 걸쳐 구성적이고 예측 가능한 암묵적 커리큘럼을 따르며, 스케일링 법칙이 포착하지 못하는 능력 습득의 순서와 패턴을 체계적으로 밝힐 수 있다.

## 📖 분석

## What do Language Models Learn and When? The Implicit Curriculum Hypothesis

본 논문은 LLM 사전학습 과정에서 능력이 출현하는 순서와 패턴을 체계적으로 분석한다. 핵심 제안인 **Implicit Curriculum Hypothesis**는 사전학습이 모델과 데이터 믹스에 걸쳐 구성적(compositional)이고 예측 가능한 커리큘럼을 따른다는 것이다. 기존 스케일링 법칙이 '얼마나' 개선되는지를 설명했다면, 이 연구는 '무엇을' '언제' 학습하는지를 밝힌다.

### 기존 Wiki와의 관계

- **[[implicit-curriculum]]**: 2026-04-11/12에 등록된 동일 논문의 업데이트 버전(v1)으로, implicit curriculum 개념의 핵심 근거 논문이다.
- **[[scaling-laws]]**: 스케일링 법칙이 검증 손실의 양적 개선만 포착하는 한계를 지적하며, 능력별 출현 순서라는 질적 차원을 보완한다.
- **[[curriculum-learning]]**: 명시적 커리큘럼 설계 없이도 데이터 분포 자체가 암묵적 커리큘럼을 형성한다는 점에서, 기존 curriculum learning 연구의 관점을 확장한다.
- **[[emergent-abilities]]**: 능력 출현의 순서가 예측 가능하다는 주장은 emergent abilities의 '갑작스러운 출현' 서사에 대한 대안적 설명을 제공한다.
- **[[multi-token-prediction]]**: 토큰 수준 학습 동역학과 연결되며, 학습 초기/후기에 습득되는 패턴의 차이를 이해하는 데 기여한다.

### 핵심 기여

1. 사전학습의 능력 습득 순서가 모델·데이터에 걸쳐 **재현 가능**함을 실증
2. 검증 손실 이면의 **세분화된 능력 추적** 프레임워크 제안
3. 구성적(compositional) 학습 순서의 존재를 통해 효율적 학습 전략 설계 가능성 시사

## 🔗 관련 논문

- 2026 04 11 what do language models learn and when the implici
- 2026 04 12 what do language models learn and when the implici

## 📐 개념

- [[concepts/implicit-curriculum.md|implicit-curriculum]]
- [[concepts/scaling-laws.md|scaling-laws]]
- [[concepts/curriculum-learning.md|curriculum-learning]]
- [[concepts/emergent-abilities.md|emergent-abilities]]
- [[concepts/multi-token-prediction.md|multi-token-prediction]]

---
_LLM 분석으로 생성됨_
