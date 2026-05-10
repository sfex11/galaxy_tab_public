# MASPO: Joint Prompt Optimization for LLM-based Multi-Agent Systems

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-10
**링크**: http://arxiv.org/abs/2605.06623v1

## 💡 핵심 인사이트

다중 에이전트 시스템에서 프롬프트 최적화는 개별 에이전트의 독립적 최적화로는 달성 불가능하며, 에이전트 간 상호작용을 고려한 공동 최적화가 시스템 수준 성능의 필수 조건이다.

## 📖 분석

## MASPO: 다중 에이전트 프롬프트의 공동 최적화

MASPO는 LLM 기반 다중 에이전트 시스템(MAS)에서 에이전트 간 프롬프트를 개별적으로가 아닌 **공동으로(jointly)** 최적화하는 프레임워크이다. 기존 MAS 연구가 각 에이전트의 역할 프롬프트를 수동으로 설계하거나 독립적으로 최적화하는 데 머물렀다면, MASPO는 에이전트 간 상호작용을 고려한 반복적 자동 최적화를 제안한다.

### 지역-전역 정렬 간극의 구체적 해법
이 논문의 핵심 기여는 [[concepts/capability-cooperation-paradox|능력-협력 역설]]이 기술하는 '개별 최적 ≠ 시스템 최적' 문제를 프롬프트 최적화 차원에서 구체화한다는 점이다. 각 에이전트의 지역적 목표(local objective)가 시스템 전체의 전역적 목표(holistic system goal)와 정렬되지 않는 **지역-전역 정렬 간극(local-global alignment gap)**을 문제로 명시하고, 이를 반복적 최적화 루프로 해소한다.

### 기존 Wiki와의 연결
- [[entities/agora-opt|Agora-Opt]]가 메모리 증강 토론에서 다중 에이전트 합의를 통해 인식론적 다원주의를 달성했다면, MASPO는 프롬프트 설계 단계에서부터 에이전트 간 정렬을 보장하는 상보적 경로를 제공한다.
- [[entities/nonzero-interaction-guided-exploration|NonZero]]가 에이전트 간 상호작용 구조를 잠재 표현으로 포착하여 탐색에 활용했다면, MASPO는 상호작용 구조를 프롬프트 의미론 차원에서 직접 조작한다.
- [[concepts/emergent-defection|창발적 비협력]]이 개별 안전 규칙 준수에도 불구하고 시스템 수준 실패가 창발하는 현상을 진단했다면, MASPO는 프롬프트 수준의 예방적 정렬을 통해 이 창발성을 원천에서 억제한다.

### 알고리즘-시스템 번역 간극의 프롬프트 차원 현현
[[entities/algorithm-system-translation-gap|algorithm-system-translation-gap]]이 '개별 에이전트 알고리즘의 의도를 시스템 수준 행동으로 번역할 때 발생하는 구조적 정보 손실'로 정의된다면, MASPO의 공동 프롬프트 최적화는 이 번역 간극을 프롬프트 설계 단계에서 부분적으로 흡수하는 구조적 메커니즘이다.

## 🔗 관련 논문

- 2026-04-30-from-soliloquy-to-agora-memory-enhanced-llm-agents.md
- 2026-05-05-nonzero-interaction-guided-exploration-for-multi-a.md
- 2026-04-26-learning-to-communicate-toward-end-to-end-optimiza.md
- 2026-04-30-recursive-multi-agent-systems.md

## 🏷️ 엔티티

- [[entities/maspo.md|maspo]]
- [[entities/multi-agent-system.md|multi-agent-system]]
- [[entities/llm-agent.md|llm-agent]]
- [[entities/prompt-engineering.md|prompt-engineering]]
- [[entities/agora-opt.md|agora-opt]]
- [[entities/nonzero-interaction-guided-exploration.md|nonzero-interaction-guided-exploration]]

## 📐 개념

- [[concepts/local-global-alignment-gap.md|local-global-alignment-gap]]
- [[concepts/joint-prompt-optimization.md|joint-prompt-optimization]]
- [[concepts/cross-agent-prompt-coordination.md|cross-agent-prompt-coordination]]

---
_LLM 분석으로 생성됨_
