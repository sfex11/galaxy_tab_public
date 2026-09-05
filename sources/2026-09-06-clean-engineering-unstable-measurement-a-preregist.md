# Clean Engineering, Unstable Measurement: A Preregistered Reliability Failure of Black-Box LLM Observers on Shared Endpoints

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-06
**링크**: http://arxiv.org/abs/2609.04198v1

## 💡 핵심 인사이트

LLM judge가 측정 도구로 기능하기 위한 최소 전제인 시간적 재현성이 실증적으로 붕괴되어 있어, judge-gated 파이프라인(훈련 데이터 큐레이션, 리더보드, 모델 비교) 전체의 신뢰성이 재현 불가능한 측정 인프라 위에 세워져 있음을 사전등록 감사로 입증한다.

## 📖 분석

# Clean Engineering, Unstable Measurement: LLM Judge의 측정 도구 신뢰성 실패

LLM judge는 이제 훈련 데이터 게이팅, 생성물 점수화, 리더보드 산출을 구동하는 **측정 도구(measurement instrument)**다. 그런데 모든 측정 도구의 최소 전제—"같은 요청을 같은 모델 이름으로 보내면 내일도 같은 값을 읽는다"—는 거의 명시된 적이 없었다. 본 논문은 이 가정을 두 차례의 **사전등록(preregistered)** 감사로 검증했고, 두 번 모두 도구 검증 단계 자체를 통과하지 못했다.

52,988건의 감사된 요청에서, 같은 윈도우 내 반복 순위의 Spearman 상관은 요구 기준에 한참 못 미치는 0.400에 그쳤다. 이는 특정 judge의 편향 문제가 아니라 **동일 엔드포인트의 시간적 재현성 자체가 붕괴**해 있음을 보여준다.

## Wiki 관점에서의 위치

- [[llm-as-judge]]의 신뢰성 논의를 '판단 품질'에서 '측정 재현성'으로 확장한다. 기존 [[transitivity-violation]]이 동시적 판단 간 추이성 위반이었다면, 이 논문은 시간축 test-retest 불안정성이라는 제3의 실패 축을 추가한다.
- [[certification-monitoring-discontinuity]]의 실증 근거를 제공한다: 측정 도구 자체가 이동하면 인증 시점의 통계적 경계([[statistical-certification]])는 사실상 하루 만에 무효화된다.
- [[evaluator-assumption]]이 지적한 평가자의 암묵적 가정 중 가장 기초적인 것—측정 가능성의 전제—을 정량적으로 감사한 최초 사례다.
- [[benchmarkless-comparative-safety-scoring]]과 [[conditional-reliability-recalibration]]처럼 LLM judge 기반 비교 평가에 의존하는 방법론 전체에 상류 오염이 된다: judge가 불안정하면 합의도 자체가 소음을 측정하는 것이 된다.
- [[mechanistic-probe-unreliability]]와 평행 구조: 내부 프로브와 외부 블랙박스 관찰자 모두 '신뢰할 수 있는 판독기'라는 전제에서 실패한다.
- 사전등록 방법론은 [[score-narrative-conflation]]을 방어하는 문화적 장치이기도 하다: 결과에 앞서 기준을 고정함으로써 불안정한 측정을 서사로 포장하는 것을 차단한다.

## 핵심 인사이트

"Clean Engineering, Unstable Measurement"라는 제목 자체가 논지다: 파이프라인 엔지니어링이 아무리 정교해도, 그 위에 얹힌 측정 도구가 재현 불가능하면 하류의 모든 결정(훈련 데이터 선택, 모델 비교, 리더보드 순위)은 이동하는 모래 위에 세워진다.

## 🔗 관련 논문

- Evaluation of Automatic Speech Recognition Using Generative Large Language Models
- Why Global LLM Leaderboards Are Misleading: Small Portfolios
- When No Benchmark Exists: Validating Comparative LLM Safety
- Bounding the Black Box: A Statistical Certification Framework for AI Risk
- MathDuels: Evaluating LLMs as Problem Posers and Solvers

## 🏷️ 엔티티

- [[entities/llm-as-judge.md|llm-as-judge]]
- [[entities/judge-instrument-reliability.md|judge-instrument-reliability]]
- [[entities/certification-monitoring-discontinuity.md|certification-monitoring-discontinuity]]
- [[entities/evaluator-assumption.md|evaluator-assumption]]
- [[entities/preregistered-measurement-audit.md|preregistered-measurement-audit]]

## 📐 개념

- [[concepts/transitivity-violation.md|transitivity-violation]]
- [[concepts/dynamic-criteria-certification-failure.md|dynamic-criteria-certification-failure]]
- [[concepts/score-narrative-conflation.md|score-narrative-conflation]]
- [[concepts/conditional-reliability-recalibration.md|conditional-reliability-recalibration]]
- [[concepts/benchmarkless-comparative-safety-scoring.md|benchmarkless-comparative-safety-scoring]]

---
_LLM 분석으로 생성됨_
