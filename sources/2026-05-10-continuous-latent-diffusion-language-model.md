# Continuous Latent Diffusion Language Model

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-10
**링크**: http://arxiv.org/abs/2605.06548v1

## 💡 핵심 인사이트

텍스트 생성의 품질 저하는 비자회귀(순차성 부재) 그 자체가 아니라 의미론적 구조의 손실에 기인하며, 계층적 정보 분해를 통해 확산 기반 비자회귀 생성이 자회귀와 경쟁 가능한 수준의 글로벌 시맨틱을 보존할 수 있다.

## 📖 분석

# Cola DLM: Continuous Latent Diffusion Language Model

**카테고리**: AI/ML — 비자회귀 언어 생성
**생성일**: 2026-05-10

## 정의

Cola DLM은 텍스트 생성을 계층적 정보 분해(hierarchical information decomposition)로 재구성하는 연속 잠재 확산 언어 모델이다. 자회귀(AR) 패러다임의 좌→우 순서 고정을 해체하고, 확산 기반 병렬 생성과 확장 가능한 표현 학습, 글로벌 시맨틱 모델링을 동시에 달성하는 것을 목표로 한다.

## 계층적 분해의 메커니즘

Cola DLM은 텍스트를 먼저 안정적인 잠재 표현으로 학습한 뒤, 이를 계층적으로 분해하여 확산 과정에서 점진적으로 복원한다. 이는 기존 비자회귀 모델들이 품질 저하 없이 병렬 생성을 달성하지 못한 근본 원인—순차적 의존성의 부재가 아닌 의미론적 구조의 상실—을 계층적 정보 구조로 보완하는 접근이다.

## 기존 Wiki와의 관계

[[diffusion-llm]] 엔티티에서 TIDE가 자회귀→확산의 지식 전이를 아키텍처 패러다임 전환의 수단으로 제시했다면, Cola DLM은 확산 언어 모델 자체의 내부 아키텍처를 계층적 분해로 재설계하여 비자회귀 생성의 실질적 성능 한계를 공격한다. [[parallel-decoding]]의 관점에서는, 기존 추측 디코딩이 자회귀 내에서의 병렬화라면 Cola DLM은 패러다임 자체를 비순차적 생성으로 전환하여 병렬화의 상한선을 근본적으로 이동시킨다.

## 연결점

- [[cross-architecture-distillation]]: AR에서 Diffusion으로의 지식 전이가 Cola DLM의 표현 공간을 어떻게 초기화할 수 있는지 시사
- [[hierarchical-kv-memory]]: 계층적 메모리 구조가 AR 서빙과 확산 생성에서 상이한 역할을 함
- [[marginal-distribution-ceiling]]: 확산 모델의 주변 분포 P(y)가 AR과 어떻게 차별화되는지가 핵심 연구 질문

## 🔗 관련 논문

- turning-the-tide-cross-architecture-distillation-f.md
- unifying-sparse-attention-with-hierarchical-memory.md
- speckv-adaptive-speculative-decoding-with-compress.md

## 🏷️ 엔티티

- [[entities/cola-dlm.md|cola-dlm]]
- [[entities/diffusion-llm.md|diffusion-llm]]
- [[entities/parallel-decoding.md|parallel-decoding]]
- [[entities/autoregressive-generation.md|autoregressive-generation]]
- [[entities/hierarchical-representation.md|hierarchical-representation]]

## 📐 개념

- [[concepts/hierarchical-information-decomposition.md|hierarchical-information-decomposition]]
- [[concepts/non-autoregressive-language-modeling.md|non-autoregressive-language-modeling]]
- [[concepts/continuous-latent-diffusion.md|continuous-latent-diffusion]]
- [[concepts/global-semantic-modeling.md|global-semantic-modeling]]

---
_LLM 분석으로 생성됨_
