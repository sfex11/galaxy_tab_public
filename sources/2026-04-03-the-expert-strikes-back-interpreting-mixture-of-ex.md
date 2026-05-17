# The Expert Strikes Back: Interpreting Mixture-of-Experts Language Models at Expert Level

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-03
**링크**: http://arxiv.org/abs/2604.02178v1

## 💡 핵심 인사이트

MoE 전문가 뉴런은 dense FFN 뉴런보다 일관되게 덜 다의적이며, 이는 MoE의 희소 라우팅이 계산 효율성뿐 아니라 내재적 해석가능성에서도 구조적 이점을 제공함을 입증한다.

## 📖 분석

## The Expert Strikes Back: Interpreting Mixture-of-Experts Language Models at Expert Level

본 논문은 Mixture-of-Experts(MoE) 아키텍처의 해석가능성을 dense FFN과 체계적으로 비교한 연구이다. MoE가 주로 계산 효율성을 위해 채택되지만, 그 희소성(sparsity)이 해석가능성 측면에서도 이점을 제공하는지를 $k$-sparse probing을 통해 분석했다.

### 핵심 발견

전문가(expert) 뉴런이 dense FFN 뉴런보다 **일관되게 덜 다의적(less polysemantic)**이라는 결과를 보고한다. 이는 MoE의 라우팅 메커니즘이 자연스럽게 뉴런의 의미적 분리를 유도하며, 각 전문가가 보다 명확한 기능적 역할을 수행함을 시사한다. 이 발견은 MoE 아키텍처가 단순히 효율성뿐 아니라 **내재적 해석가능성(inherent interpretability)** 측면에서도 구조적 이점을 가진다는 새로운 관점을 제시한다.

### Wiki 연결점

이 연구는 [[concepts/mechanistic-interpretability.md|mechanistic interpretability]]와 직접적으로 연결된다. 기존 Wiki의 mechanistic interpretability 연구들이 주로 steering vector와 activation patching을 통한 dense 모델 분석에 집중한 반면, 본 논문은 MoE라는 다른 아키텍처 축에서의 해석가능성을 탐구한다. 또한 [[concepts/mixture-of-experts.md|mixture of experts]] 개념의 이해를 효율성 너머 해석가능성으로 확장하며, Nemotron-Cascade 2 등 기존 MoE 관련 연구와 상호보완적이다. [[concepts/representation-steering.md|representation steering]] 연구에서 다룬 뉴런 수준의 의미 분석과도 방법론적 유사성이 있다.

$k$-sparse probing이라는 분석 도구는 뉴런의 다의성(polysemanticity)을 정량화하는 체계적 방법으로, 향후 다양한 아키텍처 비교 연구의 표준 도구가 될 수 있다.

## 🔗 관련 논문

- 2026 04 11 what drives representation steering a mechanistic 
- 2026 03 27 analysing the safety pitfalls of steering vectors

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/mixture-of-experts.md|mixture-of-experts]]
- [[concepts/mechanistic-interpretability.md|mechanistic-interpretability]]
- [[concepts/representation-steering.md|representation-steering]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[entities/mixture-of-experts.md|mixture of experts]]
