# Stellar Colosseum: A Many-Agent Harness for Long-Horizon Research in Mathematics and Theoretical Computer Science

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-16
**링크**: http://arxiv.org/abs/2609.15983v1

## 💡 핵심 인사이트

장기 수학 연구의 병목은 증명 작성 능력이 아니라 '대안을 언제 탐색하고 언제 분해에 커밋할 것인가'라는 메타 수준 조율이며, 이를 모델 불가지론적 다수 에이전트 하네스가 추론 배분을 통해 담당할 수 있다.

## 📖 분석

Stellar Colosseum은 수학·이론컴퓨터과학의 장기 호라이즌 연구를 위한 모델 불가지론적 다수 에이전트 하네스다. 진단은 명확하다 — LLM은 짧은 증명은 그럴듯하게 생산하지만, 불확실하고 상호의존적인 결정의 연쇄로 구성된 장기 연구에서는 신뢰성이 무너진다. 이는 [[concepts/proof-planning-horizon.md|proof planning horizon]]이 다룬 호라이즌 문제의 실행 수준 규정이자 [[concepts/unrecoverable-reasoning-error.md|unrecoverable reasoning error]]의 수학 도메인 근거다.

핵심 설계는 3계층이다: (1) 증명 구성 전에 대안 전략을 병렬 탐색하는 단계 — [[concepts/alternative-decision-trajectory.md|alternative decision trajectory]]의 수학 연구 실현, (2) 경로가 분해에 충분히 성숙했는지 판단하는 준비도 게이트 — [[concepts/adaptive-validity.md|adaptive validity]]의 '상태 타당성 재평가' 원리를 분해 개시 판단으로 특화한 것, (3) 정리를 분해 가능한 구조로 표현. 이로써 [[entities/agentic-harness-engineering.md|agentic harness engineering]]의 범위가 실행 인프라에서 연구 오케스트레이션으로 확장되며, [[concepts/inference-budget-progressive-investment.md|inference budget progressive investment]]의 예산 점진 투입이 '병렬 경로 간 배분 + 성숙도 기반 커밋'으로 구체화된다. 모델 불가지론성은 하네스 기여가 모델 능력과 분리 가능함([[concepts/model-harness-decomposability.md|model harness decomposability]])을 전제한다.

[[entities/ai-co-mathematician.md|ai co mathematician]]이 실패 가설 추적 중심의 다중 에이전트 수학 가속이었다면, 본 논문은 '언제 커밋할 것인가'라는 메타 결정을 하네스가 담당함을 제시한다. [[concepts/autoresearch.md|autoresearch]]가 연구 단계 간 파이프라인 자동화였다면, 본 논문은 단일 과제 내부의 심층 탐색 축으로 보완한다.

## 🔗 관련 논문

- AI Co-Mathematician: Accelerating Mathematicians with Agenti
- Autonomous Research for Open-Ended Problems: A Case Study
- Avatar: Toward Autonomous End-to-End Orchestration of Scient

## 🏷️ 엔티티

- [[entities/stellar-colosseum.md|stellar-colosseum]]
- [[entities/agentic-harness-engineering.md|agentic-harness-engineering]]
- [[entities/ai-co-mathematician.md|ai-co-mathematician]]
- [[entities/proof-planning-horizon.md|proof-planning-horizon]]
- [[entities/alternative-decision-trajectory.md|alternative-decision-trajectory]]
- [[entities/adaptive-validity.md|adaptive-validity]]
- [[entities/inference-budget-progressive-investment.md|inference-budget-progressive-investment]]
- [[entities/unrecoverable-reasoning-error.md|unrecoverable-reasoning-error]]
- [[entities/autoresearch.md|autoresearch]]

## 📐 개념

- [[concepts/readiness-gate.md|readiness-gate]]
- [[concepts/parallel-strategy-exploration.md|parallel-strategy-exploration]]
- [[concepts/theorem-decomposition-representation.md|theorem-decomposition-representation]]
- [[concepts/model-agnostic-harness.md|model-agnostic-harness]]

---
_LLM 분석으로 생성됨_
