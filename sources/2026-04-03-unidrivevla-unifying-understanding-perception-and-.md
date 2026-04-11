# UniDriveVLA: Unifying Understanding, Perception, and Action Planning for Autonomous Driving

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-03
**링크**: http://arxiv.org/abs/2604.02190v1

## 💡 핵심 인사이트

VLA 모델에서 공간 인지와 의미 추론의 트레이드오프를 통합 아키텍처로 해결하여, 자율주행 VLA가 2D 언어 지식과 3D 공간 정보를 동시에 활용할 수 있는 경로를 제시한다.

## 📖 분석

## UniDriveVLA: 자율주행을 위한 이해·인지·행동 계획 통합 VLA 모델

UniDriveVLA는 자율주행 분야에서 Vision-Language-Action(VLA) 모델이 직면하는 **공간 인지(spatial perception)와 의미 추론(semantic reasoning) 간의 딜레마**를 해결하기 위한 통합 프레임워크다. 기존 VLA 시스템은 2D Vision-Language Model을 직접 채택하면 공간 인지가 제한되고, 3D 인지를 강화하면 의미 추론 능력이 약화되는 트레이드오프에 빠져 있었다.

UniDriveVLA는 이 문제를 세 가지 능력—장면 이해(understanding), 공간 인지(perception), 행동 계획(action planning)—을 하나의 VLA 아키텍처 안에서 통합함으로써 극복한다. 이는 VLM 기반 자율주행 연구의 핵심 과제였던 **2D 시각-언어 지식과 3D 공간 정보의 효과적 융합**에 대한 새로운 접근을 제시한다.

이 연구는 기존 VLM/VLA 기반 자율주행 연구([[Fail2Drive]], [[AgentVLN]] 등)가 인지와 추론을 분리하여 다루던 한계를 넘어, end-to-end 통합 관점을 제공한다는 점에서 의의가 있다. 또한 [[MARCUS]]와 같은 agentic VLM 연구, [[VectorWorld]]의 world model 접근과도 상호보완적 관계에 있으며, 자율주행에서의 closed-loop 평가([[Fail2Drive]])와 연결하여 실제 주행 성능 검증 관점에서도 중요한 위치를 차지한다.

핵심적으로, VLA 패러다임이 단순한 언어-비전 결합을 넘어 **행동 출력까지 포함하는 통합 모델**로 진화하고 있음을 보여주며, 이는 embodied AI와 자율주행의 교차점에서 중요한 연구 방향이다.

## 🔗 관련 논문

- Fail2Drive: Benchmarking Closed-Loop Driving Generalization
- AgentVLN: Towards Agentic Vision-and-Language Navigation
- MARCUS: An agentic, multimodal vision-language model for car
- VectorWorld: Efficient Streaming World Model via Diffusion F
- Visually-grounded Humanoid Agents
- CADENCE: Context-Adaptive Depth Estimation for Navigation

## 🏷️ 엔티티

- [[entities/vlm.md|vlm]]
- [[entities/mllm.md|mllm]]

## 📐 개념

- [[concepts/autonomous-driving.md|autonomous-driving]]
- [[concepts/vision-language-model.md|vision-language-model]]
- [[concepts/spatial-reasoning.md|spatial-reasoning]]
- [[concepts/embodied-ai.md|embodied-ai]]
- [[concepts/closed-loop-evaluation.md|closed-loop-evaluation]]
- [[concepts/world-model.md|world-model]]
- [[concepts/agentic-vlm.md|agentic-vlm]]
- [[concepts/autonomous-driving-perception.md|autonomous-driving-perception]]

---
_LLM 분석으로 재생성됨_
