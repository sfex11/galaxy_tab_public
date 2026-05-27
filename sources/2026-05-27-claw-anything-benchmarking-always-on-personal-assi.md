# Claw-Anything: Benchmarking Always-On Personal Assistants with Broader Access to User's Digital World

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-27
**링크**: http://arxiv.org/abs/2605.26086v1

## 💡 핵심 인사이트

기존 에이전트 평가 체계가 '좁은 사용자 상태'에서만 에이전을 평가하여 '항상 켘 사용자 상태'에서의 성능을 보장하지 못하는 근본적 한계를 구조적으로 드러내며, 에이전의 실제 맥락 환경(전체 디지털 발자국)을 평가 대상으로 편입함으로써 기존 평가 체계의 signal-evaluation-decoupling이 가설이 아닌 실제 환경에서도 검증됨을 보여준다.

## 📖 분석

# Claw-Anything: Always-On Personal Assistants의 범치가 드 넓은 사용자 디지털 세계 접근

기존 에이전트 평가 체계(ClawGym, Claw-Eval-Live)가 에이전트의 동적 도구역(툴 환경, API 호출, 파일 시스템)에서만 성능을 측정한다면, Claw-Anything은 **항상 켜(Always-On) 퍼라널럼**이라는 새로운 평가 차원을 제시한다. '항상 켜' 에이전트는 사용자의 전체 디지털 세계(이메일, 문서, 브라우저, 캘릭더, 메신지 앱 등)를 이해하고 활용할 수 있어야 하며, 기존 벤치마크가 채택한 좁은 사용자 상태로 인한 평가의 근본적 한계를 구조적으로 드러낸다.

## sandbox-liveworld-gap에 대한 구체적 해결
기존 sandbox-liveworld-gap 엔티티는 이 문제를 진단만으로 기술했다면서 Claw-Anything은 그에 대한 **실증적 해결**을 제공한다. 항상 켜 설정에서는 에이전의 실패 모드가 단순한 과제 해결 능력 부족이 아니라 **사용자 맥락 전체를 인지하지 못해 발생**함을 보여준다. 예를 들어, 이메일 맥락에서 3주 전의 결재함을 요청하는 질의에 기존 벤치마크의 정적 답변이 실패하고 사용자가 직접 메모리를 뒤져야 하는 상황이 빈번하며, 문서 편집기가 에이전의 코드 해석과 충돌되는 사례가 관찰된다. Claw-Anything은 사용자의 전체 디지털 발자국(digital footprint)을 구조화하여 좁은 벤치마크가 보지 못하는 정보 축적 문제를 명시적으로 드러낸다.

## live-benchmark의 확장
기존 live-benchmark 엔티티는 시간에 따라 변하는 실시간 태스크를 반영하도록 설계되었으나, 여전히 좁은 사용자 상태를 가정한 채 신호만 갱신한다. Claw-Anything은 **신호 계층의 갱신**을 통해 사용자의 디지털 활동을 실시간으로 반영하며, 평가 대상(에이전의 맥락 전략, 문서 편집 동향 변화 등) 자체가 시간에 따라 변화하는 동적 환경을 추적한다. 이로써 기존 signal-evaluation-decoupling이 신호-평가 갱신을 통해 정적 평가와 동적 환경 평가를 분리하는 구조가 실제 환경에서도 유효하게 작동함을 실증한다.

## 하네스 숨겨 문제의 구체화
harness-as-hidden-variable 엔티티와 연관하여, Claw-Anything은 벤치마크 자체가 에이전이 접근 가능한 사용자 세계의 어느 부분을 규명하지 않음을 보여준다. 좁은 벤치마크의 툴 가용자-도구나 제한된 API 호출 집합이 에이전의 'always-on' 요구조건에 미달하는 사례를 체계적으로 분석한다. 예를 들어, 특정 브라우저가 에이전의 편집기를 방해하려 할 때 에이전이 이전에 생성한 문서를 인용하지 못하는 현상, 또는 파일 시스템의 계층 구조를 이해하지 못해 잘못된 경로로 탐색하는 현상 등은 단순한 능력 문제가 아니라 사용자의 디지털 세계에 대한 **구조적 무지**에서 기인한 실패임을 보여준다.
## 관련 소스
- sources/2026-05-27-claw-anything-benchmarking-always-on-personal-assistants-with-broader-access-to-users-digital-world.md

## 🏷️ 엔티티

- [[entities/sandbox-liveworld-gap.md|sandbox-liveworld-gap]]
- [[entities/live-benchmark.md|live-benchmark]]
- [[entities/harness-as-hidden-variable.md|harness-as-hidden-variable]]
- [[entities/evaluator-assumption.md|evaluator-assumption]]

## 📐 개념

- [[concepts/always-on-assistant.md|always-on-assistant]]
- [[concepts/digital-world-access.md|digital-world-access]]
- [[concepts/user-state-completeness.md|user-state-completeness]]

---
_LLM 분석으로 생성됨_
