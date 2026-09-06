# Translation as a Decision Space: A Multi-Agent Perspective on Low-Resource Dialect Generation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-06
**링크**: http://arxiv.org/abs/2609.04048v1

## 💡 핵심 인사이트

NMT의 단일 출력 관행은 다수의 언어학적으로 유효한 번역 경로를 은폐하며, 번역을 다중 에이전트가 탐색하는 구조화된 결정 공간으로 재정의하면 저자원 방언에서 진정성·레지스터·구조 안정성이라는 다차원 유효성을 분리 평가할 수 있다.

## 📖 분석

# Translation as a Decision Space: A Multi-Agent Perspective on Low-Resource Dialect Generation (2026-09-06)

## 핵심 주장

NMT가 입력당 단일 출력을 산출하는 관행은 다국어 디코딩 내부에 암묵적으로 존재하는 **대안적 결정 궤적**들을 은폐한다. 저자원 방언에서는 어휘 진정성(lexical authenticity)·레지스터(register)·구조적 안정성이 상이한 다수의 언어학적으로 유효한 실현이 공존하므로, 이 불투명성이 특히 치명적이다. 본 논문은 번역을 자율 번역 에이전트들이 탐색하는 **구조화된 결정 공간**으로 재정의한다.

## 기존 Wiki와의 관계

- **[[concepts/evaluator-assumption.md|evaluator assumption]]**: '입력당 정답은 하나'라는 관행은 평가자 가정의 번역 도메인 사례이며, 유효 실현의 다원성을 체계적으로 은폐한다.
- **[[concepts/geometric-collapse.md|geometric collapse]]**: 단일 출력 산출은 다중 유효 모드 중 하나로의 수렴이라는 점에서 모드 붕괴 문제의 번역 버전이다.
- **[[concepts/agent-environment-generation.md|agent environment generation]]**: 태스크(번역)가 자체적으로 탐색 가능한 환경(결정 공간)을 구성하는 사례로, 환경 생성의 대상이 외부 소프트웨어에서 태스크 내부 구조로 확장됨을 보여준다.
- **[[entities/discourse-aware-translation.md|discourse aware translation]]**: DiscoSign의 담화 인지 축과 본 논문의 대안 탐색 축이 병렬을 이루어, 번역 연구가 문장 수준 정적 매핑에서 맥락·대안을 아우르는 동적 과제로 확장되는 흐름을 강화한다.
- **[[concepts/multi-agent-system.md|multi agent system]]**: 에이전트를 협력 조율 대상이 아닌 결정 공간의 분담 탐색자로 활용하는 새로운 응용을 제시한다.

## 연구 지형적 의미

정적 단일 참조 평가의 한계를 노출한다는 점에서 [[concepts/dynamic-benchmark.md|dynamic benchmark]]·[[concepts/self-play-benchmark.md|self play benchmark]] 계열과 합류하며, 번역을 '함수 평가'에서 '공간 탐색'으로 전환한다.

## 🔗 관련 논문

- DiscoSign: Discourse-Aware Text to Sign Language Gloss Trans
- Escaping Mode Collapse in LLM Generation via Geometric Regulation

## 🏷️ 엔티티

- [[entities/translation-decision-space.md|translation-decision-space]]
- [[entities/low-resource-dialect-generation.md|low-resource-dialect-generation]]
- [[entities/multi-agent-system.md|multi-agent-system]]
- [[entities/machine-translation.md|machine-translation]]
- [[entities/discourse-aware-translation.md|discourse-aware-translation]]
- [[entities/agent-environment-generation.md|agent-environment-generation]]
- [[entities/evaluator-assumption.md|evaluator-assumption]]
- [[entities/geometric-collapse.md|geometric-collapse]]
- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/single-output-opacity.md|single-output-opacity]]
- [[concepts/alternative-decision-trajectory.md|alternative-decision-trajectory]]
- [[concepts/multi-dimensional-translation-validity.md|multi-dimensional-translation-validity]]

---
_LLM 분석으로 생성됨_
