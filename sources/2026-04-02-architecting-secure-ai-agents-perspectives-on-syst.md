# Architecting Secure AI Agents: Perspectives on System-Level Defenses Against Indirect Prompt Injection Attacks

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-02
**링크**: http://arxiv.org/abs/2603.30016v1

## 💡 핵심 인사이트

간접 프롬프트 인젝션 방어는 단일 모델 수준이 아닌 에이전트 시스템 아키텍처 전반에 걸친 동적 보안 정책 통합이 필요하며, 컨텍스트 의존적 보안 판단은 런타임에서만 가능하다는 점이 핵심이다.

## 📖 분석

## Architecting Secure AI Agents: Perspectives on System-Level Defenses Against Indirect Prompt Injection Attacks

본 포지션 페이퍼는 LLM 기반 AI 에이전트가 직면하는 **간접 프롬프트 인젝션(indirect prompt injection)** 공격에 대한 시스템 수준 방어 아키텍처를 논의한다. 간접 프롬프트 인젝션은 신뢰할 수 없는 외부 데이터에 악의적 명령이 삽입되어 에이전트가 위험한 행동을 수행하도록 유도하는 공격 방식이다.

저자들은 세 가지 핵심 입장을 제시한다: (1) 동적 환경에서는 **동적 재계획(dynamic replanning)**과 보안 정책의 실시간 갱신이 필수적이며, (2) 특정 **컨텍스트 의존적 보안 판단**은 런타임에서만 내릴 수 있고, (3) 이러한 방어 메커니즘은 에이전트 시스템 아키텍처 전반에 걸쳐 통합되어야 한다.

이 연구는 기존 Wiki의 [[ai-safety]] 개념과 직접적으로 연결되며, 특히 [[TraceSafe|TraceSafe: A Systematic Assessment of LLM Guardrails]]가 다루는 LLM 가드레일 평가와 상호보완적이다. TraceSafe가 기존 가드레일의 효과를 '평가'하는 데 초점을 맞춘다면, 본 논문은 방어 아키텍처를 어떻게 '설계'해야 하는지에 대한 비전을 제시한다. 또한 [[llm-agent]] 엔티티의 보안 측면을 심화하며, [[adversarial-prompting]] 개념의 에이전트 환경 확장판으로 볼 수 있다. [[differential-privacy]]와 함께 LLM 에이전트의 신뢰성 확보를 위한 다층적 보안 프레임워크의 한 축을 형성한다.

## 🔗 관련 논문

- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 03 19 differential privacy in generative ai agents analy
- 2026 04 09 who governs the machine a machine identity governa
- 2026 04 11 act wisely cultivating meta cognitive tool use in

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/adversarial-prompting.md|adversarial-prompting]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/prompt-engineering.md|prompt-engineering]]

---
_LLM 분석으로 재생성됨_
