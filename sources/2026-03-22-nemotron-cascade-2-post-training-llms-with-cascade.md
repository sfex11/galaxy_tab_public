# Nemotron-Cascade 2: Post-Training LLMs with Cascade RL and Multi-Domain On-Policy Distillation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-22
**링크**: http://arxiv.org/abs/2603.19220v1

## 💡 핵심 인사이트

30B MoE 모델에서 3B 활성 파라미터만으로 올림피아드 금메달급 추론을 달성한 것은, cascade 강화학습과 multi-domain on-policy distillation이 모델 규모의 한계를 극복하는 효과적인 post-training 전략임을 실증한다.

## 📖 분석

## Nemotron-Cascade 2: Post-Training LLMs with Cascade RL and Multi-Domain On-Policy Distillation

Nemotron-Cascade 2는 NVIDIA가 공개한 30B MoE(Mixture-of-Experts) 모델로, 활성 파라미터는 3B에 불과하지만 프론티어급 수학·코딩 추론 성능을 달성한다. 2025 IMO 금메달 수준, IOI, ICP 등 국제 올림피아드에서 경쟁력 있는 성과를 보인 두 번째 오픈웨이트 LLM이다(첫 번째는 DeepSeekV3.2-Speciale-671B).

### 핵심 기술

**Cascade RL(캐스케이드 강화학습)**: 단일 모델이 아닌 다단계 캐스케이드 구조에서 강화학습을 적용하여, 작은 활성 파라미터로도 복잡한 추론 체인을 효과적으로 학습한다. 이는 기존 단일 모델 RL 대비 효율성과 성능 양면에서 이점을 제공한다.

**Multi-Domain On-Policy Distillation**: 수학, 코딩, 에이전틱 태스크 등 다양한 도메인에서 on-policy 데이터를 활용한 지식 증류를 수행한다. 이를 통해 도메인 간 간섭을 최소화하면서 멀티도메인 역량을 동시에 확보한다.

**MoE 아키텍처의 효율성**: 30B 총 파라미터 중 3B만 활성화하는 구조로, 추론 시 계산 비용을 대폭 절감하면서도 dense 모델에 준하는 성능을 유지한다. 이는 에이전틱 배포 시나리오에서 특히 실용적이다.

### 의의

소규모 활성 파라미터 모델이 올림피아드급 추론에 도달할 수 있음을 실증하여, '규모의 법칙'에 대한 재고를 촉진한다. Cascade RL은 post-training 단계에서의 새로운 패러다임으로, 기존 SFT+RLHF 파이프라인을 넘어서는 접근법이다.

## 🔗 관련 논문

- 2026 04 10 how much llm does a self revising agent actually n
- 2026 04 09 in place test time training
- 2026 04 10 android coach improve online agentic training effi
- 2026 04 08 triattention efficient long reasoning with trigono

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/multi-agent-system.md|multi-agent-system]]
- [[concepts/speculative-decoding.md|speculative-decoding]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[entities/nemotron-cascade-2.md|nemotron cascade 2]]

---
**관련**: [[concepts/end-to-end-vla-training.md|end to end vla training]]

---
**관련**: [[concepts/goal-conditioned-policy.md|goal conditioned policy]]

---
**관련**: [[concepts/test-time-training.md|test time training]]

---
**관련**: [[entities/training-data-pruning.md|training data pruning]]

---
**관련**: [[entities/self-referential-training-vulnerability.md|self referential training vulnerability]]

---
**관련**: [[concepts/training-loop-safety-incident.md|training loop safety incident]]

---
**관련**: [[concepts/persistent-workspace-training.md|persistent workspace training]]

---
**관련**: [[concepts/verifiable-training-data-synthesis.md|verifiable training data synthesis]]

---
**관련**: [[concepts/training-phase-knowledge-contamination.md|training phase knowledge contamination]]

---
**관련**: [[concepts/stabilized-knowledge-distillation.md|stabilized knowledge distillation]]
