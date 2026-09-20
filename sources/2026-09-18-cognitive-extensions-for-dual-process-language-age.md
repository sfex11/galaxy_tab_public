# Cognitive Extensions for Dual-Process Language Agents: Memory and Self-Reflection in Interactive Environments

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-18
**링크**: http://arxiv.org/abs/2609.19128v1

## 💡 핵심 인사이트

대화형 환경의 에이전트 취약성은 모델 전면 재훈련이 아니라 기억(AMM)과 성찰(SRM)이라는 분해된 인지 기능의 모듈형 부착으로 국소 치료 가능하며, 이는 인지 개선의 단위가 모델이 아닌 인지 기능임을 시사한다.

## 📖 분석

대화형 환경에서 언어 에이전트의 취약성 — 장기 상태 추적 실패, 무효 행동 실행, 실패 스텝의 미복구 — 를 SwiftSage 계열 이중 과정(dual-process) 에이전트에 두 개의 모듈형 인지 확장을 부착해 해결한다. AMM(Adaptive Memory Module)은 salience 게이팅으로 에피소딩 기억의 저장을 선별하고 트리거 구동 검색으로 회수하며, SRM(Self-Reflection Module)은 실행 시간 예산 내에서 경계 지어진 검증과 교정 개입을 수행한다.

기존 Wiki와의 관계: ① [[concepts/dual-separated-agent.md|dual separated agent]]의 사고-실행-검증 3계층 분리에 fast/slow 이중 과정 변형을 제공하며, SRM은 외부 검증 계층의 기능을 실행 창 내부의 bounded 검증으로 인라인화한다. ② [[entities/episodic-context.md|episodic context]]·[[entities/persistent-world-model.md|persistent world model]] 계열의 에피소딩 기억 논의에 salience 게이팅이라는 저장 판별 기준을 추가해 [[concepts/internal-cognitive-state-responsive-memory.md|internal cognitive state responsive memory]]의 구체적 실현이 된다. ③ [[concepts/intra-generative-intervention.md|intra generative intervention]]이 규정한 제3 패러다임(실행 중 개입)의 정식 구현으로, [[concepts/retrospective-thinking.md|retrospective thinking]](발화 후 회고)과 구별되는 시간축 지점을 점유한다. ④ [[concepts/harness-side-compensation.md|harness side compensation]] 관점에서 두 모듈은 재훈련 없이 하네스 측에서 인지 실패를 구조적으로 보정하는 조립형 사례다. ⑤ [[concepts/unrecoverable-reasoning-error.md|unrecoverable reasoning error]]의 조기 차단 경로를 제공하고, [[concepts/adaptive-inference.md|adaptive inference]]의 적응 축을 '검증 예산' 차원으로 확장한다.

핵심 통찰: 대화형 취약성의 치료 단위는 모델 전체가 아니라 분해된 인지 기능(기억·성찰)이며, 모듈형 부착이 전면 개선을 대체할 수 있다.

## 🔗 관련 논문

- Remember to be Curious: Episodic Context and Persistent World Model
- RetroThinker: Enabling Retrospective Thinking in Speech LLMs
- Cliff: Learning Process Rewards from the First Mistake
- When LLMs Stop Following Steps: A Diagnostic Study of Procedural Execution

## 🏷️ 엔티티

- [[entities/dual-process-agent.md|dual-process-agent]]
- [[entities/dual-separated-agent.md|dual-separated-agent]]
- [[entities/salience-gated-episodic-memory.md|salience-gated-episodic-memory]]
- [[entities/trigger-driven-retrieval.md|trigger-driven-retrieval]]
- [[entities/bounded-execution-time-validation.md|bounded-execution-time-validation]]
- [[entities/internal-cognitive-state-responsive-memory.md|internal-cognitive-state-responsive-memory]]
- [[entities/episodic-context.md|episodic-context]]
- [[entities/intra-generative-intervention.md|intra-generative-intervention]]
- [[entities/retrospective-thinking.md|retrospective-thinking]]
- [[entities/harness-side-compensation.md|harness-side-compensation]]
- [[entities/unrecoverable-reasoning-error.md|unrecoverable-reasoning-error]]
- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/thought-action-separation.md|thought-action-separation]]

## 📐 개념

- [[concepts/salience-gated-episodic-memory.md|salience-gated-episodic-memory]]
- [[concepts/trigger-driven-retrieval.md|trigger-driven-retrieval]]
- [[concepts/bounded-execution-time-validation.md|bounded-execution-time-validation]]
- [[concepts/modular-cognitive-extension.md|modular-cognitive-extension]]
- [[concepts/thought-action-separation.md|thought-action-separation]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-18-in-context-robot-learning-with-vlm-agents]]: 재훈련 없이 배포 시점 컨텍스트 소비(ICL)와 부착형 기억 모듈(AMM)로 적응을 달성한다는 '컴파일이 아닌 소비·부착' 전략을 공유한다.
- → [[sources/2026-09-17-agentic-societies-need-a-social-harness]]: 에이전트의 한계를 모델 재훈련이 아닌 외부 하네스(사회적)와 모듈 부착(인지적)이라는 시스템 수준 개입으로 치료한다는 입장을 공유한다.

---
**관련**: [[entities/distill-globally-adapt-locally.md|distill globally adapt locally]]

---
**관련**: [[entities/privacy-coordination-tension.md|privacy coordination tension]]

---
**관련**: [[entities/streaming-adaptive-inference.md|streaming adaptive inference]]

---
**관련**: [[entities/trust-aware-adaptive-disclosure.md|trust aware adaptive disclosure]]

---
**관련**: [[entities/perception-cognitive-capacity-mismatch.md|perception cognitive capacity mismatch]]

---
**관련**: [[entities/distributed-cognitive-constitution.md|distributed cognitive constitution]]

---
**관련**: [[entities/adaptive-forgetting-as-function.md|adaptive forgetting as function]]

---
**관련**: [[concepts/adaptive-disagreement-pressure.md|adaptive disagreement pressure]]

---
**관련**: [[concepts/self-emission-adaptive-trigger.md|self emission adaptive trigger]]

---
**관련**: [[concepts/trust-aware-adaptive-disclosure.md|trust aware adaptive disclosure]]

---
**관련**: [[concepts/non-cognitive-oracle.md|non cognitive oracle]]

---
**관련**: [[concepts/maneuver-class-extension.md|maneuver class extension]]
