# DRIVE-Nav: Directional Reasoning, Inspection, and Verification for Efficient Open-Vocabulary Navigation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-31
**링크**: http://arxiv.org/abs/2603.28691v1

## 💡 핵심 인사이트

프론티어 포인트 대신 지속적 방향(persistent direction)을 탐색 단위로 사용하면, 불완전한 관측 하에서의 경로 불안정성과 반복 방문 문제를 구조적으로 해소할 수 있다.

## 📖 분석

## DRIVE-Nav: Directional Reasoning, Inspection, and Verification for Efficient Open-Vocabulary Navigation

**분류**: Embodied AI / Open-Vocabulary Navigation

DRIVE-Nav는 Open-Vocabulary Object Navigation(OVON) 태스크를 위한 구조화된 탐색 프레임워크다. 기존 제로샷 방법들이 불완전한 관측 하에서 밀집 프론티어 포인트에 대해 추론하면서 불안정한 경로 선택, 반복 방문, 불필요한 행동 오버헤드를 초래하는 문제를 해결한다.

### 핵심 아이디어

DRIVE-Nav의 핵심은 원시 프론티어(raw frontier) 대신 **지속적 방향(persistent direction)**을 중심으로 탐색을 조직화하는 것이다. 에이전트가 마주친 방향을 더 완전하게 검사(inspect)하고, 방향 기반 추론을 통해 효율적인 탐색 전략을 수립한다. 이는 프론티어 기반 탐색의 근본적 한계인 관측 불완전성에서 오는 노이즈를 구조적으로 줄이는 접근이다.

### 기존 연구와의 연결

DRIVE-Nav는 [[embodied-ai]] 분야의 내비게이션 연구 계보에 속하며, 특히 AgentVLN의 에이전틱 VLN 접근과 비교된다. AgentVLN이 VLM 기반의 에이전틱 탐색을 제안했다면, DRIVE-Nav는 방향 기반 구조화를 통해 탐색 효율성을 높이는 데 초점을 둔다. NavTrust가 embodied navigation의 신뢰성 벤치마킹에 집중한 반면, DRIVE-Nav는 실제 탐색 전략의 구조적 개선을 다룬다.

또한 [[vision-language-model]]을 활용한 제로샷 내비게이션 접근으로, VLM의 공간 추론 능력을 방향 기반 프레임워크 안에서 활용한다는 점에서 [[spatial-reasoning]] 연구와도 밀접하다. CADENCE의 깊이 추정 기반 내비게이션과는 상호 보완적 관계에 있다.

## 🔗 관련 논문

- AgentVLN
- CADENCE: Context-Adaptive Depth Estimation for Navigation
- NavTrust: Benchmarking Trustworthiness for Embodied Navigation
- Loc3R-VLM: Language-based Localization and 3D Reasoning with VLMs
- Maestro: Adapting GUIs and Guiding Navigation

## 🏷️ 엔티티

- [[entities/vlm.md|vlm]]

## 📐 개념

- [[concepts/embodied-ai.md|embodied-ai]]
- [[concepts/spatial-reasoning.md|spatial-reasoning]]
- [[concepts/vision-language-model.md|vision-language-model]]

---
_LLM 분석으로 재생성됨_
