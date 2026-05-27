# Visual-Redundancy-Controlled Parallel Decoding for Diffusion-Based Multimodal Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-27
**링크**: http://arxiv.org/abs/2605.25820v1

## 💡 핵심 인사이트

기존 신뢰도 기반 병렬 디코딩이 '각 위치의 신뢰도'라는 1차원 최적화에 머무르는 반면, dMLLM의 마스크 병렬 디코딩은 '어떤 위치를 함께 커밋해야 하는가'라는 2차원 최적화를 도입하여 출력의 일관성과 효율을 동시에 달성하는 새로운 차원을 생성한다.

## 📖 분석

# Visual-Redundancy-Controlled Parallel Decoding for Diffusion-Based Multimodal LLMs

Diffusion 기반 멀티모달 대형 언어 모델(dMLLM)의 병렬 마스크 디코딩은 기존 자회귀 기반 병렬 디코딩과 근본적으로 다른 문제를 직면한다. 자회극 접근은 각 마스크 위치의 신뢰도를 독립적으로 순위하고 상위-K개를 커밋하는 반면, 이 논문은 **위치 간 중복성(redundancy)**을 명시적으로 모델링�하여 어떤 위치들을 함께 커밋할지 결정해야 하는 **위치 선택 문제**로 재정의한다. 시각 토큰의 연관성이 높은 위치들을 한데 모두 커밋하는 것은 불필요한 계산을 낭비고, 반대로 독립적 순위만으로는 불충분한 컨텍스트를 생성할 수 있다. 이 논문은 dMLLM의 비자회규적 생성 특성을 고려한 체계적 병렬 디코딩의 새로운 축을 제시한다.

## 기존 Wiki와의 관계

기존 [[entities/parallel-decoding|parallel-decoding]] 엔티티는 주로 자회귀 기반 추측 디코딩에 집중되어 있으며, 확장적 드래프 트리(VRAN), 위치 인식 기반 드래프팅(Position-Aware Drafting) 등은 여전히 타겟 분포 무변경 원칙 하에서 수용률을 최적화하는 연구였다. 그러나 dMLLM에서의 마스크 병렬 디코딩은 타겟 분포에 대한 개별 위치의 신뢰도 순위 외에 **위치 간의 상호 연관성**이라는 새로운 차원을 도입한다. 또한 [[entities/non-autoregressive-language-modeling|non-autoregressive-language-modeling]]의 비순차 생성 특성상, 특히 시각 토큰의 지역적 연관성이라는 dMLLM 특유의 문제를 명확히 식별한다.

## 핵심 인사이트
기존 신뢰도 기반 병렬 디코딩이 '어떤 위치가 가장 신뢰도가 높은가'라는 단일 차원 최적화를 수행하여 entities/output-space-pruning의 한계를 넘는다. 이 논문은 신뢰도의 '위치 간 공동 신뢰도'를 핵심으로 삼아, 단일 순위 상위-K 선택이 가진 시각적 불일치를 유발할 수 있다는 구조적 취약점을 최초로 문제화한다. 이는 [[entities/output-entropy-degradation|output-entropy-degradation]](출력 엔트로피 저하)과도 연결되며, 다양성 확보를 위한 entities/vector-policyoptimization 같은 접근이 비순차 모델 생성에서는 구조적 한계를 다룬다.

## 🏷️ 엔티티

- [[entities/parallel-decoding.md|parallel-decoding]]

## 📐 개념

- [[concepts/inter-position-redundancy.md|inter-position-redundancy]]

---
_LLM 분석으로 생성됨_
