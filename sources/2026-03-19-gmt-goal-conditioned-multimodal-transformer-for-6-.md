# GMT: Goal-Conditioned Multimodal Transformer for 6-DOF Object Trajectory Synthesis in 3D Scenes

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-19
**링크**: http://arxiv.org/abs/2603.17993v1

## 💡 핵심 인사이트

Transformer 아키텍처를 3D 장면의 6-DOF 물체 조작 궤적 합성에 적용하여, 멀티모달 장면 이해와 목표 조건부 제어를 통해 물리적으로 타당한 로봇 궤적 생성을 가능하게 한 프레임워크이다.

## 📖 분석

## GMT: Goal-Conditioned Multimodal Transformer for 6-DOF Object Trajectory Synthesis in 3D Scenes

**arXiv**: http://arxiv.org/abs/2603.17993v1
**날짜**: 2026-03-19

### 개요

GMT는 3D 환경에서 6-DOF(6 자유도) 물체 조작 궤적을 합성하기 위한 멀티모달 트랜스포머 프레임워크이다. 기존 접근법들이 2D 또는 부분적 3D 표현에 의존하여 전체 장면 기하학을 포착하지 못하고 궤적 정밀도에 제약이 있었던 한계를 극복하고자 한다.

### 핵심 기여

- **멀티모달 장면 이해**: 3D 포인트 클라우드, 시각 정보, 언어 지시 등 다양한 모달리티를 통합하여 장면을 이해하고, 이를 기반으로 물리적으로 타당한 6-DOF 궤적을 생성한다.
- **목표 조건부 생성**: 목표 상태(goal condition)를 명시적으로 입력받아, 원하는 최종 상태로의 궤적을 제어 가능하게 합성한다.
- **Transformer 아키텍처 활용**: 시퀀스 모델링에 강점을 가진 Transformer를 궤적 합성에 적용하여, 시간적 일관성과 공간적 정밀도를 동시에 확보한다.

### 기존 Wiki와의 연결

**Transformer** 엔티티와 직접적으로 관련된다. GMT는 Transformer 아키텍처를 로봇 조작 궤적 합성이라는 새로운 도메인에 적용한 사례로, Transformer의 적용 범위가 NLP·비전을 넘어 로보틱스의 공간 추론 영역으로 확장되고 있음을 보여준다. 또한 멀티모달 입력을 처리한다는 점에서 최근 멀티모달 연구 흐름과도 맥을 같이 한다.

3D 환경에서의 물체 궤적 합성은 로봇이 복잡한 장면과 상호작용하기 위한 핵심 역량이며, 향후 LLM 기반 에이전트가 물리 세계에서 행동을 계획할 때 이러한 궤적 합성 모듈과의 통합이 중요해질 것이다.

## 🏷️ 엔티티

- [[entities/transformer.md|transformer]]

## 📐 개념

- [[concepts/reinforcement-learning.md|reinforcement-learning]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[concepts/transformer.md|transformer]]

---
**관련**: [[concepts/expressiveness-conditioned-absorption.md|expressiveness conditioned absorption]]
