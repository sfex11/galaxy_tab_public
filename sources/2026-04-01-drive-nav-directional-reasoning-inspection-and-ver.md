# DRIVE-Nav: Directional Reasoning, Inspection, and Verification for Efficient Open-Vocabulary Navigation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-01
**링크**: http://arxiv.org/abs/2603.28691v1

## 💡 핵심 인사이트

밀집 프론티어 포인트 대신 지속적 방향(persistent directions)을 탐색 단위로 사용함으로써, 불완전 관측 환경에서의 경로 안정성과 탐색 효율성을 동시에 개선하는 구조화된 OVON 프레임워크를 제시했다.

## 📖 분석

## DRIVE-Nav: Directional Reasoning, Inspection, and Verification for Efficient Open-Vocabulary Navigation

**분류**: Embodied AI / Open-Vocabulary Navigation

DRIVE-Nav는 Open-Vocabulary Object Navigation(OVON) 문제를 해결하기 위한 구조화된 프레임워크로, 기존 제로샷 방법들이 불완전한 관측 하에서 밀집 프론티어 포인트에 대해 추론하면서 발생하는 불안정한 경로 선택, 반복 방문, 불필요한 행동 오버헤드 문제를 해결한다.

### 핵심 접근법

DRIVE-Nav의 핵심 혁신은 원시 프론티어(raw frontiers) 대신 **지속적 방향(persistent directions)**을 중심으로 탐색을 조직화하는 것이다. 이 프레임워크는 세 가지 단계로 구성된다:
- **Directional Reasoning**: 환경을 방향 단위로 구조화하여 탐색 공간을 줄임
- **Inspection**: 만난 방향들을 더 완전하게 검사하여 정보 기반 결정 수행
- **Verification**: 탐색 결과를 검증하여 불필요한 재방문 방지

### 기존 연구와의 연결

DRIVE-Nav는 [[AgentVLN]]의 에이전틱 비전-언어 내비게이션과 유사한 embodied navigation 문제를 다루지만, 사전 정의된 언어 명령이 아닌 개방형 어휘 목표를 처리한다는 점에서 차별화된다. [[CADENCE]]의 맥락 적응형 깊이 추정과 보완적 관계에 있으며, 내비게이션 에이전트의 공간 인식 능력 향상이라는 공통 목표를 공유한다.

VLM 기반 제로샷 접근법을 사용한다는 점에서 [[vision-language-model]] 연구 흐름에 속하며, 구조화된 탐색 전략은 [[graph-based-planning]] 개념과도 연결된다. 특히 불완전 관측 하 효율적 탐색이라는 문제 설정은 [[embodied-ai]] 분야의 핵심 도전 과제를 정면으로 다룬다.

## 🔗 관련 논문

- AgentVLN: Towards Agentic Vision-and-Language Navigation
- CADENCE: Context-Adaptive Depth Estimation for Navigation
- Loc3R-VLM: Language-based Localization and 3D Reasoning with
- NavTrust: Benchmarking Trustworthiness for Embodied Navigation

## 📐 개념

- [[concepts/embodied-ai.md|embodied-ai]]
- [[concepts/vision-language-model.md|vision-language-model]]
- [[concepts/graph-based-planning.md|graph-based-planning]]
- [[concepts/spatial-reasoning.md|spatial-reasoning]]

---
_LLM 분석으로 재생성됨_
