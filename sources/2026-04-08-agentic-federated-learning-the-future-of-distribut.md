# Agentic Federated Learning: The Future of Distributed Training Orchestration

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-08
**링크**: http://arxiv.org/abs/2604.04895v1

## 💡 핵심 인사이트

LLM 에이전트를 연합학습의 오케스트레이션 제어 평면으로 활용함으로써, 정적 FL 프레임워크의 이질성·비정상성 적응 한계를 동적으로 극복하는 패러다임 전환을 제시한다.

## 📖 분석

## Agentic Federated Learning: The Future of Distributed Training Orchestration

본 논문은 **Agentic-FL**이라는 새로운 패러다임을 제안한다. 기존 연합학습(Federated Learning)의 정적 최적화 방식이 클라이언트의 확률적 이질성(stochastic heterogeneity)과 예측 불가능한 시스템 역학에 적응하지 못하는 한계를 지적하며, **LLM 기반 에이전트(LMagents)**가 자율적으로 분산 학습을 오케스트레이션하는 프레임워크를 소개한다.

### 핵심 아이디어

기존 FL은 클라이언트 선택, 집계 전략, 자원 배분 등을 사전 정의된 규칙으로 처리하지만, Agentic-FL에서는 LLM 에이전트가 실시간으로 시스템 상태를 관찰하고 적응적 의사결정을 수행한다. 이는 [[federated-learning]]의 근본적 한계인 non-IID 데이터 분포와 시스템 이질성 문제를 동적으로 해결하려는 시도이다.

### 기존 연구와의 연결

- **LLM Agent + 최적화**: [[llm-agent]] 엔티티의 활용 범위가 NLP/코드 생성을 넘어 분산 시스템 오케스트레이션으로 확장되는 사례. [[multi-agent-system]]의 조율(coordination) 문제와도 직결된다.
- **연합학습 보안**: 기존 [[federated-learning]] 관련 논문(FL-PBM 등)이 백도어 공격 방어에 집중했다면, 본 논문은 효율성과 적응성 관점에서 접근한다.
- **에이전트 기반 의사결정**: [[ai-decision-making]], [[agent-coordination]] 개념과 밀접하며, 에이전트가 자원 할당과 클라이언트 선택을 자율적으로 수행한다는 점에서 [[task-allocation]]과도 관련된다.
- **비정상 역학 대응**: 시스템 역학의 예측 불가능성에 대응한다는 점에서 [[non-stationary-dynamics]] 개념과 연결된다.

### 의의

LLM 에이전트를 ML 인프라 자체의 제어 평면(control plane)으로 활용하는 접근은, 에이전트 연구가 '도구 사용자'에서 '시스템 운영자'로 진화하는 흐름을 보여준다.

## 🔗 관련 논문

- 2026 03 19 federated distributional reinforcement learning wi
- 2026 03 31 fl pbm pre training backdoor mitigation for federa
- 2026 04 03 collaborative task and path planning for heterogen
- 2026 04 09 who governs the machine a machine identity governa

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/multi-agent-system.md|multi-agent-system]]

## 📐 개념

- [[concepts/federated-learning.md|federated-learning]]
- [[concepts/agent-coordination.md|agent-coordination]]
- [[concepts/task-allocation.md|task-allocation]]
- [[concepts/non-stationary-dynamics.md|non-stationary-dynamics]]
- [[concepts/ai-decision-making.md|ai-decision-making]]

---
_LLM 분석으로 재생성됨_
