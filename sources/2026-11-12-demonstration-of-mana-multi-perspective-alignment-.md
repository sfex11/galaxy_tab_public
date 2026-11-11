# Demonstration of MANA: Multi-perspective Alignment of NPC Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-12
**링크**: http://arxiv.org/abs/2611.14431v1

## 💡 핵심 인사이트

MANA는 시연이 외부 기록 자료가 아니라 에이전트 자신의 시점에서 수행되는 'POV 공유 체화 시연'을 통해, 시연→명세→행동의 번역 계층 없이 시연이 행동 정책으로 직접 증류되는 저작 경로를 제시한다.

## 📖 분석

MANA는 NPC 행동을 체화된 시연(embodied demonstration)으로 정렬하는 인터랙티브 저작 방식으로, Minecraft에서 개발자가 게임을 플레이하며 임의 캐릭터의 시점(POV)으로 동적으로 전환해 이동·대화를 그 자리에서 시연하는 시스템이다. 각 시연은 즉시 distill되어 NPC 행동으로 정렬되며, 게임 캐릭터가 시연의 표현 수용자이자 실행 주체가 된다. 기존 Wiki의 시연 연구 계보와 대비되는 핵심은 'POV 스위칭'이다 — 시연자가 외부 관찰자(레코딩된 인간)가 아니라 에이전트 자신의 지각 채널에 직접 주입되어 시연이 원천과 동일한 관찰 분포 위에서 이루어진다. 이는 demonstration-as-context(시연을 컨텍스트로 주입하는 경로)와 demonstration-as-specification(시연을 명세로 컴파일하는 경로) 사이의 제3 극점을 제공한다: 시연이 별도 명세로 번역되지 않고 캐릭터의 행동 정책 자체로 직접 증류된다. 또한 in-situ 시연은 시뮬레이터를 공유 실험 기판(substrate-as-interface)으로 삼아, 개발자-캐릭터 간 표현 계약이 관찰 채널 일치를 통해 최소화됨을 보여준다. 자연스러운 후속 질문은 이 직접 증류 경로가 실행 계층 감사(demonstration-to-code-compilation의 코드 저작물)와 어떻게 결합되는가다.

## 🔗 관련 논문

- 2026-09-26-rapid-robot-agentic-programming-from-demonstration
- 2026-09-18-in-context-robot-learning-with-vlm-agents
- 2026-09-11-show-harness-just-a-vlm-agent-can-play-robots

## 🏷️ 엔티티

- [[entities/demonstration-as-specification.md|demonstration-as-specification]]
- [[entities/demonstration-as-context.md|demonstration-as-context]]
- [[entities/agent-identity.md|agent-identity]]
- [[entities/substrate-as-interface.md|substrate-as-interface]]
- [[entities/representation-contract.md|representation-contract]]
- [[entities/demonstration-to-code-compilation.md|demonstration-to-code-compilation]]
- [[entities/authoring-in-environment.md|authoring-in-environment]]

## 📐 개념

- [[concepts/embodied-demonstration-authoring.md|embodied-demonstration-authoring]]
- [[concepts/pov-switching-demonstration.md|pov-switching-demonstration]]
- [[concepts/in-situ-alignment.md|in-situ-alignment]]
- [[concepts/demonstration-to-policy-distillation.md|demonstration-to-policy-distillation]]

---
_LLM 분석으로 생성됨_
