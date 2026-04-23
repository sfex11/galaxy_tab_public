# SWE-chat: Coding Agent Interactions From Real Users in the Wild

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-24
**링크**: http://arxiv.org/abs/2604.20779v1

## 💡 핵심 인사이트

코딩 에이전트의 실제 가치는 통제된 벤치마크 성능이 아니라 'in the wild'에서 사용자가 에이전트 출력을 얼마나 채택하는지(actual utility)로 결정되며, SWE-chat은 이 실증적 차원을 최초로 대규모로 포착한다.

## 📖 분석

# SWE-chat

**카테고리**: AI/ML — 코딩 에이전트 평가
**생성일**: 2026-04-24

## 정의

SWE-chat은 오픈소스 개발자의 실제 코딩 에이전트 세션을 대규모로 수집한 최초의 생태계 데이터셋으로, 6,000개 세션·63,000여 사용자 프롬프트·355,000건 에이전트 도구 호출을 포함한다. 자동 수집 파이프라인을 통해 지속적으로 확장되는 'living dataset' 구조를 가진다.

## 기존 Wiki와의 관계

### 샌드박스-실세계 격차의 실증적 극복
기존 Wiki에서 ClawBench가 샌드박스 성공률 65-75%가 라이브 환경에서 33.3%로 급락함을 보고한 바 있다. SWE-chat은 이 격차를 메우는 반대 방향의 접근 — 실제 'in the wild' 데이터를 직접 수집하여 평가 기준을 현실에 정렬하는 방식을 제시한다.

### 에이전트 평가 패러다임의 전환
기존 llm-benchmark·web-agent-evaluation이 합성 태스크 중심이었다면, SWE-chat은 '사용자가 실제로 에이전트에게 무엇을 요청하고, 얼마나 유용한 출력을 얻는가'라는 실용성 관점을 도입한다. 이는 LLM-as-Judge의 비일관성 문제를 실증적 기준으로 보완할 수 있는 기반을 제공한다.

### 도구 호출 패턴의 거시적 분석
355,000건의 도구 호출 데이터는 tool-use·blind-tool-invocation 개념에 실증적 근거를 제공할 수 있다. 에이전트가 실제로 어떤 도구를 언제, 어떻게 호출하는지에 대한 패턴 분석은 Act Wisely 등 메타인지적 도구 사용 연구와 직결된다.

## 관련 논문
- [[concepts/vibe-coding.md|vibe coding]]
- [[concepts/action-expert-fine-tuning.md|action expert fine tuning]]
- [[concepts/interaction-awareness.md|interaction awareness]]

- [[sources/2026-04-24-swe-chat-coding-agent-interactions-from-real-use.md|SWE-chat: Coding Agent Interactions From Real Users in the Wild]]

## 🔗 관련 논문

- 2026-04-13-clawbench-can-ai-agents-complete-everyday-online-t.md
- 2026-04-30-beyond-code-snippets-benchmarking-llms-on-reposito.md
- 2026-04-13-act-wisely-cultivating-meta-cognitive-tool-use-in-.md

## 🏷️ 엔티티

- [[entities/swe-chat.md|swe-chat]]
- [[entities/llm-agent.md|llm-agent]]
- [[entities/computer-use-agent.md|computer-use-agent]]
- [[entities/benchmark.md|benchmark]]
- [[entities/repository-level-code-understanding.md|repository-level-code-understanding]]

## 📐 개념

- [[concepts/in-the-wild-agent-dataset.md|in-the-wild-agent-dataset]]
- [[concepts/agent-session-dataset.md|agent-session-dataset]]
- [[concepts/tool-call-utility-analysis.md|tool-call-utility-analysis]]
- [[concepts/living-dataset.md|living-dataset]]

---
_LLM 분석으로 생성됨_
