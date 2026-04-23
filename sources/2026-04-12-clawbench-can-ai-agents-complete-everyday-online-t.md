# ClawBench: Can AI Agents Complete Everyday Online Tasks?

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-12
**링크**: http://arxiv.org/abs/2604.08523v1

## 💡 핵심 인사이트

실제 라이브 웹 플랫폼 144개에서 일상 태스크 153개를 평가함으로써, AI 에이전트의 현실 세계 범용성을 체계적으로 측정하는 프레임워크를 제시한다.

## 📖 분석

## ClawBench: Can AI Agents Complete Everyday Online Tasks?

ClawBench는 일상적인 온라인 작업 수행 능력을 평가하기 위한 AI 에이전트 벤치마크 프레임워크이다. 153개의 간단한 태스크를 144개의 실제 라이브 플랫폼에서 15개 카테고리(구매, 예약, 구직 지원 등)에 걸쳐 평가한다.

### 핵심 특징
- **실제 웹 환경 기반**: 기존 시뮬레이션 환경이 아닌 실제 라이브 웹사이트에서 에이전트를 테스트하여 현실적인 평가를 제공
- **일상 태스크 중심**: 이메일 자동화를 넘어 구매, 예약, 지원서 제출 등 실생활에서 반복적으로 수행하는 작업을 대상으로 함
- **다양한 플랫폼 커버리지**: 144개 플랫폼 × 15개 카테고리로 에이전트의 범용성을 측정

### 기존 연구와의 관계
ClawBench는 [[concepts/web-agent-evaluation.md|web agent evaluation]] 분야의 핵심 벤치마크로, 기존의 ClawBench 초기 버전(2026-04-11)을 확장한 것으로 보인다. [[concepts/computer-use-agent.md|computer use agent]] 개념과 직접 연관되며, Android Coach의 온라인 에이전트 학습 효율화 연구([[sources/2026-04-10-android-coach-improve-online-agentic-training-effi.md]])와 상호보완적이다. TraceSafe의 LLM 가드레일 평가([[sources/2026-04-10-tracesafe-a-systematic-assessment-of-llm-guardrail.md]])는 이러한 실제 환경 에이전트의 안전성 측면을 다루며, Comparing Human Oversight Strategies([[sources/2026-04-08-comparing-human-oversight-strategies-for-computer-.md]])는 에이전트 감독 전략을 제시한다. [[entities/llm-agent.md|llm agent]] 엔티티의 실용적 평가 사례로서, [[concepts/closed-loop-evaluation.md|closed loop evaluation]] 및 [[concepts/tool-use.md|tool use]] 개념과도 밀접하게 연결된다.

## 🔗 관련 논문

- 2026 04 11 clawbench can ai agents complete everyday online t
- 2026 04 10 android coach improve online agentic training effi
- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 08 comparing human oversight strategies for computer 
- 2026 04 11 act wisely cultivating meta cognitive tool use in 

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/web-agent-evaluation.md|web-agent-evaluation]]
- [[concepts/computer-use-agent.md|computer-use-agent]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/closed-loop-evaluation.md|closed-loop-evaluation]]
- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/ai-safety.md|ai-safety]]

---
_LLM 분석으로 생성됨_
