# Joint Treatment Effect Estimation from Incomplete Healthcare Data: Temporal Causal Normalizing Flows with LLM-driven Evolutionary MNAR Imputation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-08
**링크**: http://arxiv.org/abs/2605.05125v1

## 💡 핵심 인사이트

EHR에서 결측, 인과 추정, 시계열 구조라는 세 가지 문제를 분리하여 다루는 기존 방법론은 MNAR 결측률이 50~80%에 달하는 현실적 조건에서 체계적 편향을 산출하며, 이를 해결하기 위해 LLM 기반 진화적 대체와 시계열 정규화 흐름을 통합한 인과 추정 파이프라인이 필요하다.

## 📖 분석

# Treatment Effect Estimation from Incomplete Healthcare Data

## 정의
전자건강기록(EHR)의 불완전한 시계열 데이터에서 인과적 치료 효과를 추정하는 2단계 파이프라인: (1) LLM 기반 진화적 MNAR(비무작위 결측) 대체, (2) 시계열 인과 정규화 흐름(Normalizing Flow)을 통한 치료 효과 추정.

## 기존 Wiki와의 관계
기존 [[medical-ai]]가 대화적 동정심·가독성 평가(SafetyALFRED 계열)와 근거 기반 QA(ArchEHR-QA)에 집중했다면, 본 논문은 medical-ai의 스코프를 **인과 추론(causal inference)**으로 확장한다. EHR 데이터가 단순한 정보 검색 대상이 아닌 인과적 분석의 원재료로 취급되며, 결측률이 50~80%에 달하는 EHR의 현실적 조건 하에서 추론이 어떻게 붕괴하는지를 문제화한다.

[[uncertainty-quantification]]과의 연결점에서, 본 논문은 불확실성 정량화의 대상을 모델 성능 예측이나 규제적 안전 증명에서 **결측 메커니즘 자체의 모델링**으로 전환한다. MNAR 결측은 데이터가 '의미 있게 누락'되는 현상이므로, 이를 단순한 노이즈가 아닌 인과 그래프의 구조적 요소로 통합해야 함을 시사한다.

## 핵심 기여
세 가지 문제—인과 추정, 결측 메커니즘, 시계열 구조—를 통합적으로 모델링하는 접근법을 제시한다. 기존 방법론들이 이 세 축을 분리하여 다룸으로써 발생하는 편향을, 정규화 흐름이 시계열 인과 구조를 명시적으로 인코딩하고 LLM이 결측 메커니즘의 진화적 탐색을 수행하는 구조로 해결한다.

## 🔗 관련 논문

- 2026-05-01-healthnlp_retrievers-at-archehr-qa-2026-cascaded-l.md
- 2026-05-02-llm-as-clinical-graph-structure-refiner-enhancing-.md
- 2026-04-25-bounding-the-black-box-a-statistical-certification.md

## 🏷️ 엔티티

- [[entities/medical-ai.md|medical-ai]]
- [[entities/uncertainty-quantification.md|uncertainty-quantification]]
- [[entities/target-trial-emulation.md|target-trial-emulation]]
- [[entities/temporal-causal-normalizing-flow.md|temporal-causal-normalizing-flow]]
- [[entities/mnar-imputation.md|mnar-imputation]]
- [[entities/treatment-effect-estimation.md|treatment-effect-estimation]]
- [[entities/time-varying-confounding.md|time-varying-confounding]]

## 📐 개념

- [[concepts/causal-estimation-missingness-joint-modeling.md|causal-estimation-missingness-joint-modeling]]
- [[concepts/llm-driven-imputation.md|llm-driven-imputation]]
- [[concepts/evolutionary-mnar-imputation.md|evolutionary-mnar-imputation]]
- [[concepts/time-varying-confounding-resolution.md|time-varying-confounding-resolution]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-05-07-safety-and-accuracy-follow-different-scaling-laws-]]: 두 논문 모두 의료 데이터와 LLM의 교차점을 다루며, 하나는 결측치가 많은 EHR에서의 인과 추정을, 다른 하나는 임상 LLM에서 안전성이 정확도와 독립적으로 스케일링됨을 보여준다.
