# Three-Step Nav: A Hierarchical Global-Local Planner for Zero-Shot Vision-and-Language Navigation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-01
**링크**: http://arxiv.org/abs/2604.26946v1

## 💡 핵심 인사이트

MLLM 기반 제로샷 VLN 에이전트의 실패는 추론 능력 부족이 아니라 단일 스케일 기획의 구조적 한계에서 기인하며, 전역-국소 계층 분해가 이를 아키텍처 수준에서 해결한다.

## 📖 분석

# Three-Step Nav: 계층적 전역-국소 기획을 통한 제로샷 VLN

**카테고리**: Embodied AI / Vision-Language Navigation
**생성일**: 2026-05-01

## 정의
MLLM 기반 제로샷 VLN 에이전트가 미지 환경에서 겪는 세 가지 구조적 실패 모드 — 경로 이탈(course drift), 조기 정지(premature halting), 낮은 성공률 — 를 계층적 전역-국소(3단계) 기획 아키텍처로 해결하는 접근법.

## 기존 Wiki와의 관계

### AgentVLN과의 연결
기존 Wiki에 등록된 AgentVLN(2026-03-20)이 VLN의 에이전틱 전환을 제시했다면, Three-Step Nav은 그 에이전트가 실제 미지 환경에서 왜 실패하는지를 세 가지 실패 모드로 구체화하고, 이에 대한 아키텍처 수준 해법을 제공한다. 특히 기획을 단일 스케일에서 전역-국소 계층으로 분해하는 것은 [[entities/hierarchical-planning|hierarchical-planning]] 엔티티에 VLN 도메인 특화 사례를 추가한다.

### 공간 추론 연구 축과의 관계
VLM 합성 분석(26편)에서 가장 두꺼운 연구 축으로 식별된 '공간 추론 능력의 확장'에 속하며, Loc3R-VLM이 3D 위치 추정을, 3DCity-LLM이 도시 규모를 다룬 것과 대비되어 실내 내비게이션의 경로 수준 기획을 다룬다.

### 체화 AI 안전성과의 간접적 관계
SafetyALFRED가 체화 환경에서의 안전 기획 부재를 문제 삼았다면, Three-Step Nav의 '경로 이탈' 문제는 안전성의 전제조건(목표 도달 능력) 부재를 나타낸다. 기획 신뢰성 확보가 안전성 확보의 상위 조건임을 시사한다.

## 관련 논문
- [[sources/2026-05-01-three-step-nav-a-hierarchical-global-local-planner-.md|Three-Step Nav: A Hierarchical Global-Local Planner for Zero-Shot Vision-and-Language Navigation]]

## 🔗 관련 논문

- 2026-03-20-agentvln-towards-agentic-vision-and-language-navig
- 2026-04-23-safetyalfred-evaluating-safety-conscious-planning-.md
- 2026-03-19-loc3r-vlm-language-based-localization-and-3d-reaso

## 🏷️ 엔티티

- [[entities/three-step-nav.md|three-step-nav]]
- [[entities/agentic-vlm.md|agentic-vlm]]
- [[entities/hierarchical-planning.md|hierarchical-planning]]
- [[entities/spatial-reasoning.md|spatial-reasoning]]
- [[entities/embodied-ai.md|embodied-ai]]

## 📐 개념

- [[concepts/three-step-nav.md|three-step-nav]]
- [[concepts/course-drift.md|course-drift]]
- [[concepts/premature-halting.md|premature-halting]]
- [[concepts/global-local-planning-hierarchy.md|global-local-planning-hierarchy]]
- [[concepts/zero-shot-vln.md|zero-shot-vln]]

---
_LLM 분석으로 생성됨_
