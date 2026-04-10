# Analysing the Safety Pitfalls of Steering Vectors

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-27
**링크**: http://arxiv.org/abs/2603.24543v1

## 💡 핵심 인사이트

활성화 스티어링 벡터가 LLM의 안전성 guardrail을 일관되게 우회할 수 있어, alignment 도구인 동시에 새로운 공격 표면이 될 수 있다는 이중성을 체계적으로 실증했다.

## 📖 분석

## Analysing the Safety Pitfalls of Steering Vectors

본 논문은 Contrastive Activation Addition(CAA) 기반 **활성화 스티어링(activation steering)**의 안전성 문제를 체계적으로 감사한 연구다. 활성화 스티어링은 가중치 업데이트 없이 LLM 행동을 조정할 수 있는 강력한 도구로 주목받고 있으나, 그 안전성 함의는 충분히 탐구되지 않았다.

### 핵심 발견

JailbreakBench를 활용한 통합 평가 프로토콜 하에서, 스티어링 벡터가 **일관되게 안전성을 저하**시킬 수 있음을 실증적으로 보여준다. 이는 스티어링 벡터의 취약성(brittleness)과 비신뢰성이 잘 알려진 것과 달리, 안전성 측면의 위험이 과소평가되어 왔음을 시사한다.

### 기존 연구와의 관계

이 연구는 [[What Drives Representation Steering? A Mechanistic Case Study|representation steering의 메커니즘적 분석]]과 직접적으로 연결된다. 해당 연구가 스티어링이 *어떻게* 작동하는지를 activation patching으로 분석했다면, 본 논문은 그 스티어링이 *안전성에 어떤 위험*을 초래하는지를 평가한다. 두 연구를 함께 보면 representation steering의 메커니즘과 위험성을 입체적으로 이해할 수 있다.

또한 [[Box Maze: A Process-Control Architecture for Reliable LLM Reasoning|adversarial prompting 대응 연구]]들과도 관련이 깊다. 스티어링 벡터가 jailbreak 공격의 새로운 경로가 될 수 있다는 점에서, LLM 안전성 guardrail 설계 시 추론 무결성뿐 아니라 활성화 수준의 조작 가능성도 고려해야 함을 보여준다.

### 시사점

활성화 스티어링은 alignment 연구에서 유망한 기법이지만, 공격 표면(attack surface)으로도 작용할 수 있다는 이중성을 명확히 한 점에서 AI safety 분야에 중요한 기여를 한다.

## 🔗 관련 논문

- 2026 04 11 what drives representation steering a mechanistic
- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 11 act wisely cultivating meta cognitive tool use in

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/representation-steering.md|representation-steering]]
- [[concepts/activation-patching.md|activation-patching]]
- [[concepts/mechanistic-interpretability.md|mechanistic-interpretability]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/adversarial-prompting.md|adversarial-prompting]]
- [[concepts/llm-alignment.md|llm-alignment]]

---
_LLM 분석으로 재생성됨_
