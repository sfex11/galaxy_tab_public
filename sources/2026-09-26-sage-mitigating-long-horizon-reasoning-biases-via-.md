# SAGE: Mitigating Long-Horizon Reasoning Biases via Topological Guidance

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-26
**링크**: http://arxiv.org/abs/2609.30192v1

## 💡 핵심 인사이트

장기 추론의 취약성은 모델 능력 부족이 아니라 추론 공간의 위상 구조가 유도하는 탐색·누적 편향이며, 기호적 위상 분석(SCA)으로 이를 형식화하면 희소 보상 체제에서도 구조적으로 교정 가능하다.

## 📖 분석

SAGE는 희소 보상 체제 하 장기 추론의 취약성을 추론 공간의 위상 구조가 유도하는 두 편향으로 진단한다. (1) 탐색 편향(exploration bias): 국소적으로 그럴듯하지만 구조적으로 불안정한 분기로 모델이 끌리는 현상. (2) 누적 편향(compounding bias): 작은 국소 편차가 깊이에 걸쳐 누적되어 희귀 보상의 도달 가능성을 억압하는 현상. 이를 완화하기 위해 Symbolic Closure Analysis(SCA)로 추론 공간의 위상을 기호적으로 형식화하고, 위상 가이던스로 탐색을 교정한다.

Wiki 지형에서의 위치: ① [[compounding-error]]에 추론 공간 버전을 제공한다 — OPTED·Talk2Escape의 물리 궤적 누적 오류와 대비하여, 누적이 궤적과 추론 깊이 양쪽에서 동형으로 발생하는 도메인 불변 구조임을 확정한다. ② 테스트타임 탐색 개입의 제3 축 — ExpBoN의 노이즈 주입, [[search-policy-learning]] 계열(Beyond Repeated Sampling)의 의미 조향에 이어 분기의 위상적 안정성이라는 구조 신호를 추가한다. ③ [[probability-quality-coupling]]의 실증 — 높은 확률 분기가 구조적으로 불안정할 수 있음을 보여 확률-품질 결합 전제의 균열을 추론 트리 탐색으로 확장한다. ④ [[topological-reasoning-offloading]]과 대비 — SENTINEL-RL이 위상 추론을 외부 그래프 엔진으로 오프로딩했다면, SAGE는 위상 분석을 탐색 교정의 내재 가이던스 신호로 전환한다. ⑤ [[false-positive-convergence]]의 추론 공간 발현 사례를 제공한다.

핵심 시사: 장기 추론 실패의 근원은 모델 능력이 아니라 공간 위상이며, 구조적 진단이 희소 보상 체제의 제약을 우회하는 경로가 된다.

## 🔗 관련 논문

- Beyond Repeated Sampling: Learning Search Policies for LLM R
- ExpBoN: Exponential-Noise Best-of-$n$ for Efficient Test-Tim
- SENTINEL-RL: Offloading Topological Reasoning from LLM Agent
- OPTED: On-Policy Fine-Tuning for End-to-End Driving using a 
- Talk2Escape: Conversational Grounding for Vision-and-Languag
- Bellman Policy Optimization

## 🏷️ 엔티티

- [[entities/compounding-error.md|compounding-error]]
- [[entities/reward-sparsity.md|reward-sparsity]]
- [[entities/search-policy-learning.md|search-policy-learning]]
- [[entities/structural-state-adaptation.md|structural-state-adaptation]]
- [[entities/topological-reasoning-offloading.md|topological-reasoning-offloading]]
- [[entities/probability-quality-coupling.md|probability-quality-coupling]]
- [[entities/false-positive-convergence.md|false-positive-convergence]]
- [[entities/exploration-bias.md|exploration-bias]]
- [[entities/symbolic-closure-analysis.md|symbolic-closure-analysis]]
- [[entities/topological-guidance.md|topological-guidance]]

## 📐 개념

- [[concepts/exploration-bias.md|exploration-bias]]
- [[concepts/symbolic-closure-analysis.md|symbolic-closure-analysis]]
- [[concepts/topological-guidance.md|topological-guidance]]

---
_LLM 분석으로 생성됨_
