# Why Global LLM Leaderboards Are Misleading: Small Portfolios for Heterogeneous Supervised ML

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-10
**링크**: http://arxiv.org/abs/2605.06656v1

## 💡 핵심 인사이트

글로벌 리더보드의 상위 50개 모델 간 쌍대 승률이 최대 0.53에 불과하여 통계적으로 구분 불가능하다는 것은, 글로벌 순위가 모델 능력의 지형이 아니라 측정 노이즈의 지형을 시각화하고 있다는 근본적 비판이다.

## 📖 분석

# 글로벌 LLM 리더보드의 통계적 허상

본 논문은 Arena의 ~89K 쌍대 비교(116개 언어, 52개 LLM)를 분석하여, 글로벌 Bradley-Terry(BT) 순위가 구조적으로 오도된다는 것을 실증한다. 핵심 발견은 두 가지로 요약된다.

**결정적 투표의 2/3가 상쇄된다.** 전역 순위를 구성하는 결정적 투표의 대부분이 서로 상반되어, 최종 순위를 형성하는 유효 신호가 극히 적다. 이는 [[entities/evaluator-assumption|평가자의 가정]]이 전역 순위의 의미론적 타당성을 보장하지 못함을 정량적으로 보여주는 첫 번째 실증이다.

**최상위 50개 모델이 통계적으로 구분 불가능하다.** 글로벌 BT 순위 상위 50개 모델 간 쌍대 승률이 최대 0.53에 불과하여, 순위 차이가 측정 가능한 능력 차이가 아닌 통계적 노이즈에 의해 생성된 것임을 보여준다. 이는 [[entities/ceiling-performance-problem|천장 성능 문제]]가 모델 측이 아닌 측정 도구 측에서도 현현됨을 의미한다.

본 논문은 이종 태스크·언어에 걸친 단일 글로벌 순위라는 [[entities/llm-benchmark|LLM 벤치마크]]의 근본적 전제를 해체한다. 개별 도메인에서 의미 있는 순위가 이종 도메인 간 집계에서 소멸하는 현상은, [[entities/transitivity-violation|추이성 위반]] 문제가 인스턴스 수준을 넘어 집계 메커니즘 수준에서 구조화됨을 시사한다. 작은 포트폴리오(small portfolio) 기반 평가를 대안으로 제시하며, 이는 [[entities/live-benchmark|라이브 벤치마크]]나 [[entities/claw-eval-live|Claw-Eval-Live]]의 도메인 특화 신호가 글로벌 순위보다 정보적으로 우월하다는 논의와 수렴한다.

## 🔗 관련 논문

- why global llm leaderboards are misleading small p
- mathduels-evaluating-llms-as-problem-posers-and-so
- claw-eval-live-a-live-agent-benchmark-for-evolving
- when-no-benchmark-exists-validating-comparative-ll

## 🏷️ 엔티티

- [[entities/llm-benchmark.md|llm-benchmark]]
- [[entities/evaluator-assumption.md|evaluator-assumption]]
- [[entities/ceiling-performance-problem.md|ceiling-performance-problem]]
- [[entities/transitivity-violation.md|transitivity-violation]]
- [[entities/statistical-ranking-indistinguishability.md|statistical-ranking-indistinguishability]]
- [[entities/vote-cancellation-effect.md|vote-cancellation-effect]]
- [[entities/cross-domain-ranking-fallacy.md|cross-domain-ranking-fallacy]]

## 📐 개념

- [[concepts/statistical-ranking-indistinguishability.md|statistical-ranking-indistinguishability]]
- [[concepts/vote-cancellation-effect.md|vote-cancellation-effect]]
- [[concepts/cross-domain-ranking-fallacy.md|cross-domain-ranking-fallacy]]
- [[concepts/small-portfolio-evaluation.md|small-portfolio-evaluation]]

---
_LLM 분석으로 생성됨_
