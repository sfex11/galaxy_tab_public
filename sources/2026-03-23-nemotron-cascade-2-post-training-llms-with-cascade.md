# Nemotron-Cascade 2: Post-Training LLMs with Cascade RL and Multi-Domain On-Policy Distillation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-23
**링크**: http://arxiv.org/abs/2603.19220v1

## 💡 핵심 인사이트

Cascade RL과 다영역 온폴리시 증류를 결합하면, 활성 파라미터 3B의 소형 MoE 모델로도 수학·코딩·에이전트 태스크에서 프론티어급 대형 모델에 근접하는 추론 성능을 달성할 수 있다.

## 📖 분석

## Nemotron-Cascade 2: Post-Training LLMs with Cascade RL and Multi-Domain On-Policy Distillation

Nemotron-Cascade 2는 NVIDIA가 공개한 30B MoE(Mixture of Experts) 모델로, 활성 파라미터는 3B에 불과하면서도 최첨단 수준의 추론 및 에이전트 능력을 달성한다. 특히 2025년 국제수학올림피아드(IMO), 국제정보올림피아드(IOI), ICPC에서 금메달 수준의 성능을 보인 두 번째 오픈웨이트 LLM이다(첫 번째는 DeepSeekV3.2-Speciale-671B).

### 핵심 기술

**Cascade RL(계단식 강화학습)**: 기존 단일 모델 RL과 달리, 대형 교사 모델과 소형 학생 모델을 계단식으로 연결하여 강화학습을 수행한다. 교사 모델이 어려운 문제에서 탐색한 고품질 추론 경로를 학생 모델이 학습함으로써, 소형 모델의 추론 한계를 효과적으로 극복한다.

**Multi-Domain On-Policy Distillation(다영역 온폴리시 증류)**: 수학, 코딩, 에이전트 등 여러 도메인에서 동시에 온폴리시 방식으로 지식을 증류한다. 이는 단일 도메인 최적화 시 발생하는 성능 저하 문제를 방지하며, 범용적 추론 능력을 유지하게 한다.

### 의의

이 연구는 **MoE 아키텍처와 post-training 기법의 결합**이 소형 모델에서도 프론티어급 성능을 가능케 함을 실증한다. 활성 파라미터 3B로 671B 모델에 근접하는 성능은 효율적 배포 관점에서 큰 함의를 가진다. 또한 Cascade RL 패러다임은 [[concepts/reinforcement-learning.md|reinforcement learning]]의 새로운 확장으로, 교사-학생 프레임워크를 RL 탐색에 적용한 점이 주목할 만하다. 에이전트 능력 강화 측면에서는 [[entities/llm-agent.md|llm agent]] 연구와 직접적으로 연결되며, post-training 최적화 기법으로서 [[concepts/post-training.md|post training]] 개념과도 깊이 관련된다.

## 🔗 관련 논문

- 2026 04 10 android coach improve online agentic training effi
- 2026 04 10 robust quadruped locomotion via evolutionary reinf
- 2026 04 09 in place test time training

## 🏷️ 엔티티

- [[entities/nemotron-cascade-2.md|nemotron-cascade-2]]
- [[entities/nvidia.md|nvidia]]

## 📐 개념

- [[concepts/mixture-of-experts.md|mixture-of-experts]]
- [[concepts/cascade-reinforcement-learning.md|cascade-reinforcement-learning]]
- [[concepts/on-policy-distillation.md|on-policy-distillation]]
- [[concepts/post-training.md|post-training]]
- [[concepts/reinforcement-learning.md|reinforcement-learning]]

---
_LLM 분석으로 재생성됨_
