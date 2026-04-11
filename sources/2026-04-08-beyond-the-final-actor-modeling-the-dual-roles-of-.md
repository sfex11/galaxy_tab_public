# Beyond the Final Actor: Modeling the Dual Roles of Creator and Editor for Fine-Grained LLM-Generated Text Detection

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-08
**링크**: http://arxiv.org/abs/2604.04932v1

## 💡 핵심 인사이트

LLM 텍스트 탐지에서 Creator-Editor 이중 역할을 명시적으로 모델링함으로써, 기존 이진 분류로는 구분 불가능했던 LLM-polished 인간 텍스트와 humanized LLM 텍스트를 정책적으로 구분 가능한 4클래스 세밀 탐지 체계를 제시했다.

## 📖 분석

## Beyond the Final Actor: Fine-Grained LLM-Generated Text Detection

본 논문은 LLM 생성 텍스트 탐지를 기존의 이진/삼진 분류에서 벗어나 **4클래스 세밀 분류(fine-grained four-class classification)** 체계로 확장한다. 순수 인간 작성, 순수 LLM 생성, LLM이 다듬은 인간 텍스트(LLM-polished), 인간이 수정한 LLM 텍스트(humanized LLM)를 구분하며, 각 유형이 정책적으로 다른 결과를 초래할 수 있음을 강조한다.

핵심 기여는 텍스트 생성 과정에서 **Creator(최초 작성자)와 Editor(편집자)의 이중 역할**을 명시적으로 모델링한 점이다. 기존 연구가 최종 출력만을 기준으로 판별했다면, 본 연구는 작성-편집 파이프라인의 구조를 반영하여 더 정교한 탐지를 가능하게 한다.

이 연구는 LLM 정렬([[llm-alignment]]) 및 AI 안전([[ai-safety]]) 분야와 밀접하게 연결된다. LLM 출력의 신뢰성과 책임 소재를 판별하는 것은 규제와 거버넌스의 핵심 과제이기 때문이다. 또한 [[reasoning-integrity]] 개념과도 관련되는데, 텍스트의 출처와 편집 이력을 추적하는 것은 추론 과정의 무결성 검증과 유사한 문제 구조를 갖는다.

[[adversarial-prompting]] 연구에서 다루는 LLM 출력 조작 탐지와도 연결점이 있으며, 특히 humanized LLM 텍스트는 탐지 회피를 위한 적대적 전략으로 활용될 수 있어 보안 관점에서도 중요하다. [[binary-analysis]]에서의 패턴 탐지 방법론과 텍스트 수준의 출처 판별 간 방법론적 유사성도 주목할 만하다.

## 🔗 관련 논문

- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 11 ads in ai chatbots an analysis of how large langua
- 2026 03 25 evaluating the reliability and fid

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/llm-alignment.md|llm-alignment]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/reasoning-integrity.md|reasoning-integrity]]
- [[concepts/adversarial-prompting.md|adversarial-prompting]]
- [[concepts/llm-generated-text-detection.md|llm-generated-text-detection]]

---
_LLM 분석으로 재생성됨_
