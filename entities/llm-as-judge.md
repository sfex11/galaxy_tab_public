# llm-as-judge

**카테고리**: 미분류
**생성일**: 2026-04-25

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-04-25-evaluation-of-automatic-speech-recognition-using-g.md|Evaluation of Automatic Speech Recognition Using Generative ]]

### Evaluation of Automatic Speech Recognition Using Generative Large Lang (2026-04-26)

LLM-as-Judge의 적용 범위가 텍스트 생성 평가를 넘어 ASR 후보 선택·의미 거리 계산 등 음성 도메인으로 확장됨을 보여주며, 특히 두 후보 간 강제 선택 방식에서 추이성 위반 문제가 어떻게 현현하는지 검증할 필요성을 제기한다.

### Evaluation of Automatic Speech Recognition Using Generative Large Lang (2026-04-27)

텍스트 도메인에서 음성 도메인으로의 확장이 단순한 도메인 전이가 아니라, 평가 대상의 근본적 속성 변화(형식 vs 의미)를 수반함을 ASR 평가 사례를 통해 명시화하여, 기존 인스턴스 수준 추이성 위반 논의에 '평가 대상 규정 문제'를 추가한다.

### When No Benchmark Exists: Validating Comparative LLM Safety Scoring Wi (2026-05-10)

LLM 판정자의 신뢰성을 근본적 능력 문제가 아닌 '판정자 고정'이라는 계약 조건으로 재구성하여, LLM-as-Judge의 한계를 프레임워크 내 파라미터로 흡수하는 설계 전략을 보여준다.

### User Feedback Provides a Unique Signal that LLMs Can not Detect (2026-09-04)

LLM 판정자가 사용자 피드백의 고유 신호를 감지하지 못한다는 결과는, LLM-as-Judge 평가 체계가 학습 신호의 가치를 구조적으로 과소평가할 수 있음을 보여주며 평가자 선택의 인식론적 위험을 부각시킨다.

### Clean Engineering, Unstable Measurement: A Preregistered Reliability F (2026-09-06)

LLM judge를 '판단자'가 아닌 '측정 도구(instrument)'로 재정의하고, 그 도구가 전제하는 시간적 재현성(test-retest reliability)이 실증적으로 붕괴되어 있음을 사전등록 감사로 보여준다. 기존의 편향·추이성 논의에 '같은 요청-같은 모델 이름-다른 시점 = 다른 판독값'이라는 제3의 실패 축을 추가한다.

### Legibility is Not Interpretability: Comparing Judged and Actual Import (2026-09-06)

판단의 추이성 위반이라는 '일관성' 문제를 넘어, 판단 대상(추론 스텝)의 텍스트가 기능적 역할 정보를 담지 않는다는 '측정 가능성' 수준의 근본 한계를 부여한다. judge의 중요도 판단이 인과적 기여와 발산함이 실증되어, judge 기반 step 평가의 타당성 기반 자체가 흔들린다.

### Clean Engineering, Unstable Measurement: A Preregistered Reliability F (2026-09-07)

LLM-as-Judge 논의의 축을 '판단 품질'(정확도·편향·추이성)에서 '측정 기기 신뢰성'(재현성·안정성)으로 확장한다. transitivity-violation 연구가 세션 내 비일관성을 다뤘다면, 본 논문은 시간이 지나면 동일 요청이 다른 판독값을 내는 시간축 비안정성을 실증하여, judge 실패 모드에 기기 드리프트라는 차원을 추가한다.

→ [[sources/2026-09-07-clean-engineering-unstable-measurement-a-preregist.md|상세 보기]]
