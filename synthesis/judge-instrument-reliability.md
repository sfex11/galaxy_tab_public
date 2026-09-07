# Judge Instrument Reliability: 합성 분석

**생성일**: 2026-09-07  
**관련 논문**: 3편  
**최종 업데이트**: 2026-09-07

# Judge Instrument Reliability: 합성 분석

> **업데이트 노트**: 2026-09-06의 초기 합성(Clean Engineering 단일 논문 기준)을 09-07 신규 등재된 Legibility 논문으로 확장했다. Clean Engineering의 두 엔트리(arXiv:2609.04198 중복 등재)는 각각 '실패 입증'과 '방법론적 함의'를 강조하므로 상보적으로 통합했다.

## 1. 공통 주제: '판단자'에서 '측정 기기'로

세 엔트리는 LLM judge를 의견을 내는 판단자가 아니라 **측정 기기(measurement instrument)**로 재정의하고, 기기로서의 자격을 두 직교 축에서 공격한다.

- **재현성 축** (Clean Engineering): 사전등록 감사 2회가 모두 도구 검증 단계에서 차단됐다. 52,988건 감사 요청에서 same-window 반복 순위 합의가 Spearman 0.400에 그쳐 기준 미달 — 특정 judge의 편향이 아니라 공유 엔드포인트의 시간적 재현성 자체의 붕괴다. 09-07 엔트리는 이를 확장해 도구 드리프트를 [[concepts/certification-monitoring-discontinuity|certification-monitoring-discontinuity]]의 제3 단절 축으로 제시하고, 리더보드 메타데이터에 '측정 시점' 격상과 사전등록의 조기 차단 기능([[entities/preregistered-measurement-audit|preregistered-measurement-audit]])을 도출한다.
- **타당성 축** (Legibility): judge가 판단한 CoT 단계 중요도와 인과적 개입으로 측정한 실제 기능적 중요도가 체계적으로 발산한다. 가독성 ≠ 해석가능성. PRM·generative critics의 공통 전제인 "trace 텍스트가 계산의 기능적 역할을 담는다"를 직접 타격한다.

## 2. 논문 간 관계

- **보완**: 두 축은 직교적이다. 기기는 안정적이지만 잘못된 대상을 잴 수도, 불안정하지만 우연히 올바른 대상을 잴 수도 있다. 합성 결론은 "재현성과 구성 타당성 모두 미확보"라는 완결적 비판이다.
- **일치**: 모두 black-box 관찰의 한계를 개입적(interventional) 검증으로 극복하려 하며, 내부 프로브와 외부 관찰자가 동일하게 실패한다는 [[concepts/mechanistic-probe-unreliability|mechanistic-probe-unreliability]]의 평행 구조를 공유한다.
- **모순**: 없음. Legibility 쪽이 명시적으로 본 엔티티의 범위를 '일관성'에서 '측정 대상 타당성'으로 확장한다고 선언한다.

## 3. 파급 효과

판단 비일관성의 실패 지도가 3차원화됐다: 동시축([[concepts/transitivity-violation|transitivity-violation]]), 시간축(본 논문), 대상축([[entities/judged-actual-importance-divergence|judged-actual-importance-divergence]]). judge-gated 인프라 전반 — 훈련 데이터 큐레이션, 리더보드, 통계 인증, process reward — 이 상류 오염을 피할 수 없다. [[concepts/score-narrative-conflation|score-narrative-conflation]]의 진단에 선행 검증 요구라는 실증적 근거가 붙었다.

## 4. 연구 트렌드와 향후 방향

1. 평가 연구의 **메트롤로지 전환**: 판단 품질·편향 논의에서 재현성·타당성의 기기 검증으로.
2. 도구 검증의 **본 실험 선행 조건화**: 잘 설계된 실험도 불안정한 기기 위에서는 무의미하다는 자기 증명.
3. **개입의 gold-standard화**: '판독 문제'에서 '개입 문제'로의 해석가능성 재정의.
4. 미해결 과제: 엔드포인트 버저닝·드리프트 모니터링 인프라, 재현성 인증 체계, judge + 인과 검증 하이브리드 설계. 단, 불안정한 judge 위의 합의는 소음을 측정할 뿐이므로 단순 앙상블은 해법이 아니다.

## 5. 관련 엔티티

[[entities/llm-as-judge|llm-as-judge]] · [[entities/preregistered-measurement-audit|preregistered-measurement-audit]] · [[entities/legibility-interpretability-gap|legibility-interpretability-gap]] · [[entities/judged-actual-importance-divergence|judged-actual-importance-divergence]] · [[concepts/statistical-certification|statistical-certification]] · [[concepts/evaluator-assumption|evaluator-assumption]] · [[concepts/benchmark-specification-gap|benchmark-specification-gap]] · [[concepts/surface-completeness-misreading|surface-completeness-misreading]]