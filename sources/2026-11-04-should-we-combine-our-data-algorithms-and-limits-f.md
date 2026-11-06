# Should We Combine Our Data? Algorithms and Limits for Privately Assessing Data Sharing

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-04
**링크**: http://arxiv.org/abs/2611.03599v1

## 💡 핵심 인사이트

데이터 공유의 가치는 개별 데이터셋 품질의 합이 아니라 라벨링 규범과 선택 편향의 결합 구조가 결정하며, 이 판단 자체가 프라이버시 제약 하의 사전 평가 문제가 된다

## 📖 분석

## 핵심 기여

두 데이터 보유자가 민감한 라벨 데이터셋을 각각 보유할 때 "통합 학습이 이득인가"를 프라이버시 제약 하에서 사전 평가하는 알고리즘과 이론적 한계를 제시한다. 핵심 발견은 **개별적으로 완벽 분류 가능한 데이터셋조차 결합 시 라벨링 표준 충돌·선택 편향으로 인해 가설 클래스 내 단일 분류기가 성립하지 않을 수 있다**는 결합 불가능성이다.

## 기존 Wiki와의 관계

- **[[component-independence-assumption]]**: 데이터셋의 개별 완벽성이 결합 품질을 담보하지 못함을 이론적으로 증명하여, 구성요소 독립성 가정 붕괴의 데이터 축 사례를 제공한다. 팀 교체 연구에서 구성 관계가 성과를 결정했듯, 데이터에서도 보유 구조가 학습 가능성을 결정하는 동형 구조다.
- **[[annotation-model-conflation]]**: 라벨링 표준 충돌은 주석 규범(Extension·Evidence·Authority)의 이질성이 이종 보유자 사이에서 학습 가능성을 파괴하는 현상으로, RLHF 주석 혼재 논의의 데이터 공유 확장이다.
- **[[model-merging]]**: 가중치 병합 간섭(New LoRA Skills)에 대응하는 데이터 병합 간섭의 정식화. 병합 간섭이 파라미터·데이터 양축의 일반 속성임을 보여준다.
- **[[privacy-coordination-tension]]**: 공유 판단 자체가 양측 민감 데이터 접근을 요구하므로, 공유 결정이 프라이버시-협력 긴장의 최소 단위가 된다.
- **[[value-context-dependence]]**: 데이터 결합 가치가 라벨 규범·가설 클래스·선택 편향에 맥락 의존적임을 형식화하여 보편적 데이터 가치 척도의 불가능성에 이론적 근거를 제공한다.

## 새 인사이트

"더 많은 데이터 = 더 좋은 모델"의 가산적 전제가 결합 구조에 의해 깨진다. 결합 가치는 비가산적이고 음수일 수 있어, 공유 이전의 사전 평가 계층([[prewrite-validation]]의 데이터 취득 버전)이 필수가 되며, 데이터 공유가 실행 이전에 검증 가능한 결정으로 승격된다. [[federated-learning]]의 참여 결정 문제와 [[differential-privacy]]의 응용 대상(훈련→공유 사전 평가) 확장도 이 논문이 제시하는 방향이다.

## 🔗 관련 논문

- Component-Aware Differential Privacy for Federated Multilingual Speech
- Trust-Aware Adaptive Disclosure for Inference Privacy Preservation
- Testing Interchangeability in LLM Agent Teams
- New LoRA Skills Should Read but Never Write

## 🏷️ 엔티티

- [[entities/component-independence-assumption.md|component-independence-assumption]]
- [[entities/annotation-model-conflation.md|annotation-model-conflation]]
- [[entities/model-merging.md|model-merging]]
- [[entities/privacy-coordination-tension.md|privacy-coordination-tension]]
- [[entities/value-context-dependence.md|value-context-dependence]]
- [[entities/federated-learning.md|federated-learning]]
- [[entities/differential-privacy.md|differential-privacy]]

## 📐 개념

- [[concepts/joint-dataset-incompatibility.md|joint-dataset-incompatibility]]
- [[concepts/pre-share-private-assessment.md|pre-share-private-assessment]]
- [[concepts/non-additive-data-value.md|non-additive-data-value]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-11-04-tracing-the-scientific-discovery-capacity-of-llms-]]: 모델의 능력과 가치를 아키텍처가 아닌 훈련 데이터의 구성 — 라벨링 규범·선택 편향과 monofact 비율 — 에서 설명하는 데이터 중심 귀속 연구다.
