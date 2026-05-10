# Measuring Faithfulness Depends on How You Measure: Classifier Sensitivity in LLM Chain-of-Thought Evaluation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-24
**링크**: http://arxiv.org/abs/2603.20172v1

## 💡 핵심 인사이트

CoT 충실성은 모델의 객관적 속성이 아니라 분류기 선택에 따라 극적으로 달라지는 측정 의존적 구성물이며, 이는 단일 메트릭 기반 LLM 평가의 신뢰성에 근본적 의문을 제기한다.

## 📖 분석

## Measuring Faithfulness Depends on How You Measure: Classifier Sensitivity in LLM Chain-of-Thought Evaluation

본 논문은 LLM의 Chain-of-Thought(CoT) 충실성(faithfulness) 평가가 측정 방법에 따라 크게 달라진다는 점을 실증적으로 보여준다. 기존 연구들이 "DeepSeek-R1은 힌트를 39% 인정한다"와 같은 단일 집계 수치를 보고하며 충실성이 객관적으로 측정 가능한 속성인 것처럼 제시해왔으나, 이 논문은 그렇지 않음을 증명한다.

세 가지 분류기(정규식 기반 탐지기, 정규식+LLM 2단계 파이프라인, 독립적 Claude Sonnet 4 판정자)를 7B~1T 파라미터 규모의 9개 모델 패밀리 12개 오픈웨이트 모델에서 생성된 10,276개 추론 트레이스에 적용했다. 핵심 발견은 분류기 선택에 따라 동일 모델의 충실성 점수가 극적으로 변화한다는 것이다.

이는 LLM 평가 방법론의 근본적 한계를 드러내는 연구로, 단일 메트릭에 의존한 모델 비교의 위험성을 경고한다. CoT 충실성은 모델의 고유 속성이 아니라 측정 프레임워크와 모델의 상호작용에서 나오는 구성물(construct)임을 시사한다. 이는 AI 안전성 평가에서도 중요한 함의를 가지며, 충실성 평가의 표준화 및 다중 분류기 앙상블 접근의 필요성을 제기한다.

기존 reasoning-chain 및 reasoning-chain-evaluation 개념과 직접적으로 연결되며, AI 안전성(ai-safety) 관점에서 모델의 내부 추론 과정 투명성 문제와도 밀접하다.

## 🔗 관련 논문

- 2026 04 08 triattention efficient long reasoning with trigono
- 2026 04 09 claw eval toward trustworthy evaluation of autonom
- 2026 04 10 tracesafe a systematic assessment of llm guardrail

## 📐 개념

- [[concepts/reasoning-chain-evaluation.md|reasoning-chain-evaluation]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/reasoning-chain.md|reasoning-chain]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[concepts/procedural-faithfulness.md|procedural faithfulness]]
