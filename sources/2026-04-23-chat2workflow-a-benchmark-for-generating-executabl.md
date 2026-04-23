# Chat2Workflow: A Benchmark for Generating Executable Visual Workflows with Natural Language

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-23
**링크**: http://arxiv.org/abs/2604.19667v1

## 💡 핵심 인사이트

LLM의 자연어 이해 능력이 곧 실행 가능한 시각적 워크플로우 생성 능력으로 전이되지 않으며, 두 능력 사이의 갭을 체계적으로 좁히는 것이 워크플로우 자동화의 핵심 과제다.

## 📖 분석

# Chat2Workflow: 자연어로 실행 가능한 시각적 워크플로우 생성 벤치마크

## 정의
실행 가능한 시각적 워크플로우(executable visual workflow)를 자연어 지시로부터 자동 생성하는 LLM의 능력을 평가하기 위해 제안된 벤치마크. 현산업에서 워크플로우 구성이 수동 공학에 의존하는 비용·시간 문제를 LLM으로 해소할 수 있는지를 검증한다.

## 기존 Wiki와의 관계

### LLM Agent 능력 스펙트럼의 확장
기존 [[llm-agent]] 연구가 주로 '주어진 워크플로우를 실행'하는 에이전트에 집중했다면, Chat2Workflow는 **'워크플로우를 생성'**하는 에이전트 역할을 새로 정의한다. 이는 [[aggregate-pipeline-serving]]이 다루는 에이전틱 파이프라인을 LLM이 직접 설계할 수 있는지라는 근본적 질문으로 이어진다.

### 벤치마크 패러다임의 이동
기존 [[llm-benchmark]]가 정답 일치나 LLM-as-Judge에 의존해왔다면, Chat2Workflow는 **실행 가능성(executability)**을 평가의 핵심 축으로 삼는다. 이는 [[closed-loop-evaluation]]이 자율주행에서 도입한 실행 기반 평가 패러다임을 워크플로우 도메인으로 확장하는 것과 같은 맥락이다.

### 컴퓨터 사용 에이전트와의 연결
[[computer-use-agent]]가 GUI를 통해 직접 행동하는 방식과 달리, Chat2Workflow는 시각적 워크플로우라는 **중간 표현(intermediate representation)**을 생성한다. 이는 [[thought-action-separation]]의 변형으로 해석할 수 있다—생성된 워크플로우가 '사고의 외재화'이자 '검증 가능한 실행 계획'이 되기 때문이다.

## 다른 논문과의 연결점
- **ClawBench** (2026-04-13): 에이전트가 온라인 작업을 수행하는 능력을 평가한 반면, Chat2Workflow는 작업 자체를 워크플로우로 설계하는 능력을 평가하여 보완적 관계
- **Scepsy** (2026-04-20): 에이전틱 워크플로우의 서빙을 최적화하는 연구와 결합하면, 생성→서빙의 전체 파이프라인 자동화가 가능
- **ClaWEnvKit** (2026-04-22): 환경 자동 생성과 워크플로우 자동 생성의 결합은 에이전트 개발의 완전 자동화를 향한 단계

## 🔗 관련 논문

- 2026 04 22 clawenvkit automatic environment generation for cl
- 2026 04 20 scepsy serving agentic workflows using aggregate l
- 2026 04 13 clawbench can ai ag
- 2026 04 22 using large language models for embodied planning

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/benchmark.md|benchmark]]
- [[entities/llm.md|llm]]
- [[entities/computer-use-agent.md|computer-use-agent]]

## 📐 개념

- [[concepts/visual-workflow-generation.md|visual-workflow-generation]]
- [[concepts/natural-language-to-executable-pipeline.md|natural-language-to-executable-pipeline]]
- [[concepts/workflow-engineering-automation.md|workflow-engineering-automation]]
- [[concepts/executable-benchmark.md|executable-benchmark]]

---
_LLM 분석으로 생성됨_
