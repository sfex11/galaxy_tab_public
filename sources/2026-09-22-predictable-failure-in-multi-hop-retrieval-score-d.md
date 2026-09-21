# Predictable Failure in Multi-Hop Retrieval: Score-Distributional Confidence Scoring and Abstention

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-22
**링크**: http://arxiv.org/abs/2609.22056v1

## 💡 핵심 인사이트

검색 실패 감축(abstention)의 가능성은 감지 특징이 담은 상호정보로 결정되며, LLM-judge 특징과 dense 특징의 상보성이 그 한계와 해법을 동시에 규정한다.

## 📖 분석

Multi-hop 검색 실패가 쿼리에 균일하게 분포하지 않고 구조적으로 예측 가능한 하위 모집단에 클러스터링됨을 두 정리로 형식화한 이론 논문이다. 첫째(CWAR Reducibility), confident-failure 감축은 검색 특징이 성공에 대한 상호정보를 가질 때만 가능하며, LLM-judge 파이프라인은 이 조건을 충족하지만 dense-only 설정은 크게 미달하여 두 레짐 간 AUC-AC 격차를 설명한다. 둘째(Feature Regime Complementarity), 특징 레짐들이 성공 예측에 상보적으로 기여한다.

이 발견은 기존 Wiki의 여러 축과 교차한다. [[expected-value-of-information]]의 '감지 신호가 정보를 담는가'라는 전제를 검색 실패 감지에서 필요충분조건으로 형식화하여 EVI 논의에 정리적 근거를 제공한다. [[multi-signal-hallucination-detection]]의 다중 직교 신호 결합 원리(의미·확신·보정)가 특징 레짐 상보성으로 검색 도메인에서 재현된다. [[judge-instrument-reliability]] 관점에서 LLM-judge는 판단자가 아니라 성공-실패 예측 정보를 담는 측정 채널로 기능함이 정량화된다. abstention은 [[early-episode-abort]]의 회복 불가능 궤적 조기 차단과 동형이며, On-Demand Attention의 recall head가 '언제 읽을까'를 예측하듯 score-distributional confidence는 '언제 abstain할까'를 예측한다. 또한 평균 지표가 클러스터된 실패를 은폐한다는 점에서 [[average-metric-concealment]]의 이론적 근거를 제공한다.

## 🔗 관련 논문

- Superintelligent Retrieval Agent: The Next Frontier of Information Retrieval
- RAFT: A Stateful Retrieval-Augmented Framework for Troubleshooting Agents
- On-Demand Attention: Language Models Know When to Recall
- Domain-Specific Hallucination Detection in Large Language Models
- Clarify, Abstain or Answer? Strategising in Conversation with LLMs
- Beyond One-Size-Fits-All: Sample-Adaptive Strategy Routing for Vision Language Model Pruning

## 🏷️ 엔티티

- [[entities/confident-failure-predictability.md|confident-failure-predictability]]
- [[entities/feature-regime-complementarity.md|feature-regime-complementarity]]
- [[entities/score-distributional-confidence.md|score-distributional-confidence]]
- [[entities/expected-value-of-information.md|expected-value-of-information]]
- [[entities/multi-signal-hallucination-detection.md|multi-signal-hallucination-detection]]
- [[entities/judge-instrument-reliability.md|judge-instrument-reliability]]
- [[entities/superintelligent-retrieval-agent.md|superintelligent-retrieval-agent]]
- [[entities/early-episode-abort.md|early-episode-abort]]
- [[entities/average-metric-concealment.md|average-metric-concealment]]

## 📐 개념

- [[concepts/confident-failure-predictability.md|confident-failure-predictability]]
- [[concepts/feature-regime-complementarity.md|feature-regime-complementarity]]
- [[concepts/score-distributional-confidence.md|score-distributional-confidence]]
- [[concepts/mutual-information-abstention-condition.md|mutual-information-abstention-condition]]

---
_LLM 분석으로 생성됨_
