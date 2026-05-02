# Crab: A Semantics-Aware Checkpoint/Restore Runtime for Agent Sandboxes

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-03
**링크**: http://arxiv.org/abs/2604.28138v1

## 💡 핵심 인사이트

에이전트 C/R의 근본적 비효율은 기술적 한계가 아니라 에이전트의 의미론적 의존 모델과 OS의 상태 캡처 모델 사이의 구조적 단절(agent-OS semantic gap)에서 기인하며, 이 간극을 의미론 인식 선택적 직렬화로 좁히는 것이 재시도 비용을 O(1)로 상한화하는 구조적 경로다.

## 📖 분석

# Crab: A Semantics-Aware Checkpoint/Restore Runtime for Agent Sandboxes

## 핵심 기여

Crab은 에이전트 샌드박스에서 체크포인트/복원(C/R)이 직면하는 근본적 간극을 **에이전트-OS 의미론 간극(Agent-OS Semantic Gap)**으로 명시적으로 규정한다. 에이전트는 의미론적 의존 그래프(어떤 상태에 의존하는가)로 추론하지만, OS는 전체 스냅샷으로 상태를 캡처한다. 이 간극이 기존 C/R 접근을 두 극단—애플리케이션 수준 복원(OS 효과 누락)과 턴별 전체 체크포인팅(정확하나 밀집 배치에서 과비용)—으로 분리한 근원이다.

## 기존 Wiki와의 관계

### algorithm-system-translation-gap의 런타임 실현
기존에 이 개념이 추상적 간극으로만 기술되던 것을, Crab이 구체적 런타임 문제로 현현한다: 의미론적 의존 그래프를 OS 체크포인트 메커니즘으로 번역할 때 발생하는 비효율이 간극의 본질이다.

### retry-context-accumulation-loop에 대한 구조적 대안
[[entities/retry-context-accumulation-loop|재시도-컨텍스트 누적 루프]]가 컨텍스트를 누적시켜 비용을 O(n)으로 폭주시킨다면, Crab의 의미론 인식 클린 체크포인트 복원은 재시도 비용을 O(1)로 상한화하는 구조적 대안을 제공한다.

### stateless-architecture-vulnerability의 실용적 중간지점
[[entities/stateless-architecture-vulnerability|상태 없는 아키텍처 취약점]]에 대해 Crab은 완전한 상태 유지가 아닌 의미론적으로 최소한의 상태만 선택적으로 보존하는 상태 없음-상태 유지 사이의 실용적 중간지점을 제시한다.

## 새로운 인사이트

Crab의 의미론 인식 C/R은 단순한 효율화 기법이 아니다. 이는 [[concepts/agent-execution-semantic-opacity|에이전트 실행 의미론 불투명성]]을 실행 환경 계층에서 부분적으로 해소하는 시도다. 에이전트의 논리적 실행 의미론(권한 승계, 제어 흐름 의존성, 도구 호출 인과 사슬)을 OS 수준 스냅샷이 포착하지 못한다는 [[concepts/semantic-system-state-disconnect|상태의 의미론적-시스템적 표현 단절]]을, 의미론적 의존 그래프를 인식하는 C/R 원시 연산으로 좁히는 경로를 연다.

다만, 다중 에이전트 확장 시 [[concepts/cross-agent-checkpoint-consistency|Cross-Agent Checkpoint Consistency]] 문제가 부분 순서 문제로 변형되며, [[concepts/checkpoint-consensus-reduction|Checkpoint Consensus Reduction]]이 요구된다는 한계가 동시에 제기된다.

## 🔗 관련 논문

- 2026-04-30-pythia-toward-predictability-driven-agent-native-l.md
- 2026-05-02-exploration-hacking-can-llms-learn-to-resist-rl-tr.md
- 2026-05-01-clawgym-a-scalable-framework-for-building-effectiv.md
- 2026-05-02-claw-eval-live-a-live-agent-benchmark-for-evolving.md

## 🏷️ 엔티티

- [[entities/crab.md|crab]]
- [[entities/semantics-aware-checkpoint.md|semantics-aware-checkpoint]]
- [[entities/agent-os-semantic-gap.md|agent-os-semantic-gap]]
- [[entities/algorithm-system-translation-gap.md|algorithm-system-translation-gap]]
- [[entities/retry-context-accumulation-loop.md|retry-context-accumulation-loop]]
- [[entities/stateless-architecture-vulnerability.md|stateless-architecture-vulnerability]]
- [[entities/checkpoint-restore-efficiency-spectrum.md|checkpoint-restore-efficiency-spectrum]]
- [[entities/selective-state-capture.md|selective-state-capture]]
- [[entities/agentic-harness-engineering.md|agentic-harness-engineering]]

## 📐 개념

- [[concepts/agent-os-semantic-gap.md|agent-os-semantic-gap]]
- [[concepts/semantic-system-state-disconnect.md|semantic-system-state-disconnect]]
- [[concepts/agent-execution-semantic-opacity.md|agent-execution-semantic-opacity]]
- [[concepts/semantic-cr-primitive.md|semantic-cr-primitive]]
- [[concepts/cross-agent-checkpoint-consistency.md|cross-agent-checkpoint-consistency]]
- [[concepts/checkpoint-consensus-reduction.md|checkpoint-consensus-reduction]]
- [[concepts/semantic-serialization-subordination.md|semantic-serialization-subordination]]
- [[concepts/delegation-boundary-serialization.md|delegation-boundary-serialization]]

---
_LLM 분석으로 생성됨_
