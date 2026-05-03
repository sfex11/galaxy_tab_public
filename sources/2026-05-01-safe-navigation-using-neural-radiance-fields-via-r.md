# Safe Navigation using Neural Radiance Fields via Reachable Sets

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-01
**링크**: http://arxiv.org/abs/2604.26899v1

## 💡 핵심 인사이트

안전 내비게이션을 동역학 불확실성의 통계적 제어가 아닌, NeRF로 압축된 환경 기하학과 reachable set으로 명시된 로봇 capability 간의 기하학적 포함 관계로 재정의함으로써, 확률적 보장과 기하학적 보장이라는 상보적 안전 패러다임을 제시한다.

## 📖 분석

# Safe Navigation using Neural Radiance Fields via Reachable Sets

**카테고리**: Embodied AI / Safe Navigation
**생성일**: 2026-05-01

## 정의

NeRF(Neural Radiance Field)로 환경의 기하학적 정보를 계산·저장·조작하고, 로봇의 실시간 상태공간 capability를 reachable set으로 표현하여 장애물이 밀집한 환경에서 안전한 내비게이션을 보장하는 프레임워크.

## 기존 Wiki와의 관계

기존 Wiki의 안전 내비게이션 연구축—CBF 기반 제어 장벽 함수([[concepts/safety-critical-control.md|safety critical control]]), GP 기반 안전 임계치 탐사([[concepts/safety-aware-exploration.md|safety aware exploration]]), POMDP 기반 확률적 쉴딩([[concepts/interval-pomdp.md|interval pomdp]])—과 상보적 관계에 있다. 이 논문들은 불확실성을 확률적 경계나 동역학적 제약으로 처리하는 반면, 본 논문은 **환경 표현 자체**를 NeRF로 신경망적으로 압축하고, 로봇의 운동학적 capability를 reachable set으로 명시적으로 기하화하여 안전성을 기하학적 보장으로 변환한다.

## 핵심 기여

기존 안전 내비게이션이 '동역학 불확실성 제어'에 집중했다면, 본 논문은 '환경 기하학의 신경망적 표현 + 로봇 capability의 기하학적 명시'라는 새로운 축을 제시한다. 이는 [[entities/safetyalfred.md|safetyalfred]]가 지적한 체화 안전 평가의 한계—LLM이 물리적 제약을 인코딩하지 않는 문제([[concepts/planning-without-physical-constraint-encoding.md|planning without physical constraint encoding]])—에 대해, 환경 모델 자체에 기하학적 안전 제약을 내재화하는 구조적 해법 경로를 제공한다.

## 다른 논문과의 연결

- [[sources/2026-04-24-a-hough-transform-approach-to-safety-aware-scalar-.md|Hough transform 안전 스칼라 필드 매핑]]과 동일한 문제(안전한 환경 탐사)에 대해 GP 기반이 아닌 NeRF 기반 접근을 제공
- [[sources/2026-04-24-interval-pomdp-shielding-for-imperfect-perception-.md|Interval POMDP 쉴딩]]의 '인지 불확실성' 문제에 대해, 환경 표현의 정밀도를 높여 인지 불확실성 자체를 원천 감소시키는 상보적 경로 제시

## 관련 논문
- [[concepts/neural-combinatorial-optimization.md|neural combinatorial optimization]]
- [[concepts/layered-capability-decomposition.md|layered capability decomposition]]
- [[concepts/methodological-navigation-gap.md|methodological navigation gap]]
- [[concepts/scalar-field-mapping.md|scalar field mapping]]
- [[concepts/neural-operator.md|neural operator]]
- [[concepts/refusal-capability.md|refusal capability]]
- [[entities/methodological-navigation-gap.md|methodological navigation gap]]

- [[sources/2604.26899-safe-navigation-using-neural-radiance-fields-via-reachable-sets.md|Safe Navigation using Neural Radiance Fields via Reachable Sets]]

## 🔗 관련 논문

- 2026 04 24 a hough transform approach to safety aware scalar field mapp
- 2026 04 24 interval pomdp shielding for imperfect perception agents
- 2026 04 23 safetyalfred evaluating safety conscious planning of multim

## 🏷️ 엔티티

- [[entities/neural-radiance-field.md|neural-radiance-field]]
- [[entities/reachable-set.md|reachable-set]]
- [[entities/embodied-ai.md|embodied-ai]]
- [[entities/safety-critical-control.md|safety-critical-control]]
- [[entities/safety-aware-exploration.md|safety-aware-exploration]]

## 📐 개념

- [[concepts/safe-navigation.md|safe-navigation]]
- [[concepts/neural-radiance-field.md|neural-radiance-field]]
- [[concepts/reachable-set.md|reachable-set]]
- [[concepts/geometric-safety-guarantee.md|geometric-safety-guarantee]]
- [[concepts/state-space-capability-representation.md|state-space-capability-representation]]
- [[concepts/cluttered-environment-navigation.md|cluttered-environment-navigation]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-05-01-three-step-nav-a-hierarchical-global-local-planner]]: 두 논문 모두 Embodied AI 환경에서 에이전트가 겪는 내비게이션의 실패 모드를 진단하고, 단일 스케일 처리의 한계를 극복하기 위해 기하학적 구조(Reachable Set, 계층적 기획)를 도입한 안전한 경로 탐색 방법을 제시한다.
