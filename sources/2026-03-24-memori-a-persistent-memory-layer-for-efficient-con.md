# Memori: A Persistent Memory Layer for Efficient, Context-Aware LLM Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-24
**링크**: http://arxiv.org/abs/2603.19935v1

## 💡 핵심 인사이트

메모리를 LLM 내부 기능이 아닌 독립적 데이터 구조화 문제로 재정의함으로써, 벤더 종속 없이 토큰 효율적인 에이전트 장기 기억을 실현한다.

## 📖 분석

## Memori: LLM 에이전트를 위한 영속적 메모리 레이어

Memori는 LLM 에이전트가 다중 세션에 걸쳐 맥락 인식(context-aware) 행동을 유지할 수 있도록 설계된 **LLM-agnostic 영속적 메모리 레이어**이다. 기존 접근법들이 특정 벤더에 종속(vendor lock-in)되고, 대량의 원시 대화를 프롬프트에 주입하여 토큰 비용 증가와 성능 저하를 유발하는 문제를 해결한다.

### 핵심 설계 철학
Memori는 메모리를 **데이터 구조화 문제(data structuring problem)**로 취급한다. Advanced Augmentation 파이프라인을 통해 원시 대화를 구조화된 메모리로 변환하며, API 레이어에서 작동하여 어떤 LLM과도 호환된다. 이는 프롬프트 엔지니어링이나 모델 내부 수정 없이 에이전트의 장기 기억을 가능하게 한다.

### 기존 연구와의 관계
- **LLM Agent 생태계**: [[llm-agent]] 엔티티와 직접 관련. 에이전트가 자율적으로 작동하려면 세션 간 상태 유지가 필수적이며, Memori는 이 인프라 계층을 제공한다.
- **프롬프트 엔지니어링 효율화**: [[prompt-engineering]] 개념과 연결. 원시 대화 전체를 프롬프트에 넣는 대신 구조화된 메모리를 선택적으로 주입하여 토큰 효율성을 높인다.
- **멀티 에이전트 시스템**: [[multi-agent-system]]에서 에이전트 간 메모리 공유 문제와 연결 가능.
- **ChameleonEpisodicMemory 연구**와 에피소딕 메모리 접근법에서 유사점이 있으나, Memori는 모델 내부가 아닌 API 레이어에서의 외부 메모리에 초점.

### 의의
메모리를 모델 종속적 기능이 아닌 독립적 인프라로 분리함으로써, 에이전트 개발의 모듈성과 이식성을 크게 향상시킨다.

## 🔗 관련 논문

- 2026 04 09 claw eval toward trustworthy evaluation of autonom
- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 09 who governs the machine a machine identity governa
- 2026 04 08 filegram grounding agent personalization in file s

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/prompt-engineering.md|prompt-engineering]]
- [[concepts/long-context.md|long-context]]
- [[concepts/multi-agent-system.md|multi-agent-system]]

---
_LLM 분석으로 재생성됨_
