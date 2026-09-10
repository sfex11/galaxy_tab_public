# Rethinking Learned Occupancy in Autonomous Active Mapping with Observation-Gated Filtering

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-10
**링크**: http://arxiv.org/abs/2609.09069v1

## 💡 핵심 인사이트

하나의 학습된 표현이 여러 계획 역할로 소비될 때, 관측 지지 게이트 없이는 표현의 비지지 영역이 탐색 결정과 안전 제약을 동시에 왜곡한다.

## 📖 분석

이 논문은 학습 기반 occupancy completion이 활성 3D 매핑에서 만드는 이중 역할 결합 문제를 진단한다. 하나의 예측 맵이 (1) 표면 획득 이득 점수화(어디를 볼 것인가)와 (2) 충돌 없는 이동 제약(어디를 갈 수 있는가)이라는 두 계획 역할을 동시에 수행하며, 직접 관측으로 뒷받침되지 않은(unsupported) occupancy가 탐색 방향과 이동 가능성 믿음을 함께 왜곡한다.

이는 [[capability-safety-inseparability]] 패턴의 표현 계층 사례다. 능력(탐색 정보 획득)과 안전(충돌 회피)이 공유 표현을 거쳐 구조적으로 결합되어, 표현의 오류가 두 축에 동시에 전파된다. [[observation-fidelity-paradox]]의 대칭 축도 제공한다. 공간 맥락 확장이라는 능력 이득이 관측 지지 범위를 벗어나면 왜곡원으로 전환된다는 것이다.

Observation-Gated Filtering은 [[raw-evidence-anchoring]]의 제어적 실현이다. 예측을 직접 관측 지지 여부로 게이트하여 파생 표현의 신뢰를 원 증거에 고정하고, 두 계획 역할 사이의 오류 전파를 절단한다. [[area-coverage]]의 커버리지 계획이 알려진 기하 위의 경로 최적화라면 본 논문은 그 상위의 감지 결정 문제를 다루며, [[safe-navigation]]·[[safety-critical-control]]·[[pomdp]]로 이어지는 활성 감지-안전 이동 문제군에 속한다. 단일 표현의 다중 소비는 관측 지지 게이트 없이는 구조적으로 위험하다는 원칙을 제시한다.

## 🔗 관련 논문

- A Hough transform approach to safety-aware scalar field mapping using Gaussian Processes
- Safe Navigation using Neural Radiance Fields via Reachable Set Analysis
- Corner Cases: Headland Coverage Path Planning for Autonomous Driving in Orchards
- Interval POMDP Shielding for Imperfect-Perception Agents

## 🏷️ 엔티티

- [[entities/capability-safety-inseparability.md|capability-safety-inseparability]]
- [[entities/observation-fidelity-paradox.md|observation-fidelity-paradox]]
- [[entities/raw-evidence-anchoring.md|raw-evidence-anchoring]]
- [[entities/area-coverage.md|area-coverage]]
- [[entities/safe-navigation.md|safe-navigation]]
- [[entities/safety-critical-control.md|safety-critical-control]]
- [[entities/output-epistemic-reliability.md|output-epistemic-reliability]]
- [[entities/observation-gated-filtering.md|observation-gated-filtering]]

## 📐 개념

- [[concepts/dual-role-representation-coupling.md|dual-role-representation-coupling]]
- [[concepts/observation-support-gating.md|observation-support-gating]]
- [[concepts/unsupported-extrapolation-distortion.md|unsupported-extrapolation-distortion]]
- [[concepts/capability-safety-inseparability.md|capability-safety-inseparability]]
- [[concepts/raw-evidence-anchoring.md|raw-evidence-anchoring]]
- [[concepts/observation-fidelity-paradox.md|observation-fidelity-paradox]]

---
_LLM 분석으로 생성됨_
