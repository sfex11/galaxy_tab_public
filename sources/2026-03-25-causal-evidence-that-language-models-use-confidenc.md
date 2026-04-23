# Causal Evidence that Language Models use Confidence to Drive Behavior

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-25
**링크**: http://arxiv.org/abs/2603.22161v1

## 💡 핵심 인사이트

LLM이 내부 신뢰도 추정치를 단순히 보고하는 것이 아니라, 기권(abstention) 등 행동 조절의 인과적 신호로 능동적으로 활용한다는 실험적 증거를 제시한 연구이다.

## 📖 분석

## Causal Evidence that Language Models use Confidence to Drive Behavior

본 논문은 LLM이 내부 신뢰도(confidence) 추정치를 단순히 출력하는 것을 넘어, 이를 **행동 조절의 인과적 신호**로 능동적으로 활용하는지를 검증한다. 메타인지(metacognition) — 자신의 인지 성능을 평가하는 능력 — 는 다양한 생물종에서 관찰되는 현상인데, 저자들은 이를 LLM에 적용하여 4단계 기권(abstention) 패러다임을 설계했다.

**핵심 실험 설계:**
- Phase 1: 기권 옵션 없이 내부 신뢰도 추정치를 확립
- Phase 2-4: 기권 옵션을 도입하여 모델이 신뢰도를 기반으로 응답 여부를 결정하는지 관찰

이 연구는 LLM의 내부 표현(internal representation)과 외부 행동 사이의 **인과적 관계**를 밝히려는 시도로, 기존의 상관관계 기반 분석을 넘어선다. 모델이 자신의 불확실성을 인식하고 이에 따라 행동을 조절한다면, 이는 AI 안전성과 신뢰성 측면에서 중대한 함의를 갖는다. 특히 고위험 의사결정 상황에서 모델이 "모른다"고 스스로 판단하고 기권할 수 있는 능력은 할루시네이션 완화와 직결된다.

기존 연구들이 LLM의 보정(calibration)이나 불확실성 정량화에 초점을 맞춘 반면, 본 논문은 신뢰도가 실제로 모델 행동의 **원인**인지를 실험적으로 규명한다는 점에서 차별화된다. 이는 [[concepts/reinforcement-learning.md|reinforcement learning]]에서의 보상 신호와 유사하게, 내부 신뢰도가 일종의 자기 참조적 피드백 루프로 기능할 가능성을 시사한다.

## 🔗 관련 논문

- 2026 04 07 understanding the role of hallucination in reinfor
- 2026 04 10 tracesafe a systematic assessment of llm guardrail

## 📐 개념

- [[concepts/metacognition.md|metacognition]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/reinforcement-learning.md|reinforcement-learning]]

---
_LLM 분석으로 재생성됨_
