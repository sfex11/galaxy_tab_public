# MAGIC: Mixed-Granularity Agent Graphs via Incremental Construction with Dense-Reward Reinforcement Learning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-24
**링크**: http://arxiv.org/abs/2609.26667v1

## 💡 핵심 인사이트

협업 토폴로지의 참여 입도(개별 에이전트 vs 집단)는 서브태스크별로 선택되어야 할 독립 설계 변수이며, 밀집 보상 RL과 점진적 구축으로 이 조합적 선택 공간을 학습 가능하게 만들 수 있다.

## 📖 분석

# MAGIC: 혼합 입도 에이전트 그래프 (2026-09-24)

LLM 다중 에이전트 시스템의 협업 토폴로지가 성능과 실행 비용을 동시에 결정한다는 진단에서 출발한다. 기존 토폴로지 생성기는 개별 에이전트 또는 사전 정의된 집단 중 하나의 입도로 고정되는데, 이는 서브태스크별로 상이한 협업 요구를 소각한다. MAGIC의 핵심 통찰은 참여 입도 자체를 서브태스크별 선택 변수로 삼는 것 — 복잡한 서브태스크는 집단 단위 참여가, 단순한 서브태스크는 개체 단위 참여가 최적이다. 이 입도 선택을 점진적 그래프 구축과 밀집 보상 RL로 학습한다.

## 기존 Wiki와의 관계

- [[multi-agent-system]]·[[agent-coordination]]: 조율 단위를 개체에서 '입도 혼합'으로 확장하는 최신 사례
- [[workflow-topology-conditional-optimization]]이 '최적화는 토폴로지에 조건부'라고 진단했다면, MAGIC는 토폴로지 자체를 학습 대상으로 격상시켜 조건-대상 구도를 반전시킨다
- [[granularity-based-skill-organization]]이 스킬을 태스크/스텝 입도로 조직하는 것과 대응 — 입도 선택이 표현 설계의 범용 원리임을 입증
- [[hierarchical-planning]]: 집단이 고정 위임 계층이 아니라 서브태스크별로 선택 가능한 중간 추상화로 재정의됨
- [[reward-sparsity]]: 밀집 보상 설계가 초희소 최종 보상 문제를 회피하게 하는 전제 조건

## 핵심 인사이트

'누가 참여하는가' 이전에 '어떤 입도로 참여하는가'가 성능과 비용을 좌우하는 독립 설계 축이다. 점진적 구축과 밀집 보상은 이산적·조합적 토폴로지 선택 공간을 학습 가능하게 만든다.

## 🔗 관련 논문

- semantic action graph a shared representation for 

## 🏷️ 엔티티

- [[entities/multi-agent-system.md|multi-agent-system]]
- [[entities/agent-coordination.md|agent-coordination]]
- [[entities/task-allocation.md|task-allocation]]
- [[entities/hierarchical-planning.md|hierarchical-planning]]

## 📐 개념

- [[concepts/collaboration-granularity-selection.md|collaboration-granularity-selection]]
- [[concepts/incremental-topology-construction.md|incremental-topology-construction]]
- [[concepts/dense-reward-topology-learning.md|dense-reward-topology-learning]]
- [[concepts/workflow-topology-conditional-optimization.md|workflow-topology-conditional-optimization]]
- [[concepts/granularity-based-skill-organization.md|granularity-based-skill-organization]]
- [[concepts/reward-sparsity.md|reward-sparsity]]
- [[concepts/communication-diversity-exchange-rate.md|communication-diversity-exchange-rate]]

---
_LLM 분석으로 생성됨_
