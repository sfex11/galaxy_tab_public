# Unlocking Lossless Speedups in LLMs via Discrete Diffusion

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-07
**링크**: http://arxiv.org/abs/2609.04010v1

## 💡 핵심 인사이트

NTP 분포의 순차성은 모델의 속성이 아니라 샘플링 절차의 속성이므로, 분포를 보존한 채 샘플러만 이산 확산으로 교체하면 무손실 병렬 가속이 달성된다.

## 📖 분석

# Unlocking Lossless Speedups in LLMs via Discrete Diffusion (2026-09-07)

## 핵심 기여
NTP로 훈련한 AR 분포를 그대로 유지한 채, 이산 확산을 병렬 샘플러로 사용해 여러 토큰을 동시에 추출하는 '확산 증강 LLM(diffusion-augmented LLM)'을 제안한다. 파라미터를 AR 가중치(NTP 목적함수)와 보조 확산 파라미터로 분리하여 사전학습 가중치를 재사용하며, 속도 향상이 분포 변경 없이('무손실') 달성됨을 보인다.

## Wiki와의 관계
- [[sequentiality-distribution-separation]]의 실증적 완성: 순차성은 분포의 속성이 아니라 샘플링 절차의 속성임을 매개변수·알고리즘 수준에서 입증한다.
- [[cola-dlm]]과 대척점: Cola DLM이 분포 자체를 비순차적으로 재설계(패러다임 외부)했다면 본 논문은 분포를 보존하고 샘플러만 교체(패러다임 내부)한다. 두 경로는 비순차 생성의 상보적 설계 공간을 형성한다.
- [[speculative-decoding]]의 무손실 병렬화 원칙을 드래프트-수용 구조 없이 확산 조건부 샘플링으로 달성하는 제2 경로다. 단, [[speculative-decoding-losslessness-premise-collapse]]가 지적한 컨텍스트 조건부 무손실성 검증은 남는 과제다.
- [[paradigm-translation-cost]] 회피: 확산을 대체 LM이 아닌 LLM 스택의 '샘플러 프리미티브'로 격하시켜, 패러다임 전환 비용 없이 병렬화를 얻는다.
- [[interface-subordinate-optimization]]의 전형적 사례: 관찰 가능한 인터페이스(AR 분포)를 유지한 채 그 아래에서 최적화가 심화된다.

## 🔗 관련 논문

- Unlocking Lossless Speedups in LLMs via Discrete Diffusion (2026-09-06 선행 등재)
- Continuous Latent Diffusion Language Model
- Turning the TIDE: Cross-Architecture Distillation for Diffusion Large Language Models
- SpecKV: Adaptive Speculative Decoding with Compression-Aware Gamma Selection
- Position-Aware Drafting for Inference Acceleration in LLM-Based Generative Recommendation

## 🏷️ 엔티티

- [[entities/diffusion-augmented-llm.md|diffusion-augmented-llm]]
- [[entities/discrete-diffusion.md|discrete-diffusion]]
- [[entities/parameter-decoupling.md|parameter-decoupling]]
- [[entities/distribution-preserving-acceleration.md|distribution-preserving-acceleration]]
- [[entities/parallel-token-sampling.md|parallel-token-sampling]]
- [[entities/sequentiality-distribution-separation.md|sequentiality-distribution-separation]]
- [[entities/autoregressive-generation.md|autoregressive-generation]]
- [[entities/speculative-decoding.md|speculative-decoding]]
- [[entities/cola-dlm.md|cola-dlm]]
- [[entities/diffusion-llm.md|diffusion-llm]]

## 📐 개념

- [[concepts/sequentiality-distribution-separation.md|sequentiality-distribution-separation]]
- [[concepts/distribution-preserving-acceleration.md|distribution-preserving-acceleration]]
- [[concepts/parallel-token-sampling.md|parallel-token-sampling]]
- [[concepts/parameter-decoupling.md|parameter-decoupling]]
- [[concepts/diffusion-sampler.md|diffusion-sampler]]
- [[concepts/interface-subordinate-optimization.md|interface-subordinate-optimization]]

---
_LLM 분석으로 생성됨_
