# Agent Explorative Policy Optimization for Multimodal Agentic Reasoning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-29
**링크**: http://arxiv.org/abs/2605.28774v1

## 💡 핵심 인사이트

이 논문이 '탐색-흡수 분리'이라는 RL의 근본 가정을 에이전트 RL의 실제 작동에서 반증하여, '생각-행동 분리'라는 새로운 해법을 제시합니다. 이 해법은 표준 RL이 에이전트의 두 행동 체제를 동일한 최적화 문제로 취급한다는 것뿐만 아니라, 에이전트 능력 확장의 근본적 장애를 구조적으로 해소한다는 점에서 특히 GRPO가 에이전트 RL에서 가장 광범위하게 발생하는 실패 모드의 원인을 규명합니다.

## 📖 분석

# thinking-acting-gap

**카테고리**: AI/ML — 에이전트 아키텍처
**생성일**: 2026-05-29

## 정의
다중모달 에이전트 설정에서 LLM의 자체 추론(thinking)과 외부 도구 호출(tool use)이 구조적 비대칭을 보이는 현상. 내부 추론은 자가 충족(self-contained)한 저분산 P(y)에서 작동하며, 도구 호출은 환경 결합적 변동성을 가진 고분산 P(y|tool_use)에서 작동한다. 표준 RL 레시피(GRPO 등)은 이 두 체제를 동일한 최적화 문제로 취급하여, 두 가지 진단적인 실패 모드를 발현시킨다: (1) 도구 호출 보상 신호가 탐색-행동 결합의 노이즈로 오염하여 에이전트가 도구 사용을 회피하게 만들고, (2) 내부 추론 보상이 도구 실행의 변동성에 매몰려 플래토우된다.

## 관련 논문

- sources/2605.28774v1

## 관련 엔티티
- exploration-action-coupling
- exploration-absorption-decoupling
- exploration-avoidance-tradeoff
- reward-hacking
- agent-loop-as-computation
- algorithm-system-translation-gap


## 🏷️ 엔티티

- [[entities/thinking-acting-gap.md|thinking-acting-gap]]
- [[entities/exploration-action-coupling.md|exploration-action-coupling]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-05-29-skill-conditioned-gated-self-distillation-for-llm-]]: 에이전트 강화학습에서 발생하는 구조적 분리 문제(전자는 '생각-행동 분리', 후자는 '탐색-흡수 분리')를 각각 식별하고, 이를 비사후적(non-post-hoc) 방식으로 통합 해결하는 구조적 해법을 제안합니다.
- → [[sources/2026-05-29-self-improving-language-models-with-bidirectional-]]: 에이전트의 탐색 한계를 근원적으로 문제 삼으며, 전자는 기존 RL의 탐색-흡수 분리 가정이 에이전트 설정에서 실패함을 보이고, 후자는 기존 탐색 방법이 확률 분포 경계에 갇히는 한계를 지적합니다.
