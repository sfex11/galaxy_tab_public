# Feeling the Space: Egomotion-Aware Video Representation for Efficient and Accurate 3D Scene Understanding

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-19
**링크**: http://arxiv.org/abs/2603.17980v1

## 💡 핵심 인사이트

IMU 기반 자기운동 데이터를 MLLM에 통합함으로써 무거운 3D 재구성 없이도 물리적으로 그라운딩된 효율적 3D 공간 추론이 가능하다.

## 📖 분석

## Feeling the Space: Egomotion-Aware Video Representation for Efficient and Accurate 3D Scene Understanding

본 논문은 멀티모달 대형 언어 모델(MLLM)의 3D 공간 추론 능력을 향상시키기 위해 **자기운동(egomotion) 모달리티**를 활용하는 새로운 접근법을 제안한다. 기존 MLLM 기반 3D 장면 이해 방식은 포인트 클라우드나 BEV(Bird's-Eye View) 맵 등 계산 비용이 높은 3D 표현에 의존하거나, 스케일과 크기의 모호성을 해결할 물리적 기반이 부족한 한계가 있었다.

핵심 기여는 **IMU(관성 측정 장치)**로 캡처한 자기운동 데이터를 비디오와 함께 MLLM에 통합하는 것이다. 이를 통해 별도의 3D 재구성 없이도 비디오 프레임 간의 카메라 움직임 정보를 활용하여 물리적으로 그라운딩된 공간 추론이 가능해진다. 이 접근법은 계산 효율성과 정확성을 동시에 달성하며, 기존의 무거운 3D 표현 방식을 대체할 수 있는 경량화된 대안을 제시한다.

이 연구는 [[concepts/reinforcement-learning|강화학습]] 기반 에이전트의 공간 인식 능력과도 연결된다. 특히 로봇 보행([[sources/2026-04-10-robust-quadruped-locomotion-via-ev|Robust Quadruped Locomotion]])이나 내비게이션([[sources/2026-04-10-cadence-context-adaptive-depth-estimation-for-navi|CADENCE]]) 작업에서 자기운동 정보의 활용은 에이전트의 환경 이해를 근본적으로 개선할 수 있다. 또한 MLLM의 멀티모달 통합 관점에서 [[entities/transformer|Transformer]] 아키텍처의 새로운 모달리티 확장 사례로 주목할 만하다.

## 🔗 관련 논문

- 2026 04 10 robust quadruped locomotion via evolutionary reinf
- 2026 04 10 cadence context adaptive depth estimation for navi

## 🏷️ 엔티티

- [[entities/transformer.md|transformer]]

## 📐 개념

- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/3d-scene-understanding.md|3d-scene-understanding]]
- [[concepts/egomotion.md|egomotion]]
- [[concepts/multimodal-learning.md|multimodal-learning]]

---
_LLM 분석으로 재생성됨_
