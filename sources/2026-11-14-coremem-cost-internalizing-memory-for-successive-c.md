# CoReMem: Cost-Internalizing Memory for Successive Coding Tasks with Prospective Valuation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-14
**링크**: http://arxiv.org/abs/2611.17316v1

## 💡 핵심 인사이트

다음 태스크를 모르는 상태에서 쓰이는 메모리의 가치는 쓰기·읽기 비용을 내재화한 사전적 가치 평가로만 합리적으로 정의된다 — 메모리는 무료 저장소가 아니라 비용-가치 투자 결정이다.

## 📖 분석

# CoReMem: Cost-Internalizing Memory for Successive Coding Tasks with Prospective Valuation

**날짜**: 2026-11-14

## 핵심 기여

진화하는 저장소 위에서 연속 코딩 태스크를 수행하는 에이전트를 위한 비용 내재화 메모리 프레임워크. 다음 태스크가 알려지기 전에 메모리를 작성해야 하는 구조적 조건 하에서, 측정된 쓰기·읽기 비용을 메모리 설계와 액터 적응의 목적함수에 내재화하고, 사전적 가치 평가(prospective valuation)로 미래 유용성을 추정한다. 태스크가 전개되는 동안 액터는 가용 메모리에 행동하는 것이 노력을 절약하는 시점을 동적으로 판단한다.

## 기존 Wiki와의 관계

- [[context-as-cost-function]]: 컨텍스트 비용화 원리를 메모리 계층으로 확장한다. 쓰기 비용은 태스크 미지 상태의 빌드타임 투자, 읽기 비용은 실행 중 런타임 예산으로 비용의 시점 분리 구조를 규정한다.
- [[future-query-agnostic-compression]]: 미래 질의 미지수라는 동일 조건 하에서 빈도·희귀성 휴리스틱 대신 비용 기반 사전적 가치 평가를 선택 기준으로 채택한다.
- [[descriptive-decisional-memory-divergence]]: 묘사적 보존이 아닌 결정적 가치 중심 선택의 코딩 도메인 실현 사례다.
- [[expected-value-of-information]]: 도구 호출에서 정의되던 EVI를 '지금 메모리에 써둘 것인가'의 쓰기 결정으로 확장한다.
- [[adaptive-validity]]: 저장 타당성에 '메모리에 행동하는 것이 노력을 절약하는가'라는 활용 타당성 축을 추가한다.
- [[cross-episode-reuse-failure]]: 재사용 실패의 원인을 능력 부족이 아닌 비용 인지 부재로 재해석하는 경로를 제공한다.
- [[metacognition]]: 가용 메모리 활용 시점 판단을 메타인지의 메모리 차원으로 추가한다.
- [[compactionrl]]: CliffCompaction이 태스크 완료 보상으로 압축 정책을 최적화했다면, 본 논문은 최적화 대상을 메모리 쓰기 자체의 비용-가치 판단으로 확장한다.

## 인사이트

메모리는 무료 저장소가 아니라 미래 불확실성 하의 비용-가치 투자 포트폴리오다. 쓰기와 읽기의 비용이 측정·내재화되는 순간 메모리 관리 전체가 투자 결정 문제로 재정의된다.

## 🔗 관련 논문

- CliffCompaction: Cost-Efficient Compaction for Long-Horizon Coding Agents
- Rare, Relevant, and Still Wrong: How Memory Fails LLM Group Decisions
- KV-streams for Efficient Compaction in Agentic Reinforcement Learning
- An Interpretable Memory Decision Controller for LLM Agents

## 🏷️ 엔티티

- [[entities/coremem.md|coremem]]
- [[entities/memory-management.md|memory-management]]
- [[entities/context-as-cost-function.md|context-as-cost-function]]
- [[entities/future-query-agnostic-compression.md|future-query-agnostic-compression]]
- [[entities/descriptive-decisional-memory-divergence.md|descriptive-decisional-memory-divergence]]
- [[entities/expected-value-of-information.md|expected-value-of-information]]
- [[entities/adaptive-validity.md|adaptive-validity]]
- [[entities/value-differential-memory-management.md|value-differential-memory-management]]
- [[entities/cross-episode-reuse-failure.md|cross-episode-reuse-failure]]
- [[entities/metacognition.md|metacognition]]
- [[entities/cost-aware-agent-evaluation.md|cost-aware-agent-evaluation]]
- [[entities/behavior-infrastructure-dual-cost-model.md|behavior-infrastructure-dual-cost-model]]
- [[entities/cost-internalizing-memory.md|cost-internalizing-memory]]
- [[entities/prospective-memory-valuation.md|prospective-memory-valuation]]

## 📐 개념

- [[concepts/cost-internalizing-memory.md|cost-internalizing-memory]]
- [[concepts/prospective-memory-valuation.md|prospective-memory-valuation]]
- [[concepts/successive-task-memory-problem.md|successive-task-memory-problem]]
- [[concepts/memory-as-cost-value-portfolio.md|memory-as-cost-value-portfolio]]

---
_LLM 분석으로 생성됨_
