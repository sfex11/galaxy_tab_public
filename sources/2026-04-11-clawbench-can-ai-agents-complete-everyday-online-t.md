# ClawBench: Can AI Agents Complete Everyday Online Tasks?

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-11
**링크**: http://arxiv.org/abs/2604.08523v1

## 💡 핵심 인사이트

AI 에이전트의 실용성을 144개 실제 라이브 플랫폼에서 일상 온라인 작업 수행 능력으로 측정하는 벤치마크를 제시하여, 시뮬레이션 기반 평가의 한계를 넘어 현실 세계 에이전트 성능의 실질적 격차를 드러낸다.

## 📖 분석

## ClawBench: Can AI Agents Complete Everyday Online Tasks?

ClawBench는 일상적인 온라인 작업 153개를 144개 실제 플랫폼에서 15개 카테고리에 걸쳐 평가하는 AI 에이전트 벤치마크 프레임워크다. 구매 완료, 예약, 구직 지원 등 사람들이 실제 생활과 업무에서 반복적으로 수행하는 작업을 대상으로 한다.

### 기존 Wiki와의 관계
- **[[claw-eval]]**과 동일한 'Claw' 계열 프로젝트로, CLAW-Eval이 자율 웹 에이전트의 신뢰성 평가에 초점을 맞췄다면, ClawBench는 실제 라이브 플랫폼에서의 과제 완수 능력을 측정하는 데 집중한다.
- **[[llm-agent]]** 엔티티의 핵심 평가 도구로, 에이전트가 도구 사용(tool-use)과 웹 인터페이스 조작을 통해 end-to-end 작업을 완료할 수 있는지를 검증한다.
- **FrontierFinance** 벤치마크가 금융 도메인 컴퓨터 사용을 평가한다면, ClawBench는 범용 일상 온라인 작업으로 범위를 확장한다.

### 주요 특징
- 144개 실제 라이브 웹사이트를 활용하여 정적 시뮬레이션이 아닌 동적 환경에서 평가
- 15개 카테고리를 통한 포괄적 일상 업무 커버리지
- **Gym-Anything**, **ACE-Bench**, **Android Coach** 등 에이전트 환경/평가 연구의 흐름과 맥을 같이하며, 특히 웹 기반 에이전트의 실용성 검증에 기여

## 🔗 관련 논문

- 2026 04 09 claw eval toward trustworthy evaluation of autonom
- 2026 04 08 frontierfinance a long horizon computer use benchm
- 2026 04 09 ace bench agent configurable evaluation with scala
- 2026 04 09 gym anything turn any software into an agent envir
- 2026 04 10 android coach improve online agentic training effi
- 2026 04 09 maestro adapting guis and guiding navigation with
- 2026 04 10 tracesafe a systematic assessment of llm guardrail

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/web-agent-evaluation.md|web-agent-evaluation]]

---
_LLM 분석으로 생성됨_
