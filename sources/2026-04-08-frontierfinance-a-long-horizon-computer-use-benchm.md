# FrontierFinance: A Long-Horizon Computer-Use Benchmark of Real-World Financial Tasks

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-08
**링크**: http://arxiv.org/abs/2604.05912v1

## 💡 핵심 인사이트

금융 도메인에서 LLM 에이전트의 실무 역량을 장기 호라이즌 컴퓨터 사용 태스크로 평가하는 최초의 벤치마크로, 기존 금융 추론 벤치마크(FinTradeBench)를 단순 QA에서 다단계 실무 수행으로 확장한다.

## 📖 분석

## FrontierFinance: A Long-Horizon Computer-Use Benchmark of Real-World Financial Tasks

FrontierFinance는 금융 분야의 실무 전문성을 측정하기 위한 장기 호라이즌(long-horizon) 컴퓨터 사용 벤치마크이다. AI 기반 노동 대체에 대한 우려가 지식 집약 산업에서 심화되는 가운데, 기존 벤치마크들이 실제 전문가 수준의 업무 수행 능력을 적절히 평가하지 못한다는 문제의식에서 출발한다.

### 핵심 특징
- **실무 기반 평가**: 금융 분야의 실제 업무 태스크를 기반으로 LLM 에이전트의 컴퓨터 사용 능력을 장기 호라이즌으로 평가
- **AI 노출 위험 정량화**: 금융이 AI 대체 위험이 높은 도메인으로 식별됨에도 강건한 벤치마크가 부재했던 공백을 메움
- **책임성 메커니즘**: 현재 LLM 배포에서 명확한 책임 소재(accountability) 메커니즘이 부족한 문제를 함께 다룸

### Wiki 연결점
FinTradeBench([[sources/2026-03-22-fintradebench-a-financial-reasoning-benchmark-for-.md|FinTradeBench]])가 금융 추론 능력의 벤치마크였다면, FrontierFinance는 이를 장기 호라이즌 컴퓨터 사용으로 확장한다. 단순 추론을 넘어 실제 도구 사용과 다단계 의사결정을 평가한다는 점에서 차별화된다. ClawBench([[sources/2026-04-11-clawbench-can-ai-agents-complete-everyday-online-t.md|ClawBench]])의 웹 에이전트 평가와도 접점이 있으며, 도메인 특화 컴퓨터 사용 벤치마크라는 방향성을 공유한다. YC-Bench의 장기 계획 평가, The Self Driving Portfolio의 금융 에이전트 아키텍처와도 연결된다. AI 안전성 관점에서는 TraceSafe의 가드레일 평가와 보완적 관계를 형성한다.

## 🔗 관련 논문

- FinTradeBench: A Financial Reasoning Benchmark for LLMs
- ClawBench: Can AI Agents Complete Everyday Online Tasks?
- The Self Driving Portfolio: Agentic Architecture for Institu
- TraceSafe: A Systematic Assessment of LLM Guardrails on Mult
- $\texttt{YC-Bench}$: Benchmarking AI Agents for Long-Term Pl

## 📐 개념

- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/financial-reasoning.md|financial-reasoning]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/web-agent-evaluation.md|web-agent-evaluation]]
- [[concepts/ai-governance.md|ai-governance]]
- [[concepts/closed-loop-evaluation.md|closed-loop-evaluation]]

---
_LLM 분석으로 재생성됨_
