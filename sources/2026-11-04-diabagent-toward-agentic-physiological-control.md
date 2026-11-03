# DiabAgent: Toward Agentic Physiological Control

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-04
**링크**: http://arxiv.org/abs/2611.03601v1

## 💡 핵심 인사이트

사전학습 스케일링이 향상시키는 임상 질의응답 능력은 생리학적 제어 능력을 담보하지 않으며, 의료 LLM의 배포 가능성 판정은 후자의 지속 개입 평가에 달려 있다.

## 📖 분석

### DiabAgent: 임상 QA에서 생리학적 제어로 (2026-11-04)

의료 LLM 연구의 평가 대상을 질의응답에서 지속 개입에 의한 생리학적 제어로 전환한다. 1형 당뇨 설정에서 에이전트는 식사·운동·질병·혈당 측정 정보를 통합해 인슐린 용량을 지속 조정해야 하며, 이는 기존 임상 QA 벤치마크([[archehr-qa]], [[grounded-clinical-qa]])가 측정하지 못하는 능력군을 격리 측정한다.

핵심 명제: 임상 QA 능력과 생리 제어 능력은 분리된 축이다. 사전학습 스케일링이 QA를 향상시켜도 제어 능력을 담보하지 않으므로, 이는 [[evaluation-deployment-unit-mismatch]]와 [[benchmark-specification-gap]]의 의료 도메인 실현이다 — 평가 단위(단일 턴 답변)와 배포 단위(다중 일 지속 개입)의 구조적 단절.

기존 논의와의 연결: 인슐린 용량 오류는 지연되고 비가역적인 저혈당을 초래하여 [[irreversible-mid-trajectory]]와 [[safety-critical-control]]의 체화 버전을 제공한다. 용량 결정이 누적 생리 이력에 의존하는 것은 [[temporal-state-dependency]]의 사례이며, 질병에 의한 포도당 동역학 변화는 [[non-stationary-dynamics]]를 유발한다. 혈당 수치라는 측정 가능한 결과는 [[rlvr]]의 훈련 신호 경로를, 생리 동역학에 대한 내부 모델 요구는 [[world-model]]의 생리학 확장을 연다.

## 🔗 관련 논문

- Advancing Clinical Genomic Analysis with a Skill-Centred Agent

## 🏷️ 엔티티

- [[entities/diabagent.md|diabagent]]
- [[entities/medical-ai.md|medical-ai]]
- [[entities/ai-decision-making.md|ai-decision-making]]
- [[entities/safety-critical-control.md|safety-critical-control]]

## 📐 개념

- [[concepts/agentic-physiological-control.md|agentic-physiological-control]]
- [[concepts/evaluation-deployment-unit-mismatch.md|evaluation-deployment-unit-mismatch]]
- [[concepts/benchmark-specification-gap.md|benchmark-specification-gap]]
- [[concepts/temporal-state-dependency.md|temporal-state-dependency]]
- [[concepts/non-stationary-dynamics.md|non-stationary-dynamics]]
- [[concepts/world-model.md|world-model]]
- [[concepts/closed-loop-evaluation.md|closed-loop-evaluation]]
- [[concepts/irreversible-mid-trajectory.md|irreversible-mid-trajectory]]
- [[concepts/rlvr.md|rlvr]]
- [[concepts/model-predictive-control.md|model-predictive-control]]

---
_LLM 분석으로 생성됨_
