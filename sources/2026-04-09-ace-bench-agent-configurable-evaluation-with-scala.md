# ACE-Bench: Agent Configurable Evaluation with Scalable Horizons and Controllable Difficulty under Lightweight Environments

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-09
**링크**: http://arxiv.org/abs/2604.06111v1

## 💡 핵심 인사이트

에이전트 벤치마크의 난이도와 호라이즌을 독립적으로 제어 가능하게 함으로써, 기존 집계 점수의 신뢰성 문제를 해결하고 에이전트 능력의 체계적 분리 측정을 가능케 한다.

## 📖 분석

## ACE-Bench: Agent Configurable Evaluation with Scalable Horizons and Controllable Difficulty under Lightweight Environments

기존 에이전트 벤치마크들이 가진 두 가지 핵심 한계를 해결하기 위한 새로운 평가 프레임워크다. 첫째, 환경 상호작용 오버헤드가 전체 평가 시간의 최대 41%를 차지하는 문제, 둘째, 태스크 호라이즌과 난이도 분포의 불균형으로 인해 집계 점수가 신뢰할 수 없는 문제를 다룬다.

ACE-Bench는 통합된 그리드 기반 계획 태스크를 중심으로 구축되며, 에이전트가 부분적으로 완성된 스케줄의 숨겨진 슬롯을 로컬 슬롯 제약조건과 글로벌 제약조건 하에서 채워야 한다. 핵심 기여는 세분화된 난이도 제어와 확장 가능한 호라이즌을 경량 환경에서 제공한다는 점이다.

이 연구는 LLM 에이전트 평가의 방법론적 발전을 대표한다. 기존 벤치마크들(ClawBench, HippoCamp, TraceSafe 등)이 특정 도메인에 초점을 맞추는 반면, ACE-Bench는 도메인 독립적이고 구성 가능한 평가를 지향한다. 특히 태스크 호라이즌과 난이도를 독립적으로 조절할 수 있어, 에이전트의 장기 계획 능력과 제약 만족 능력을 체계적으로 분리하여 측정할 수 있다.

경량 환경 설계는 대규모 에이전트 평가의 실용성 문제를 직접 해결하며, 이는 Batched Contextual Reinforcement에서 다룬 토큰 효율성 및 스케일링 법칙 연구와 상호보완적이다. 또한 Box Maze의 프로세스 제어 아키텍처 연구와 유사하게 구조화된 제약 하에서의 LLM 추론 능력을 평가한다는 공통점이 있다.

## 🔗 관련 논문

- 2026 04 11 clawbench can ai agents complete everyday online t
- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 05 batched contextual reinforcement a task scaling la
- 2026 03 22 box maze a process control architecture for reliab
- 2026 04 03 hippocamp benchmarking contextual agents on person
- 2026 04 11 act wisely cultivating meta cognitive tool use in

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/closed-loop-evaluation.md|closed-loop-evaluation]]
- [[concepts/ai-decision-making.md|ai-decision-making]]
- [[concepts/scaling-laws.md|scaling-laws]]
- [[concepts/tool-use.md|tool-use]]

---
_LLM 분석으로 재생성됨_
