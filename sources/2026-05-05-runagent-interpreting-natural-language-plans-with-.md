# RunAgent: Interpreting Natural-Language Plans with Constraint-Guided Execution

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-05
**링크**: http://arxiv.org/abs/2605.00798v1

## 💡 핵심 인사이트

LLM 플랜 실행의 비신뢰성은 추론 실패가 아니라 자연어 계획과 프로그래밍적 실행 사이에 실행 의미론의 중간 표현층이 부재하기 때문이며, 제어 구조를 제약 강제 메커니즘으로 재해석한 에이전트 언어가 이 간극을 실용적으로 메운다.

## 📖 분석

# RunAgent: Interpreting Natural-Language Plans with Constraint-Guided Execution

**카테고리**: AI/ML — 에이전트 플랜 실행
**생성일**: 2026-05-05

## 정의
자연어로 작성된 계획을 해석하면서 단계별 실행을 제약(rubrics)과 제어 구조(IF, GOTO, FORALL 등)를 통해 강제하는 다중 에이전트 플랜 실행 플랫폼.

## 기존 Wiki와의 관계

### 자연어-형식언어 번역의 제3경로
기존 [[natural-language-to-formal-language]] 논의가 'NL→LTL 등 형식 명세'의 완전 번역과 '의미론적 번역의 어려움'을 다루었다면, RunAgent는 완전한 형식화가 아닌 **에이전트 언어(agentic language)**라는 중간 표현을 도입한다. 이는 NL의 표현력을 유지하면서 프로그래밍의 결정론성을 부여하는 제3경로로, 기존의 2분법(NL vs 형식언어)을 해체한다.

### 프로세스 제어의 플랜 수준 확장
[[process-control-architecture]]가 Box Maze에서 추론 체인 내부의 무결성을 아키텍처 수준에서 강제했다면, RunAgent는 이를 **플랜 실행 계층**으로 확장한다. 단계별 rubric 검증이 스텝 수준 검증 디코딩([[step-level-verification-decoding]])의 실제 구현 사례가 되며, 제어 구조(IF/GOTO)가 프로세스 제어를 플랜 의미론에 직접 매핑한다.

### 알고리즘-시스템 번역 간극의 중간층 해법
[[algorithm-system-translation-gap]]이 '의미론적 의존 그래프를 OS 메커니즘으로 번역할 때의 비효율'을 문제 삼았다면, RunAgent의 에이전트 언어는 이 번역 간극을 **실행 의미론의 명시적 중간 표현**으로 완화하는 시도다. 제어 구조가 플랜의 의미론을 코드가 아닌 제약으로 인코딩한다.

## 연결점
- [[scientific-workflow-agent]]: 연구 질문→워크플로우 자동화가 '의미론적 번역'에 집중했다면, RunAgent는 번역된 플랜의 **실행 신뢰성**에 집중하여 보완적 축을 형성한다.
- [[sandbox-liveworld-gap]]: 플랜 실행의 결정론성 강화가 샌드박스-실세계 간극을 구조적으로 축소하는 경로를 제공한다.
- [[agentic-harness-engineering]]: 제약과 rubric이 하네스의 핵심 구성요소(실행 제어)를 플랜 언어 수준에서 내재화한다.

## 🔗 관련 논문

- sources/2026-04-26-from-research-question-to-scientific-workflow-leve.md
- sources/2026-03-22-box-maze-a-process-control-architecture-for-reliab.md
- sources/2026-05-02-crab-a-semantics-aware-checkpointrestore-runtime-f.md

## 🏷️ 엔티티

- [[entities/constraint-guided-plan-execution.md|constraint-guided-plan-execution]]
- [[entities/agentic-language.md|agentic-language]]
- [[entities/llm-agent.md|llm-agent]]
- [[entities/natural-language-to-formal-language.md|natural-language-to-formal-language]]
- [[entities/process-control-architecture.md|process-control-architecture]]
- [[entities/algorithm-system-translation-gap.md|algorithm-system-translation-gap]]
- [[entities/scientific-workflow-agent.md|scientific-workflow-agent]]
- [[entities/agentic-harness-engineering.md|agentic-harness-engineering]]

## 📐 개념

- [[concepts/constraint-guided-plan-execution.md|constraint-guided-plan-execution]]
- [[concepts/agentic-language.md|agentic-language]]
- [[concepts/plan-execution-semantics.md|plan-execution-semantics]]
- [[concepts/rubric-based-step-verification.md|rubric-based-step-verification]]
- [[concepts/control-construct-grounding.md|control-construct-grounding]]

---
_LLM 분석으로 생성됨_
