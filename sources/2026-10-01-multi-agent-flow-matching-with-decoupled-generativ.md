# Multi-Agent Flow Matching with Decoupled Generative Guidance

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-01
**링크**: http://arxiv.org/abs/2609.38133v1

## 💡 핵심 인사이트

다중 에이전트 생성에서 조인트 하드 제약은 각 에이전트의 유도 입력 간 순환 의존성을 유발하며, 각 에이전트가 독립적으로 자기 유도를 산출하는 분리형 유도 구조가 이 순환을 끊는 구조적 해법이다.

## 📖 분석

생성 모델의 표현력이 생성물의 하드 제약 만족에 대한 형식적 보장을 수반하지 않는다는 간극을 다중 에이전트 설정으로 확장해 다룬다. 난제는 구조적이다: 조인트 하드 제약이 여러 에이전트에 걸쳐 있어 각 에이전트의 유도(guidance)가 타 에이전트의 유도에 의존하는데, 유도들은 동시에 계산되므로 순환 의존성이 발생한다. 본 논문은 각 에이전트가 타 에이전트의 동시 계산 결과 없이 자기 유도 입력을 결정하는 **분리형 생성 유도(decoupled generative guidance)**로 이 순환을 끊는다.

Wiki 지형에서의 위치: [[compositional-incoherence]]와 [[compositional-safety]]가 '개별 유효성의 합성이 조인트 유효성을 보장하지 않는다'는 진단을 제공했다면, 본 논문은 그 생성 측 쌍대 문제 — 조인트 제약을 만족하는 객체의 분산적 생산 — 를 flow matching 계층에서 공략한다. [[communication-free-coordination]]의 생성 공간 확장으로, 통신 없는 조율 원리가 물리·행동 공간에서 분포 수준 생성으로 이동함을 보여준다. [[flow-matching]]의 위상도 확장된다: Flow-OPD가 flow matching 모델의 증류 훈련이었다면 본 논문은 flow matching을 제약 만족 생성의 프리미티브로 격상시킨다.

## 🔗 관련 논문

- Flow-OPD: On-Policy Distillation for Flow Matching Models

## 🏷️ 엔티티

- [[entities/flow-matching.md|flow-matching]]
- [[entities/multi-agent-system.md|multi-agent-system]]
- [[entities/compositional-incoherence.md|compositional-incoherence]]
- [[entities/communication-free-coordination.md|communication-free-coordination]]
- [[entities/formal-verification.md|formal-verification]]
- [[entities/decoupled-generative-guidance.md|decoupled-generative-guidance]]
- [[entities/joint-hard-constraint-generation.md|joint-hard-constraint-generation]]

## 📐 개념

- [[concepts/decoupled-generative-guidance.md|decoupled-generative-guidance]]
- [[concepts/joint-hard-constraint-generation.md|joint-hard-constraint-generation]]
- [[concepts/generative-guarantee-gap.md|generative-guarantee-gap]]

---
_LLM 분석으로 생성됨_
