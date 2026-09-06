# Efficient Test-Time Adaptation through Human-AI Interaction

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-06
**링크**: http://arxiv.org/abs/2609.04141v1

## 💡 핵심 인사이트

개인 전문성은 평균 능력에서의 이탈에 존재하며, 문서화되지 않은 개인 기준은 명시적 명세가 아니라 반복적 인간-AI 상호작용을 통해서만 표면화된다.

## 📖 분석

# Efficient Test-Time Adaptation through Human-AI Interaction

## 핵심 주장

AI 에이전트는 인구 규모 데이터로 훈련되어 다수 실무자의 능력을 앙상블하는 폭넓은 능력을 갖추지만, 산출물은 개인 전문가가 명성을 걸 수 있는 품질 기준에 미치지 못한다. 개방형 태스크에서 성공 기준은 이질적이고 문서화되지 않으며, 개인 전문성은 정확히 '평균에서의 상승과 이탈'에 존재한다. 사용자는 자신의 기준을 완전히 명시할 수 없으므로, 반복적 인간-AI 상호작용이 이 암묵적 기준을 표면화하는 효율적 테스트 시점 적응 경로가 된다.

## Wiki에서의 위치

이 논문은 [[concepts/adaptive-inference.md|adaptive inference]]의 적응 차원에 제4의 축을 추가한다. 기존 적응이 외부 환경(CADENCE), 내부 시스템 상태(SpecKV), 신념 상태에 반응했다면, 본 논문은 사용자와의 반복 교환에서 발현되는 **암묵적 개인 기준**에 반응하는 적응 유형을 제시한다.

[[concepts/marginal-distribution-ceiling.md|marginal distribution ceiling]] 관점에서 인구 규모 훈련은 주변 분포가 평균 실무자의 분포를 인코딩하게 만들며, 개인 기준은 조건화되지 않은 암묵적 조건들이다. 이 간극을 메우는 경로가 파라미터 재학습이 아닌 추론 시점 상호작용임을 시사한다.

2026-09-04의 "User Feedback Provides a Unique Signal that LLMs Can not Detect"가 사용자 피드백 신호가 LLM 평가 계층에서 판독되지 않는 문제를 진단했다면, 본 논문은 반복 상호작용 프로토콜로 그 신호를 점진적으로 추출하는 해법 측을 제공하여 문제-해법 쌍을 형성한다.

## 새로운 인사이트

[[concepts/preference-discovery-construction-boundary.md|preference discovery construction boundary]]의 경계 문제에 대한 구체적 사례를 제공한다. 사용자가 표현할 수 없는 기준이 반복적 교환을 통해 표면화될 때, 선호 발견과 구성이 동일한 과정의 두 측면으로 융합된다. [[concepts/goal-operationalization.md|goal operationalization]] 또한 에이전트의 단방향 변환이 아닌 인간-AI 간 공동 구성으로 재정의되어야 함을 보여준다.

## 🔗 관련 논문

- User Feedback Provides a Unique Signal that LLMs Can not Detect

## 🏷️ 엔티티

- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/personal-ai-agent.md|personal-ai-agent]]
- [[entities/user-feedback-signal.md|user-feedback-signal]]
- [[entities/tacit-criteria-surfacing.md|tacit-criteria-surfacing]]

## 📐 개념

- [[concepts/marginal-distribution-ceiling.md|marginal-distribution-ceiling]]
- [[concepts/preference-discovery-construction-boundary.md|preference-discovery-construction-boundary]]
- [[concepts/goal-operationalization.md|goal-operationalization]]
- [[concepts/adaptive-validity.md|adaptive-validity]]
- [[concepts/capability-task-quality-decoupling.md|capability-task-quality-decoupling]]
- [[concepts/human-trace-external-anchoring.md|human-trace-external-anchoring]]
- [[concepts/tacit-criteria-surfacing.md|tacit-criteria-surfacing]]

---
_LLM 분석으로 생성됨_
