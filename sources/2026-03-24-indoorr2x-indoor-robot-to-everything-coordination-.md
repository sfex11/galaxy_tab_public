# IndoorR2X: Indoor Robot-to-Everything Coordination with LLM-Driven Planning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-24
**링크**: http://arxiv.org/abs/2603.20182v1

## 💡 핵심 인사이트

실내 로봇 협업에서 R2R을 넘어 IoT 인프라 전체와의 R2X 통신 패러다임을 제시하고, LLM 기반 계획으로 이기종 센서 데이터를 통합 조율하는 최초의 벤치마크 프레임워크이다.

## 📖 분석

## IndoorR2X: Indoor Robot-to-Everything Coordination with LLM-Driven Planning

**IndoorR2X**는 실내 환경에서 로봇 간(R2R) 통신을 넘어, IoT 센서(카메라 등)를 포함한 건물 전체 인프라와의 협업을 통해 부분 관측성(partial observability) 문제를 해결하는 최초의 벤치마크 및 시뮬레이션 프레임워크이다.

### 핵심 아이디어
기존 로봇 간 통신(R2R)만으로는 실내 장면 이해에서 부분 관측성을 극복하기 위해 과도한 탐색 비용이나 팀 규모 확대가 필요하다. IndoorR2X는 이미 많은 실내 환경에 설치된 저비용 IoT 센서들이 제공하는 지속적이고 건물 전체에 걸친 컨텍스트를 활용하여 이 한계를 돌파한다. 여기서 'R2X'는 Vehicle-to-Everything(V2X) 통신 패러다임에서 영감을 받은 개념으로, 로봇이 다른 로봇뿐 아니라 인프라 전체와 정보를 교환하는 구조를 의미한다.

### LLM 기반 계획
LLM을 활용한 계획(planning) 모듈이 핵심 구성요소로, 이기종 센서 데이터를 통합하고 로봇의 행동을 조율한다. 이는 [[entities/llm-agent.md|llm agent]] 연구에서 LLM이 도구 사용과 환경 상호작용을 조율하는 패러다임의 자연스러운 확장이며, [[concepts/embodied-ai.md|embodied ai]]와 [[concepts/spatial-reasoning.md|spatial reasoning]] 분야를 IoT 인프라 수준으로 확장한 사례이다.

### 기존 연구와의 연결
- **AgentVLN** 등 비전-언어 내비게이션 연구와 달리, 단일 로봇의 인식 한계를 IoT 인프라 융합으로 보완하는 시스템 수준 접근을 취한다.
- **DRIVE-Nav** 등 자율주행 내비게이션 연구의 실내 버전으로 볼 수 있으며, V2X에서 R2X로의 패러다임 전환을 제시한다.
- [[concepts/multi-agent-system.md|multi agent system]] 관점에서 로봇-센서 간 이기종 협업이라는 새로운 차원을 추가한다.

## 🔗 관련 논문

- 2026 04 09 maestro adapting guis and guiding navigation with
- 2026 04 10 cadence context adaptive depth estimation for navi
- 2026 04 09 social dynamics as critical vulnerabilities that u

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/embodied-ai.md|embodied-ai]]
- [[concepts/spatial-reasoning.md|spatial-reasoning]]
- [[concepts/multi-agent-system.md|multi-agent-system]]

---
_LLM 분석으로 재생성됨_
