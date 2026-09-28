# Multi-agent Scaling Across Disjunctive and Compensatory Tasks

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-29
**링크**: http://arxiv.org/abs/2609.31563v1

## 💡 핵심 인사이트

다중 에이전트 스케일링의 효용은 팀 크기가 아니라 과제 구조에 조건부이며, 동질 팀의 대규모 극한은 단일 모델 분포의 최빈 답변으로 수렴하여 팀 스케일링의 점근 상한이 개별 모델의 분포 속성으로 결정된다.

## 📖 분석

Steiner의 집단 과제 택소노미(분리형 disjunctive vs 보상형 compensatory)를 다중 에이전트 LLM 스케일링 분석의 프레임으로 도입한다. 핵심 명제는 스케일링 효과가 팀 크기가 아니라 과제 구조의 함수라는 것이다.

분리형 과제에서는 팀 성과가 최고 구성원에 의해 결정되며, 팀 크기 증가는 P(최소 1개 성공)→1의 꼬리 확률 경로로 단조 개선을 제공한다 — 이는 [[test-time-scaling]]의 best-of-n 논리와 동형 구조다. 보상형 과제에서는 독립 표본의 조건부 독립 가정 하에 다수결의 대규모 팀 극한이 모델의 최빈 답변으로 수렴한다.

이 수렴 결과는 [[marginal-distribution-ceiling]]의 다중 에이전트 버전이다: 조건부 정제가 P(y)의 지형을 벗어나지 못하듯, 동질 팀 투표도 단일 모델의 최빈 답변을 넘지 못한다. 이는 상관 오류가 집계 이득을 소진한다는 [[correlated-error-summation]]과 [[co-failure-ceiling]]의 발견을 이론적으로 재정식화한다.

[[capability-cooperation-paradox]]에 과제 구조 조건을 부여한다: 능력이 지배하는 분리형 과제에서는 협력적 구조가 무의미하고, 집계가 지배하는 보상형 과제에서만 독립성·다양성이 전제되므로 [[conditional-heterogeneity-maintenance]]의 비용-편익이 성립한다. 동질 팀의 무한 확장이 최빈값 수렴으로 귀결된다는 점은 [[agent-homogeneity-bias-amplification]]의 점근적 형태이기도 하다.

기존 [[agent-voting]], [[belief-aggregation]] 논의가 투표를 능력 향상 장치로 다뤘다면, 본 논문은 투표의 효용이 과제 택소노미에 조건부임을 밝혀 다중 에이전트 평가에 '과제 구조 명세'라는 전제를 추가한다. [[shannon-game-taxonomy]]가 게임 택소노미로 분석 프레임을 구축했듯, 외부 택소노미의 도입이라는 공통 방법론도 확인된다.

## 🏷️ 엔티티

- [[entities/steiner-task-taxonomy.md|steiner-task-taxonomy]]
- [[entities/disjunctive-compensatory-task-scaling.md|disjunctive-compensatory-task-scaling]]
- [[entities/modal-answer-asymptote.md|modal-answer-asymptote]]
- [[entities/multi-agent-system.md|multi-agent-system]]
- [[entities/agent-voting.md|agent-voting]]
- [[entities/belief-aggregation.md|belief-aggregation]]
- [[entities/capability-cooperation-paradox.md|capability-cooperation-paradox]]
- [[entities/conditional-heterogeneity-maintenance.md|conditional-heterogeneity-maintenance]]
- [[entities/agent-homogeneity-bias-amplification.md|agent-homogeneity-bias-amplification]]
- [[entities/collective-safety-analysis.md|collective-safety-analysis]]
- [[entities/agent-interchangeability.md|agent-interchangeability]]

## 📐 개념

- [[concepts/marginal-distribution-ceiling.md|marginal-distribution-ceiling]]
- [[concepts/correlated-error-summation.md|correlated-error-summation]]
- [[concepts/co-failure-ceiling.md|co-failure-ceiling]]
- [[concepts/test-time-scaling.md|test-time-scaling]]
- [[concepts/plurality-voting-modal-convergence.md|plurality-voting-modal-convergence]]
- [[concepts/conditional-independence-given-item.md|conditional-independence-given-item]]

---
_LLM 분석으로 생성됨_
