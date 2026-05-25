# AwareVLN: Reasoning with Self-awareness for Vision-Language Navigation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-25
**링크**: http://arxiv.org/abs/2605.22816v1

## 💡 핵심 인사이트

VLN에서 SOTA 방법들이 에이전트-지시간-장면 간의 관계를 명시적으로 모델링하지 못하는 근본적 한계를 지적한다. AwareVLN은 에이전트가 자신의 상태(무엇을 보았는가), 위치(지금 어디에 있는가), 지시(무엇이 필요한가)를 명시적으로 모델링하는 삼원적 인지 구조(self-awareness)를 제안하여, 장면 그래프 구성 + 계층적 계획 중 자기 인지 점검(self-awareness check)을 통해 기존 계층적 계획의 한계를 구조적으로 해결한다.

## 📖 분석

## AwareVLN: Reasoning with Self-awareness for Vision-Language Navigation

VLN에서 SOTA 방법들은 VLM의 추론 능력을 end-to-end 행동 예측에 활용하거나 휴리스트 플래닝을 구축하지만, 에이전트-지시간-장면 간의 관계를 명시적으로 모델링하지 못하는 근본적 한계를 지적한다. AwareVLN은 에이전트가 자신의 상태(무엇을 보았는가), 위치(지금 어디에 있는가), 지시(무엇이 필요한가)를 명시적으로 모델링하는 **자기 인지(self-awareness)**를 제안한다. VLM의 장면적 이해 능력을 활용해 장면 그래프를 구성하면서, 계층적 계획 과정에서 자기 인지 점검(self-awareness check)을 삽입하여 기존 계층적 계획의 한계를 해결한다.

### 관련 엔티티
- [[entities/agentic-vlm|agentic-vlm]]: 기존 항목에서 VLN의 단계별 판단과 다단계 경로 이탈이라는 한계를 보완한다. 이 논문은 그 원인이 '자기 인지 부재'에 있음을 구체화한다.
- [[entities/representation-action-gap|representation-action-gap]]: 장면 이해가 행동으로 번역되지 않는 현상의 VLN 실증을 제공한다. 에이전트가 장면을 이해하더라도 자신의 장면 내 위치를 모르지 못하면 행동 결정이 실패한다는 구체적 메커니즘이다.
- [[entities/planning-gap|planning-gap]]: 자기 인지를 계층적 계획에 내재화함으로써, 기존 계층적 계획(Three-Step Nav 등)의 한계를 구조적으로 해소한다.
- entities/observation-fidelity-paradox: 관찰 충실도를 높여도 에이전트-장면 관계가 모델링되지 않으면 충실도가 오히려 저하되는 역설에 대한 VLN 실증을 제공한다.
- [[entities/three-step-nav|three-step-nav]]: 계층적 계획을 사용하지만 자기 인지 점검이 없어 한계에 직면하는 기존 방법과의 한계를 비교 검증한다.
- [[entities/zero-shot-vln|zero-shot-vln]]: 데모stration 없는 제로샷 VLN 설정에서 자기 인지가 특히 중요함을 보여준다.

### 새 엔티티 제안: agent-scene-instruction-triad
VLN에서 에이전트가 (1) 장면에서 무엇을 관찰했는지, (2) 장면 내 자신의 현재 위치를 어디로 인식하는지, (3) 지시가 현재 무엇을 요구하는지를 명시적으로 모델링하는 삼원적 인지 구조. 기존 방법이 블랙박스 추론(단계별 행동 예측)와 정적 맵(정적 맵 구축)의 한계를 동시에 해결하는 접근으로, 에이전트가 자신의 인지적 위치를 상활하고 계획의 유효성을 자가 검증 가능하게 만든다.

### 새 개념 제안: agent-scene-instruction-triad
VLN에서 에이전트가 지시, 장면, 자신의 상태를 삼원적으로 인지하고 이를 기반으로 행동을 계획해야 한다는 구조적 요구. 기존 방법이 에이전트-지시 간 관계를 모델링하지 않아 발생하는 추론-행동 단절의 근원을 해명한다.

## 🏷️ 엔티티

- [[entities/agent-scene-instruction-triad.md|agent-scene-instruction-triad]]

## 📐 개념

- [[concepts/agent-scene-instruction-triad.md|agent-scene-instruction-triad]]

---
_LLM 분석으로 생성됨_
