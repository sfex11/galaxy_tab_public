# DeltaBox: Scaling Stateful AI Agents with Millisecond-Level Sandbox Checkpoint/Rollback

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-25
**링크**: http://arxiv.org/abs/2605.22781v1

## 💡 핵심 인사이트

C/R 레이턴시 병목의 근원이 'OS가 무엇을 저장하는가'가 아니라 '에이전트가 무엇에 의존하는가'에 대한 무지에서 기인한다는 점이다. DeltaBox의 상태 유형 분해는 이 무지를 OS의 용어(파일시스템 diff)에서 에이전트의 용어(의존 그래프 diff)로 전환하는 데카르트적 재프레이밍의 사례를 제공한다.

## 📖 분석

# DeltaBox: Scaling Stateful AI Agents with Millisecond-Level Sandbox Checkpoint/Rollback

## 정의

LLM 기반 에이전트가 테스트타임 트리 탐색이나 강화학습 등 빈번한 상태 탐색을 수행할 때, 샌드박스의 전체 상태(파일시스템, 프로세스 상태, 메모리·컨텍스트 등)를 매번 전체 복제하는 체크포인트/롤백(C/R) 방식은 수백 밀리초에서 수 초까지의 레이턴시를 유발하여 심층 탐색과 대규모 팬아웃을 구조적으로 병목시킨다. DeltaBox는 전체 스냅샷이 아닌 증분형(delta)만 저장·복원하는 방식을 제안하여, C/R 레이턴시를 밀리초 수준으로 절반하는 파이프라인을 구현한다.

## 상태 유형 분해
DeltaBox는 에이전트 샌드박스 상태를 세 가지 유형으로 분해하여 각각에 맞는 증분 정책을 적용한다:

1. **파일시스템 상태**: 변경된 파일만 증분 저장 (fs-level diff)
2. **프로세스 상태**: 프로세스 트리/메모리 맵에서 변경분만 증분 (proc-level diff)
3. **컨텍스트 상태**: 대화 히스토리·프롬프트에서 변경분만 증분 (ctx-level diff)
4. **네트워크 상태**: 소켓 연결 상태 변화만 증분 (net-level diff)
5. **권한 상태**: 권한· capabilities 변경만 증분 (perm-level diff)


이 분해는 OS 수준의 전체 스냅샷이 에이전트의 의미론적 의존 구조를 무시하고 불필요한 I/O를 포함한다는 병목을 정확히 진단한다.

## 관련 논문
- sources/2026-05-25-deltabox-scaling-stateful-ai-agents-with-millisecon.md

## 관련 엔티티
- checkpoint-restore-efficiency-spectrum: 기존 스펙트럼이 전체 스냅샷 기반 C/R과 증분 기반 C/R을 극단의 효율 스펙트럼으로 구조화하여 이 논문의 구체적 메커니즘을 제공한다.
- agent-sandbox-state-management: OS 수준의 전체 스냅샷 기반 C/R이 에이전트 실행의 의미론적 의존 구조(어떤 파일·컨텍스트에 의존하는가)를 무시하는 구조적 한계를 명확히 진단한다.
- agent-os-semantic-gap: OS가 에이전트의 의미론적 의존 그래프를 이해하지 못하여 전체 스냅샷으로 변환할 때 발생하는 의미론 보존 실패의 구체적 사례를 제공한다.
- state-integrity-latency-tradeoff: 전체 스냅샷 기반 C/R이 상태 무결성을 강제할수록 레이턴시가 증가하는 구조적 트레이드오프를, 증분 기반 C/R이 의미론적 최소 상태만 복원하여 레이턴시를 O(Δ)로 상한화하는 방법을 제시한다.

## 🔗 관련 논문

- checkpoint-restore-efficiency-spectrum
- agent-sandbox-state-management
- agent-os-semantic-gap
- state-integrity-latency-tradeoff

## 🏷️ 엔티티

- [[entities/delta-checkpoint-rollback.md|delta-checkpoint-rollback]]
- [[entities/delta-checkpoint-rollback.md|delta-checkpoint-rollback]]

## 📐 개념

- [[concepts/delta-checkpoint-rollback.md|delta-checkpoint-rollback]]

---
_LLM 분석으로 생성됨_
