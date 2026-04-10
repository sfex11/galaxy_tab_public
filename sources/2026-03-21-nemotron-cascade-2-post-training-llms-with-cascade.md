# Nemotron-Cascade 2: Post-Training LLMs with Cascade RL and Multi-Domain On-Policy Distillation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-21
**링크**: http://arxiv.org/abs/2603.19220v1

## 💡 핵심 인사이트

Cascade RL과 multi-domain on-policy distillation을 결합하면 3B 활성 파라미터만으로도 IMO/IOI 금메달 수준의 추론 성능을 달성할 수 있어, post-training 전략의 중요성이 모델 규모를 압도할 수 있음을 실증한다.

## 📖 분석

## Nemotron-Cascade 2: Post-Training LLMs with Cascade RL and Multi-Domain On-Policy Distillation

Nemotron-Cascade 2는 NVIDIA가 공개한 30B MoE(Mixture of Experts) 모델로, 활성 파라미터는 3B에 불과하지만 프론티어 오픈 모델에 근접하는 수학·코딩 추론 성능을 달성한다. DeepSeekV3.2-Speciale-671B-A37B에 이어 두 번째로 2025년 국제수학올림피아드(IMO), 국제정보올림피아드(IOI), ICPC에서 금메달 수준 성능을 기록한 오픈 웨이트 LLM이다.

### 핵심 기법

**Cascade Reinforcement Learning**: 단일 단계 RL이 아닌 다단계 캐스케이드 구조의 강화학습을 적용하여 추론 능력을 점진적으로 향상시킨다. 이는 기존 RLHF 기반 post-training과 차별화되는 접근으로, 복잡한 수학·코딩 문제에서 체계적인 추론 체인을 형성하도록 유도한다.

**Multi-Domain On-Policy Distillation**: 수학, 코딩, 에이전트 태스크 등 다양한 도메인에서 on-policy 데이터를 활용한 지식 증류를 수행한다. 이를 통해 소형 MoE 구조에서도 대형 모델의 능력을 효과적으로 전이할 수 있음을 보여준다.

**MoE 효율성**: 30B 전체 파라미터 중 3B만 활성화하는 극단적 희소 활성화 전략은 추론 시 연산 비용을 대폭 절감하면서도 성능 저하를 최소화한다. 이는 실용적 배포 관점에서 중요한 의미를 가진다.

### 의의

이 연구는 post-training 단계에서의 RL 전략 설계가 모델 크기 못지않게 중요함을 실증적으로 보여준다. 특히 에이전트 능력(agentic capabilities)을 갖춘 소형 모델의 가능성을 열어, LLM Agent 연구와 직접적으로 연결된다. Cascade RL 접근은 기존 reinforcement learning 연구의 새로운 응용 방향을 제시하며, on-policy distillation은 transfer learning의 발전된 형태로 볼 수 있다.

## 🔗 관련 논문

- 2026 04 10 android coach improve online agentic training effi
- 2026 04 10 robust quadruped locomotion via evolutionary reinf
- 2026 04 09 in place test time training
- 2026 04 10 how much llm does a self revising agent actually n

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/transfer-learning.md|transfer-learning]]
- [[concepts/post-training.md|post-training]]
- [[concepts/reasoning-chain.md|reasoning-chain]]

---
_LLM 분석으로 재생성됨_
