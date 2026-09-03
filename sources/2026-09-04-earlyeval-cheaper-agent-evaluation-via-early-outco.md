# EarlyEval: Cheaper Agent Evaluation via Early Outcome Prediction

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-04
**링크**: http://arxiv.org/abs/2609.02783v1

## 💡 핵심 인사이트

에이전트 평가 비용은 태스크 수와 태스크당 실행 비용의 곱셈 구조로 분해되며, 조기 결과 예측은 벤치마크 증류와 직교하는 태스크당 비용 축의 새로운 절감 경로다.

## 📖 분석

# EarlyEval: Cheaper Agent Evaluation via Early Outcome Prediction (2026-09-04)

## 핵심 통찰

에이전트 평가 총비용은 '태스크 수 × 태스크당 실행 비용'의 곱셈 구조다. 기존 연구인 벤치마크 증류(benchmark distillation)는 태스크 수 축만 줄였고, 본 논문은 태스크당 실행 비용 축을 개척한다: 궤적 초반에 최종 성공/실패를 예측하고(early outcome prediction) 확신이 임계치를 넘으면 실행을 조기 중단한다.

## 기존 Wiki와의 관계

- [[benchmark]]: 기존 논의(MathDuels, RoboGrid)가 '무엇을 측정할까'에 집중했다면, 본 논문은 '얼마나 비싸게 측정하는가'를 독립 문제로 격상시킨다. 프론티어 모델의 벤치마크 1회 통과가 수천 달러인 현실에서 벤치마크의 경제학이 등장한다.
- [[adaptive-inference]]: 조기 중단 결정은 [[speckv]]의 압축 상태 반응형 γ 선택과 구조적으로 동형이나, 적응 시점이 배포가 아닌 평가라는 차이가 있다.
- [[early-episode-abort]]: doomed trajectory 조기 감지를 생산(개입)에서 평가(측정)로 전용한다.
- [[behavior-infrastructure-dual-cost-model]]: (호출 비용)×(호출 횟수) 곱셈 분해가 평가 도메인에서 (태스크당 비용)×(태스크 수)로 재현되며, 각 축이 독립적으로 최적화 대상임을 공유한다.

## 난제와 시사점

조기 중단의 예측 오류는 벤치마크 결과 자체의 왜곡으로 이어진다. 벤치마크 증류가 표본 수의 통계적 트레이드오프라면, 조기 예측은 '측정 충실도 vs 계산 비용' 트레이드오프를 도입하여 [[benchmark-specification-gap]] 계열의 측정 타당성 논의에 새 하위 축을 추가한다. [[process-reward-model]]이 중간 스텝을 학습 보상으로 평가한다면, 조기 결과 예측은 동일한 중간 신호를 측정 중단 결정에 사용한다는 점에서 용도가 다르다. 같은 시기의 Efficient SWE Agent Benchmarking via Trajectory-Aware...와 함께, 에이전트 평가의 실행 비용이 독립 연구 축으로 성장하는 신호다.

## 🔗 관련 논문

- Efficient SWE Agent Benchmarking via Trajectory-Aware ...
- Claw-Eval-Live: A Live Agent Benchmark for Evolving Real-World Workflows

## 🏷️ 엔티티

- [[entities/benchmark.md|benchmark]]
- [[entities/adaptive-inference.md|adaptive-inference]]

## 📐 개념

- [[concepts/early-outcome-prediction.md|early-outcome-prediction]]
- [[concepts/evaluation-cost-decomposition.md|evaluation-cost-decomposition]]
- [[concepts/early-episode-abort.md|early-episode-abort]]
- [[concepts/cost-aware-agent-evaluation.md|cost-aware-agent-evaluation]]
- [[concepts/process-reward-model.md|process-reward-model]]

---
_LLM 분석으로 생성됨_
