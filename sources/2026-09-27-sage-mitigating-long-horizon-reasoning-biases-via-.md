# SAGE: Mitigating Long-Horizon Reasoning Biases via Topological Guidance

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-27
**링크**: http://arxiv.org/abs/2609.30192v1

## 💡 핵심 인사이트

장기 추론의 취약성은 계산량 부족이 아니라 추론 공간 구조가 유도하는 탐색·복합 편향의 산물이며, 분기의 위상적 폐쇄성이라는 구조 신호로 탐색을 교정하면 확률적 판정만으로는 포착 불가능한 구조적 불안정성을 사전에 차단할 수 있다.

## 📖 분석

SAGE는 희소 보상 체제에서 장기 추론이 취약해지는 원인을 복합 추론 공간이 유도하는 두 편향으로 규정한다. 첫째 탐색 편향(exploration bias)은 모델이 국소적으로 그럴듯하지만 구조적으로 불안정한 분기로 끌리는 현상이고, 둘째 복합 편향(compounding bias)은 깊이에 걸쳐 국소 편차가 누적되어 희귀 보상을 억제하는 현상이다. 이를 진단하기 위해 Symbolic Closure Analysis(SCA)를 이론적 렌즈로 제안하여 분기의 위상적 폐쇄성을 판별하고, 그 결과를 탐색 가이던스 신호로 추론 과정 내부에 내재화한다.

기존 Wiki 지형에서 이 논문은 두 축을 확정한다. 첫째, 탐색 교정 신호의 계층 구조다 — ExpBoN의 노이즈 주입, Beyond Repeated Sampling의 의미 수준 조향에 이어 SAGE가 위상적 안정성이라는 구조 신호라는 제3 축을 제공하여 노이즈→의미→구조로 정교화되는 계층을 완성한다. 둘째, 위상 활용의 제2 경로다 — SENTINEL-RL이 위상 추론을 외부 그래프 엔진으로 오프로딩해 실행 검증에 사용했다면, SAGE는 위상 분석을 추론 내부의 탐색 교정 도구로 내재화하여 위상의 기능 영역을 확장한다.

또한 국소 고확률 분기의 구조적 불안정성 규정은 확률-품질 결합 전제가 추론 트리 탐색에서도 균열됨을 보이며, 구조 기반 판정은 판정 기준의 확률 외부 이동이라는 횡단 흐름의 추론 공간 사례가 된다.

## 🔗 관련 논문

- Beyond Repeated Sampling: Learning Search Policies for LLM Reasoning
- SENTINEL-RL: Offloading Topological Reasoning from LLM Agents
- ExpBoN: Exponential-Noise Best-of-$n$ for Efficient Test-Time
- StageGuard: Learning Stage Transitions for Long-Horizon Robo

## 🏷️ 엔티티

- [[entities/search-policy-learning.md|search-policy-learning]]
- [[entities/exploration-bias.md|exploration-bias]]
- [[entities/compounding-bias.md|compounding-bias]]
- [[entities/symbolic-closure-analysis.md|symbolic-closure-analysis]]
- [[entities/topological-guidance.md|topological-guidance]]
- [[entities/structural-state-adaptation.md|structural-state-adaptation]]

## 📐 개념

- [[concepts/probability-quality-coupling.md|probability-quality-coupling]]
- [[concepts/extra-probabilistic-adjudication.md|extra-probabilistic-adjudication]]
- [[concepts/reward-sparsity.md|reward-sparsity]]
- [[concepts/test-time-scaling.md|test-time-scaling]]
- [[concepts/semantic-exploration-steering.md|semantic-exploration-steering]]
- [[concepts/soft-best-of-n.md|soft-best-of-n]]
- [[concepts/topological-reasoning-offloading.md|topological-reasoning-offloading]]

---
_LLM 분석으로 생성됨_
