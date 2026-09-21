# RheoSampling: Resolving the One-Hot Dilemma in Stochastic Dynamic-Tree Speculative Decoding

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-22
**링크**: http://arxiv.org/abs/2609.21827v1

## 💡 핵심 인사이트

동적 트리 추측 디코딩의 결정론적 구축 메커니즘은 확률적 샘플링에서 드래프트 분포를 원핫으로 붕괴시켜, 가속의 유효성이 디코딩 체제(탐욕 vs 확률적)에 정반대로 조건부임을 규명한다.

## 📖 분석

RheoSampling은 동적 트리 추측 디코딩(EAGLE-3 계열)의 '원핫 딜레마'를 규명하고 해결한다. 트리 기반 방법은 탐욕 디코딩에서 결정론적 top-K 확장과 전역 프루닝으로 우수하나, 확률적 디코딩(T>0)에서는 이 메커니즘이 드래프트 분포를 원핫 확률로 붕괴시켜 수용률이 급락한다. 가속 메커니즘의 유효성이 샘플링 체제에 정반대로 조건부인 구조적 딜레마다.

이 발견은 [[distribution-preserving-acceleration]] 논의에 결정적 위반 사례를 제공한다 — 트리 구축이라는 인프라 구조 선택이 분포 자체를 은밀히 변형하며, [[serving-layer-neutrality-premise]]가 예고한 '적응적 추론 최적화의 분포 변형 효과'의 구체적 현현이다. [[decoder-primitive-redefinition]] 관점에서 트리 확장·프루닝은 확률 출력 위의 자원 배분이 아니라 확률 자체를 재구성하는 원시 연산 개입임이 드러난다.

[[speculative-decoding]] 계열에서 [[speckv]]·[[speculation-length-adaptation]]이 파라미터(γ) 적응을 다뤘다면, 본 논문은 메커니즘 자체의 체제 조건부성(탐욕 vs 확률적)을 문제화하여 [[adaptive-inference]]의 조건 축을 확장한다. 원핫 붕괴는 외부에서 관찰되지 않는 조용한 분포 파괴이므로, 가속의 무손실성이 토큰 일치를 넘어 분포 충실도까지 포괄해야 함을 시사한다.

## 🔗 관련 논문

- SpecKV: Adaptive Speculative Decoding with Compression-Aware Gamma Sel
- Unlocking Lossless Speedups in LLMs via Discrete Diffusion
- Position-Aware Drafting for Inference Acceleration in LLM-Based Genera

## 🏷️ 엔티티

- [[entities/speculative-decoding.md|speculative-decoding]]
- [[entities/distribution-preserving-acceleration.md|distribution-preserving-acceleration]]
- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/one-hot-dilemma.md|one-hot-dilemma]]

## 📐 개념

- [[concepts/serving-layer-neutrality-premise.md|serving-layer-neutrality-premise]]
- [[concepts/decoder-primitive-redefinition.md|decoder-primitive-redefinition]]
- [[concepts/token-step-pipeline-hierarchy.md|token-step-pipeline-hierarchy]]
- [[concepts/parallel-token-sampling.md|parallel-token-sampling]]
- [[concepts/sequentiality-distribution-separation.md|sequentiality-distribution-separation]]

---
_LLM 분석으로 생성됨_
