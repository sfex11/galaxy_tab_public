# Clean Engineering, Unstable Measurement: A Preregistered Reliability Failure of Black-Box LLM Observers on Shared Endpoints

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-07
**링크**: http://arxiv.org/abs/2609.04198v1

## 💡 핵심 인사이트

LLM judge가 측정 기기라면 그 재현성('같은 요청은 같은 판독값') 자체가 검증 대상이며, black-box 공유 엔드포인트에서 이 전제가 실증적으로 붕괴하면 사전등록·임계값 고정 등 아무리 깨끗한 연구 설계도 측정 도구 검증 없이는 무효가 된다.

## 📖 분석

LLM judge가 훈련 데이터 게이팅, 생성물 채점, 리더보드를 좌우하는 측정 기기(measurement instrument)임에도, '같은 요청은 내일도 같은 판독값을 낸다'는 암묵적 전제는 거의 검증된 적이 없다. 본 논문은 이 전제를 사전등록된 두 캠페인으로 감사했고, 결과는 측정 도구 자체의 실패였다: 52,988건의 감사된 요청 시도에서 same-window 반복 순위 합의가 Spearman 0.400에 그쳐 요구 기준을 넘지 못했다.

기존 Wiki와의 관계에서 중요한 것은 평가 축의 확장이다. [[transitivity-violation]]이 동일 세션 내 judge 판단의 추이성 위반을 다뤘다면, 본 논문은 시간축 비일관성을 추가한다 — 판단 비일관성의 원인이 모델의 추론 논리만이 아니라 공유 엔드포인트 상의 기기 드리프트일 수 있음을 보여준다. 이는 [[statistical-certification]]이 전제하는 측정 도구의 시간 불변성을 무너뜨리며, [[certification-monitoring-discontinuity]]에 '도구 드리프트'라는 제3의 단절 축을 제안한다. 인증 무효화가 평가 기준 변화뿐 아니라 측정 기기 변화에서도 발생함이 입증된 것이다.

방법론적으로는 사전등록 연구의 모범 사례다: 모든 임계값을 사전에 고정하고 측정 전 도구 검증을 선행 조건으로 삼아, 두 캠페인 모두 본 실험 전 도구 검증 단계에서 차단됐다. [[preregistered-measurement-audit]]이 '연구 실패의 조기 차단 장치'로 작동한 희귀 실증 사례이며, 잘 설계된(clean) 실험조차 측정 도구가 불안정하면 무의미하다는 제목의 자기 증명을 완성한다.

[[llm-benchmark]] 리더보드 관점에서는 점수 변동이 모델 능력 변화가 아니라 측정 기기 변화에서 비롯될 수 있다는 새로운 혼입 원천을 제시하며, '언제 측정했는가'를 평가 메타데이터의 필수 항목으로 격상시킨다. 이는 [[score-narrative-conflation]]의 진단 — 점수를 능력 서사로 곧장 연결하는 오류 — 에 선행 검증 단계를 요구하는 실증적 근거가 된다.

## 🔗 관련 논문

- Clean Engineering, Unstable Measurement: A Preregistered Rel
- Legibility is Not Interpretability: Comparing Judged and Act
- Evaluation of Automatic Speech Recognition Using Generative
- Why Global LLM Leaderboards Are Misleading: Small Portfolios
- When No Benchmark Exists: Validating Comparative LLM Safety

## 🏷️ 엔티티

- [[entities/judge-instrument-reliability.md|judge-instrument-reliability]]
- [[entities/preregistered-measurement-audit.md|preregistered-measurement-audit]]
- [[entities/llm-as-judge.md|llm-as-judge]]
- [[entities/transitivity-violation.md|transitivity-violation]]
- [[entities/statistical-certification.md|statistical-certification]]
- [[entities/certification-monitoring-discontinuity.md|certification-monitoring-discontinuity]]
- [[entities/llm-benchmark.md|llm-benchmark]]
- [[entities/score-narrative-conflation.md|score-narrative-conflation]]
- [[entities/agreement-based-reliability.md|agreement-based-reliability]]
- [[entities/dynamic-criteria-certification-failure.md|dynamic-criteria-certification-failure]]

## 📐 개념

- [[concepts/black-box-instrument-drift.md|black-box-instrument-drift]]
- [[concepts/measurement-repeatability.md|measurement-repeatability]]
- [[concepts/same-request-same-reading-assumption.md|same-request-same-reading-assumption]]

---
_LLM 분석으로 생성됨_
