# Corner Cases: Headland Coverage Path Planning for Autonomous Driving in Arable Farming

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-06
**링크**: http://arxiv.org/abs/2609.04103v1

## 💡 핵심 인사이트

완전한 커버리지는 표준 방법이 배제한 조작(후진 회전)의 수용을 요구한다 — 문자 그대로의 코너가 우아한 해법의 구조적 공백을 폭로하는 실제 코너 케이스다.

## 📖 분석

이 논문은 농경지 헤드랜드(논 가장자리 회전 구역)의 커버리지 경로 계획을 다룬다. 기존 방법들은 중첩 다각형과 부드러운 회전(smooth turn)으로 헤드랜드를 커버했으나, 논 구석을 완전히 덮으려면 후진 조작이 불가피하다. 본 논문은 다각형 구석을 변형해 후진 회전을 허용함으로써 이 간극을 해소하고, gap·overlap·경계 침범의 3축 지표로 타 방법과 비교하여 특히 구석에서 커버리지가 개선됨을 실증한다.

Wiki 관점에서 이 논문의 기여는 제목의 언어유희를 넘는다. 'Corner cases'가 암시하듯, 표준적 우아한 해법이 실패하는 지점이 문자 그대로 기하학적 구석이며, 완전성은 우아함의 포기를 요구한다. 이는 [[concepts/area-coverage.md|area coverage]]가 매핑·탐사 맥락에서 다뤄온 커버리지 개념을 농업 작업의 기하학적 완전성(빈틈 없음, 최소 중복, 경계 준수)으로 확장하고, [[concepts/autonomous-driving.md|autonomous driving]]의 스코프를 온로드 경로 추종에서 오프로드 커버리지 작업으로 넓힌다. 또한 기존 방법의 '부드러운 회전만 허용'이라는 암묵적 전제가 구석 공백의 근원이었다는 진단은, 설계 전제가 최적화 대상의 공백을 규정한다는 [[concepts/evaluator-assumption.md|evaluator assumption]] 패턴의 물리적 사례가 된다.

## 🔗 관련 논문

- A Hough transform approach to safety-aware scalar field mapping using robots
- Toward Robust LiDAR Semantic Segmentation for Real-World Deployment
- Density-Driven Optimal Control: Convergence Guarantees for Stochastic Optimal Control

## 🏷️ 엔티티

- [[entities/headland-coverage-path-planning.md|headland-coverage-path-planning]]
- [[entities/area-coverage.md|area-coverage]]
- [[entities/autonomous-driving.md|autonomous-driving]]
- [[entities/reversing-turn-coverage.md|reversing-turn-coverage]]

## 📐 개념

- [[concepts/smooth-turn-coverage-limitation.md|smooth-turn-coverage-limitation]]
- [[concepts/corner-case-completeness.md|corner-case-completeness]]
- [[concepts/coverage-quality-triple-metric.md|coverage-quality-triple-metric]]
- [[concepts/field-robotics.md|field-robotics]]

---
_LLM 분석으로 생성됨_
