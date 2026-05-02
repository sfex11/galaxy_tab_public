# Crab: A Semantics-Aware Checkpoint/Restore Runtime for Agent Sandboxes

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-02
**링크**: http://arxiv.org/abs/2604.28138v1

## 💡 핵심 인사이트

에이전트 샌드박스의 C/R 비효율의 근인은 기술적 한계가 아니라 에이전트가 의미론적으로 의존하는 OS 상태와 전체 OS 스냅샷 사이의 구조적 불일치(에이전트-OS 의미론적 간극)이며, 이 간극을 인식론적으로 좁히는 것이 재시도 비용 폭주와 상태 불일치를 동시에 해결한다.

## 📖 분석

# Crab: Semantics-Aware Checkpoint/Restore for Agent Sandboxes

**카테고리**: 에이전트 인프라 / 상태 관리
**생성일**: 2026-05-02

## 정의

Crab은 에이전트 샌드박스(컨테이너·마이크로VM)의 체크포인트/복원(C/R)에서 발생하는 **에이전트-OS 의미론적 간극**을 식별하고, 이를 해소하는 의미론 인식 런타임이다. 기존 접근이 애플리케이션 수준 복원(OS 부작용 누락)과 전체 턴별 체크포인팅(밀집 배치 하에서 과비용)의 두 극단에 머물던 것을, 에이전트가 의미론적으로 의존하는 OS 상태의 부분집합만 선택적으로 캡처함으로써 중간 지점을 찾는다.

## 기존 Wiki와의 관계

### retry-context-accumulation-loop에 대한 구조적 대안
기존에 재시도 시 컨텍스트가 누적되어 비용이 기하급수적으로 폭주하는 문제를 '누적을 피하는 것'이 아닌 '클린 체크포인트로 복원하는 것'으로 해결하는 경로를 제공한다. 재시도-컨텍스트 누적 루프가 토큰 수준의 회피 전략이라면, Crab은 상태 수준의 근본 해결책이다.

### algorithm-system-translation-gap의 구체적 사례
에이전트의 의미론적 요구(어떤 파일·프로세스·아티팩트에 의존하는가)와 OS의 체크포인트 메커니즘(전체 상태 스냅샷) 사이의 번역 간극을 실제 런타임 문제로 구체화한다.

### sandbox-liveworld-gap의 인프라적 해법
샌드박스 내 상태가 라이브 환경과 다르게 동작하는 문제를, C/R의 정확성을 높임으로써 샌드박스-실세계 갭을 좁히는 하위 인프라로 기능한다.

## 관련 논문

- [[sources/2026-05-02-crab-a-semantics-aware-checkpoint-restore-runtime.md|Crab: A Semantics-Aware Checkpoint/Restore Runtime for Agent Sandboxes]]

## 🔗 관련 논문

- 2026 04 30 agentic harness engineering observability driven a
- 2026 05 01 clawgym a scalable framework for building effectiv
- 2026 04 30 pythia toward predictability driven agent native l

## 🏷️ 엔티티

- [[entities/crab.md|crab]]
- [[entities/semantics-aware-checkpoint.md|semantics-aware-checkpoint]]
- [[entities/sandbox-liveworld-gap.md|sandbox-liveworld-gap]]
- [[entities/retry-context-accumulation-loop.md|retry-context-accumulation-loop]]
- [[entities/algorithm-system-translation-gap.md|algorithm-system-translation-gap]]
- [[entities/agentic-harness-engineering.md|agentic-harness-engineering]]
- [[entities/clawgym.md|clawgym]]
- [[entities/stateless-architecture-vulnerability.md|stateless-architecture-vulnerability]]

## 📐 개념

- [[concepts/semantics-aware-checkpoint.md|semantics-aware-checkpoint]]
- [[concepts/agent-os-semantic-gap.md|agent-os-semantic-gap]]
- [[concepts/selective-state-capture.md|selective-state-capture]]
- [[concepts/checkpoint-restore-efficiency-spectrum.md|checkpoint-restore-efficiency-spectrum]]
- [[concepts/agent-sandbox-state-management.md|agent-sandbox-state-management]]

---
_LLM 분석으로 생성됨_
