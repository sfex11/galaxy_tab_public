# Comparative Analysis of Agent Evaluation Frameworks: Stability, Detection, and Discovery in Enterprise Analytics Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-12
**링크**: http://arxiv.org/abs/2611.14493v1

## 💡 핵심 인사이트

평가 프레임워크는 상호 대체 불가능한 이질적 측정기기이며, 안정성·탐지·발견이 패러다임별로 분산되므로 단일 프레임워크 선택이 아닌 측정 목적별 조합이 요구된다.

## 📖 분석

기업 분석 에이전트의 실패 탐지를 위해 세 가지 평가 패러다임(트레이스 기반 LLM 판정, 텍스트 전용 LLM 판정+레드팀, 결정론적 휴리스틱)을 동결 실행 트레이스 위에서 3단계로 비교한 연구다. 핵심 기여는 평가 프레임워크를 측정기기로 취급해 그 계측학적 속성을 분리 측정한 점이다: 재현 안정성은 결정론적 휴리스틱이, 알려진 실패 탐지는 LLM 판정이, 신규 실패 발견은 레드팀이 우위를 보이는 안정성·탐지·발견 삼위 구조가 형성된다. 이는 [[judge-instrument-reliability]]의 'LLM judge는 측정기기' 논의에 패러다임 간 상보 삼분법을 제공하고, [[non-cognitive-oracle]](결정론적 오라클은 안정하지만 탐지 범위가 좁다)의 스펙트럼 위치를 실증 데이터로 채운다. 세 프레임워크가 서로 다른 실패 집합을 탐지한다는 발견은 [[oracle-plurality-concept-distinction]] 원리의 평가기기 차원 확장이며, 프레임워크 간 불일치 자체가 에이전트 실패 구조에 대한 정보원이 된다. 동결 트레이스 사용은 [[matched-condition-comparison]] 원리의 평가기기 비교 버전으로, 에이전트 행동 분산을 통제해 순수한 기기 간 차이만을 격리한다. [[cot-monitorability]] 관점에서 트레이스 접근 깊이(전체 트레이스 vs 텍스트 전용)가 탐지 능력을 결정함도 실증된다.

## 🔗 관련 논문

- Ensemble methodology for reference free confidence
- Scenario orchestration for closed loop policy eval

## 🏷️ 엔티티

- [[entities/judge-instrument-reliability.md|judge-instrument-reliability]]
- [[entities/llm-as-judge.md|llm-as-judge]]
- [[entities/non-cognitive-oracle.md|non-cognitive-oracle]]
- [[entities/comparison-oracle.md|comparison-oracle]]
- [[entities/detector-as-instrument.md|detector-as-instrument]]
- [[entities/cot-monitorability.md|cot-monitorability]]
- [[entities/agent-execution-semantic-opacity.md|agent-execution-semantic-opacity]]
- [[entities/matched-condition-comparison.md|matched-condition-comparison]]
- [[entities/oracle-plurality-concept-distinction.md|oracle-plurality-concept-distinction]]
- [[entities/stability-detection-discovery-triad.md|stability-detection-discovery-triad]]

## 📐 개념

- [[concepts/stability-detection-discovery-triad.md|stability-detection-discovery-triad]]
- [[concepts/evaluation-paradigm-triangulation.md|evaluation-paradigm-triangulation]]
- [[concepts/frozen-trace-controlled-evaluation.md|frozen-trace-controlled-evaluation]]

---
_LLM 분석으로 생성됨_
