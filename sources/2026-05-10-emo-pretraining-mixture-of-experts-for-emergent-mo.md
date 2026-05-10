# EMO: Pretraining Mixture of Experts for Emergent Modularity

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-10
**링크**: http://arxiv.org/abs/2605.06663v1

## 💡 핵심 인사이트

MoE의 진정한 모듈성은 라우팅 효율화가 아니라 사전학습 목적 함수 설계에서 비로소 발현되며, 도메인별 전문가 독립성은 사후적 분할이 아닌 훈련 초기부터 의도적으로 조직되어야 한다.

## 📖 분석

# EMO: Pretraining Mixture of Experts for Emergent Modularity

EMO는 MoE(Mixture-of-Experts) 아키텍처가 가진 근본적 모듈성 한계—도메인별 전문가 부분집합으로 추론을 제한하면 성능이 심각하게 저하된다는 문제—를 사전학습 목적 함수 설계로 해결하는 접근법이다. 기존 MoE가 라우팅 효율화에 집중한 반면, EMO는 전문가가 사전학습 과정에서 **기능적 모듈로 자가조직**되도록 유도하여, 특정 도메인에 해당하는 전문가만으로도 성능 저하 없는 추론을 가능하게 한다.

이는 [[entities/mixture-of-experts|mixture-of-experts]]의 이해를 근본적으로 전환한다. 기존 MoE에서 '전문가 특화'는 토큰 단위 라우팅의 부산물에 불과했으나, EMO는 모듈성이 사전학습 단계에서 **의도적 설계 대상**이 되어야 함을 보여준다. 또한 [[entities/on-device-inference|on-device-inference]]의 실현 경로를 모델 압축(양자화·프루닝)에서 아키텍처 수준의 선택적 활성화로 확장하며, [[concepts/marginal-distribution-ceiling|주변 분포 성능 상한선]] 관점에서는 도메인별 전문가 부분집합이 해당 도메인의 P(y)를 보존하는 조건을 사전학습에서 어떻게 달성하는지를 구체화한다.

[[entities/non-linear-task-scaling|non-linear-task-scaling]]과의 교차점에서도 흥미롭다—전문가 모듈성이 태스크 스케일링과 어떻게 상호작용하는지, 모듈 간 독립성이 스케일링 효율에 미치는 영향이 후속 연구 주제가 된다.

## 🔗 관련 논문

- 2026-05-09-emo-pretraining-mixture-of-experts-for-emergent-mo

## 🏷️ 엔티티

- [[entities/mixture-of-experts.md|mixture-of-experts]]
- [[entities/on-device-inference.md|on-device-inference]]
- [[entities/marginal-distribution-ceiling.md|marginal-distribution-ceiling]]

## 📐 개념

- [[concepts/emergent-modularity.md|emergent-modularity]]
- [[concepts/pretraining-induced-expert-specialization.md|pretraining-induced-expert-specialization]]
- [[concepts/domain-selective-inference.md|domain-selective-inference]]

---
_LLM 분석으로 생성됨_
