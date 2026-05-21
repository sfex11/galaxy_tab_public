# A Methodology for Selecting and Composing Runtime Architecture Patterns for Production LLM Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-21
**링크**: http://arxiv.org/abs/2605.20173v1

## 💡 핵심 인사이트

에이전트 런타임의 핵심 설계 결함은 '코드를 써서 실행하지 말고, 확률적 출력과 결정론적 실행 사이의 경계를 4요소 계약(SDB)로 명시적으로 규정하라'이다. 기존 문제들이 algorithm-system-translation-gap, agent-os-semantic-gap, algorithm-system-boundary-collapse 등으로 분절적으로 다루던 경계 문제를 SDB 계약 하나로 통합하여 구조적 해법을 제공한다.

## 📖 분석

# Stochastic-Deterministic Boundary (SDB)

**카테고리**: 에이전트 아키텍처 / 런타임 시스템
**생성일**: 2026-05-21

## 정의
Production LLM 에이전트의 확률적 모델 출력을 결정론적 소프트웨어 시스템으로 변환하는 경계를 4요소 계약(proposer, verifier, commit step, reject signal)으로 정식화한 구조. 이 경계를 에이전트 런타임의 "하중력 분산(load-bearing primitive)"으로 취급하며, 일반 함수 호출이 소프트웨어에서 어떻게 작동하는지처럼 SDB가 에이전트 런타임에서 어떻게 작동해야 하는지를 규정한다.

## 4요소 계약

1. **Proposer**: LLM이 생성한 확률적 출력 후보를 제시
2. **Verifier**: 결정론적 실행이 가능한지 검증 (형식, 타입, 권한 등)
3. **Commit step**: 검증 통과 시 확률적 출력을 결정론적 상태로 변환하는 연산
4. **Reject signal**: 검증 실패 시 되돌리 또는 재생성을 트리거

## SDB를 하중력 분산으로 취급하는 근거
에이전트 런타임은 "LLM이 토큰을 생성한다"는 설명으로는 부족하다. 실제 운영에서는 LLM 출력이 (a) 직접 실행 불가능한 자연어, (b) 파싱/인코딩/검증을 거쳐야 하는 중간 형태, (c) 시스템 API 호출로 변환되어야 하는 세 가지 중 하나의 상태를 거친다. SDB는 이 변환 경계를 명시적 계약으로 규정함으로써, 런타임 내부의 "의미 없는 번역"을 구조화한다.

## 반패턴: 비중재된 번역 (Unmediated Translation)
SDB가 없이 LLM 출력을 직접 시스템에 전달하는 것은 일반 소프트웨어에서 `eval()` 호출이 아닌 `exec(raw_string)`을 수행하는 것과 동등하다. 이는 [[algorithm-system-translation-gap]]을 현현시키는 가장 흔한 형태의 결함이다.

## 관련 논문
- sources/2026-05-21-a-methodology-for-selecting-and-composing-runtime-architecture-patterns-for-production-ll.md

---
# algorithm-system-translation-gap

**카테고리**: 에이전트 아키텍처
**생성일**: 2026-05-01

## 정의
_Wiki 축적 중_

## 관련 논문
- sources/2026-05-01-unifying-sparse-attention-with-hierarchical-memory.md
### A Methodology for Selecting and Composing Runtime Architecture Patterns for Production LLM Ag (2026-05-21)

SDB(확률적-결정론적 경계)는 이 간극을 정식화된 4요소 계약으로 구조화한다. 기존 연구들이 간극의 존재를 진단만 했다면, 본 논문은 그 간극을 '어떻게 교차하는가'라는 구조적 설계 문제로 전환한다. SDB 계약이 충족되면, 알고리즘 층과 시스템 층 사이의 번역이 하드코딩되어 검증 가능한 엔지니어링이 된다.

---
# agent-os-semantic-gap

**카테준**: 에이전트 런타임
**생성일**: 2026-05-02

## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-05-02-crab-a-semantics-aware-checkpointrestore-runtime-f.md
### A Methodology for Selecting and Composing Runtime Architecture Patterns for Production LLM Ag (2026-2026-05-21)
SDB 계약은 OS가 에이전트의 의미론적 의존을 이해하는 데 필요한 인터페이스를 제공한다. OS 런타임이 SDB의 4요소 계약을 인식하면, 단순한 프로세스 스냅샷이 아닌 의미론적 경계에서의 선택적 캡처가 가능해진다. Crab의 의미론 인식 C/R은 SDB의 commit 단계에서의 의미론을 보존하는 구체적 구현이다.

---
# agentic-harness-engineering

**카테고리**: 에이전트 아키텍처
**생성일**: 2026-05-02

## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-05-02-crab-a-semantics-aware-checkpointrestore-runtime-fn.md
### A Methodology for Selecting and Composing Runtime Architecture Patterns for Production LLM Ag (2026-2026-05-21)
SDB는 하네스 엔지니어링이 다루는 '하네스가 에이전트의 행동을 어떻게 제약하는가'를 명시적 계약으로 규명한다. 하네스가 SDB 계약을 준수하면, 하네스-모델 결합 시스템의 안전성과 검증 가능성이 계약 수준으로 보장됨을 수 있다.

---
# algorithm-system-boundary-collapse

**카테고리**: 에이전트 아키텍처
**생성일**: 2026-05-20

## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-05-20-code-as-agent-harness.md
### A Methodology for Selecting and Composing Runtime Architecture Patterns for Production LLM Agents (2026-05-21)
코드 생성이 스스로 실행 인프라의 역할을 모호하게 흡수하려는 '경계 소멸'을 SDB가 명시적으로 거부한다. SDB 계약에 따르면 코드는 반드시 Proposer-Verifier 패턴의 입력이 되어야 하며, 직접 실행 권한을 가질 수 없다. 이 논문은 경계 소멸을 방지하는 구조적 방어물로 SDB를 위치시킨다.

---
# agent-execution-semantic-opacity

**카테고리**: 에이전트 런타임
**생성일**: 2026-05-02

## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-05-02-crab-a-semantics-aware-checkpointrestore-runtime-fn.md
### A Methodology for Selecting and Composing Runtime Architecture Patterns for Production LLM Agents (2026-2026-05-21)
SDB가 존재하지 않으면 에이전트 실행의 의미론이 OS 수준에서 포착 불가능하다. SDB 계약의 Verifier와 Commit 단계가 의미론적 투명성을 제공하므로, 경계 전환 시 "무엇이 의미론적으로 보존되었는가"를 검증 가능하게 된다.

---
# semantic-dependency-graph

**카테고리**: 에이전트 런타임
**생성일**: 2026-05-02

## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-05-02-crab-a-semantics-aware-checkpointrestore-runtime-fn.md
### A Methodology for Selecting and Composing Runtime Architecture Patterns for Production LLM Agents (2026-2026-05-21)
SDB의 Commit 단계는 의미론적 의존 그래프의 특정 절단을 '결정론적 스냅샷'으로 고정하는 연산이다. 이를 통해 의미론적 의존 그래프가 semantic-dependency-snapshot-mismatch 문제를 해결하는 구체적 경로를 제공한다.

---
# semantic-dependency-snapshot-mismatch
**카테고리**: 에이전트 런타임
**생성일**: 2026-05-20

## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-05-20-code-as-agent-harness.md
### A Methodology for Selecting and Composing Runtime Architecture for Production LLM Agents (2026-05-21)
SDB의 Commit 단계가 의미론적 의존 그래프의 정확한 스냅샷을 보장함으로써, 기존에 문서 중심적 인프라가 가진 '의미론적 의존-스냅샷 불일치' 문제를 해결한다. 전체 스냅샷이 아닌 의미론적 경계에서의 선택적 증분 스냅샷을 가능하게 한다.

---
# dynamic-translation-layer
**카테고리**: 에이전트 런타임
**생성일**: 2026-05-20

## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-05-20-code-as-agent-harness.md
### A Methodology for Selecting and Composing Runtime Architecture Patterns for Production LLM Agents (2026-05-21)
SDB는 동적 번역 계층을 구조화된 계약으로 구현한다. 기존 개념이 '동적 번역 계층이 필요하다'는 직관에 머무는 설계에서, SDB는 그 계층이 무엇을 의미하는지(Proposer/Verifier/Commit/Reject)를 명시하고 각 계층이 어떤 시스템 상태와 결합되어야 하는지를 규명한다.

---
# code-as-agent-harness

**카테고리**: 에이전트 아키텍처
**생성일**: 2026-05-20

## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-05-20-code-as-agent-harness.md
### A Methodology for Selecting and Composing Runtime Architecture Patterns for Production LLM Agents (2026-05-21)
SDB 관점에서 code-as-agent-harness를 재평가한다. 코드는 SDB의 Proposer 출력에 대한 하나의 가능한 구현이지만, SDB 계약이 없으면 코드가 직접 실행 권한을 가지는 경계 소멸의 위험을 갖는다. SDB 계약 아래에서 코드는 "결정론적 실행을 위한 제약 기반 스크립트"로 재위치된다.

---
# checkpoint-restore-efficiency-spectrum
**카테고리**: 에이전트 런타임
**생성일**: 2026-05-02

## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-05-02-crab-a-semantics-aware-checkpointrestore-runtime-fn.md
### A Methodology for Selecting and Composing Runtime Architecture Patterns for Production LLM Agents (2026-06-21)
SDB의 Commit 단계는 C/R 스펙트럼 내에서 가장 의미 있는 캡처 지점이 된다. SDB가 명시하는 경계에서만 C/R이 의미를 보존하면, 불필요한 전체 스냅샷 비용을 피하고 O(1) 복원 상한을 실질적으로 달성할 수 있다.

---
# crab

**카테고리**: 에이전트 런타임
**생성일**: 2026-05-02

## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-05-02-crab-a-semantics-aware-checkpointrestore-runtime-fn.md
### A Methodology for Selecting and Composing Runtime Architecture Patterns for Production LLM Agents (2026-06-21)
Crab은 SDB 계약의 Commit 단계에 해당하는 의미론 인식 C/R의 구체적 구현이다. SDB가 제공하는 '의미론적 경계에서의 선택적 증분 스냅샷' 메커니즘을 Crab이 실제 런타임에서 구현한다. SDB 계약 없이 Crab이 작동하면 의미론이 보존되지 않는 체크포인트가 생성된다.

---
# process-control-architecture

**카테고리**: 에이전트 아키텍처
**생성일**: 2026-03-22

## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-03-22-box-maze-a-process-control-architecture-for-reliab.md
### A Methodology for Selecting and Composing Runtime Architecture Patterns for Production LLM Agents (2026-06-21)
SDB는 프로세스 제어 아키텍처를 확률적-결정론 경계로 확장한다. Box Maze가 토큰 수준 제어에서 프로세스 무결성을 강제했다면, SDB는 경계 수준에서 시스템 무결성을 강제한다. 두 계층은 상보완적이다: Box Maze의 토큰 내부 무결성이 SDB의 경계 수준 무결성의 전제가 된다.

---
# reversible-sft

**카테고리**: 학습 / 학습 후
**생성일**: 2026-05-10

## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-05-10-crafting-reversible-sft-behaviors-in-large-languag.md
### A Methodology for Selecting and Composing Runtime Architecture Patterns for Production LLM Agents (2026-06-21)
SDB의 Commit 단계는 SFT로 학습된 행동을 '동결'시키는 메커니즘이다. SFT 동안에는 확률적 변이 허용되지만, SDB를 통과한 결정론적 고정은 그 변이를 확률적 분포에 매못시킨다(reversible). 즉 SDB가 없으면 복원 불가능한 행동이 SDB가 있으면 복원 가능한 행동이 된다.

---
# sources/2026-05-21-a-methodology-for-selecting-and-composing-runtime-architecture-patterns-for-production-ll.md

**카테고리**: 에이전트 아키텍처 / 런타임 시스템
**생성일**: 2026-05-21

## 핵심
Production LLM 에이전트가 확률적 모델 출력과 결정론적 소프트웨어 시스템 사이의 경계를 **확률적-결정론적 경계(Stochastic-Deterministic Boundary, SDB)**라 명명하고, 이를 4요소 계약(Proposer, Verifier, Commit, Reject)으로 정식화한다. SDB는 에이전트 런타임의 "하중력 분산(load-bearing primitive)"으로, 일반 함수 호출이 소프트웨어에서 작동하는 방식으로 에이전트 런타임에서도 작동해야 한다고 주장한다.

## 4요소 계약
SDB는 다음 네 부분으로 구성된다:

1. **Proposer**: LLM이 생성한 확률적 출력 후보를 시스템에 제안
2. **Verifier**: 제안된 후보가 결정론적 실행이 가능한지 검증 (형식, 타입, 권한 등)
3. **Commit step**: 검증 통과 시 확률적 출력을 결정론적 상태로 변환하는 연산
4. **Reject signal**: 검증 실패 시 되돌리 또는 재생성을 트리거

## 하중력 분산 근거
에이전트 런타임은 "LLM이 토큰을 생성한다"는 설명으로는 부족하다. 실제 운영에서는 LLM 출력이 직접 실행 불가능한 자연어이며, 시스템 API 호출로 변환되어야 하는 세 가지 상태를 거친다. SDB는 이 변환 경계를 명시적 계약으로 규정함으로써, 런타임 내부의 "의미 없는 번역"을 구조화한다.

## 반패턴: 비중재된 번역 (Unmediated Translation)
SDB가 없이 LLM 출력을 직접 시스템에 전달하는 것은 일반 소프트웨어에서 `eval(raw_string)`을 직접 실행하는 것과 동등하다. 이는 [[algorithm-system-translation-gap]]을 현현시키는 가장 흔한 형태의 결함이며, algorithm-system-boundary-collapse을 유발한다.

## 기존 연구와의 관계
### [[algorithm-system-translation-gap]]
SDB(확률적-결론적 경계)는 이 간극을 정식화된 4요소 계약으로 구조화한다. 기존 연구들이 간극의 존재를 진단만 했다면, 본 논문은 그 간극을 '어떻게 교차하는가'라는 구조적 설계 문제로 전환한다.

### [[agent-os-semantic-gap]]
SDB 계약이 OS가 에이전트의 의미론적 의존을 이해하는 데 필요한 인터페이스를 제공한다.

### [[agentic-harness-engineering]]
SDB 계약이 하네스가 에이전트의 행동을 어떻게 제약하는가를 명시적 계약으로 규명한다.

### [[algorithm-system-boundary-collapse]]
코드 생성이 스스로 실행 인프라의 역할을 모호하게 흡수하려는 '경계 소멸'을 SDB가 명시적으로 거부한다.
### [[code-as-agent-harness]]
코드는 SDB의 Proposer 출력에 대한 하나의 가능한 구현이지만, SDB 계약이 없으면 직접 실행 권한을 가지는 경계 소멸의 위험을 간는다.
### [[agent-execution-semantic-opacity]]
SDB가 존재하지 않으면 에이전트 실행의 의미론이 OS 수준에서 포착 불가능하다.
### [[semantic-dependency-graph]]
SDB의 Commit 단계는 의미론적 의존 그래프의 특정 절단을 '결정론적 스냅샷'으로 고정한다.
### [[semantic-dependency-snapshot-mismatch]]
SDB의 Commit 단계가 의미론적 의존 그래프의 정확한 스냅샷을 보장함으로써 기존 문제를 해결한다.
### [[crab]]
Crab은 SDB의 Commit 단계에 해당하는 의미론 인식 C/R의 구체적 구현이다.
### [[process-control-architecture]]
SDB는 프로세스 제어 아키텍처를 확률적-결정론 경계로 확장한다.
### [[reversible-sft]]
SDB의 Commit 단계는 SFT로 학습된 행동을 '동결'시키는 메커니즘이다.
### [[checkpoint-restore-efficiency-spectrum]]
SDB의 Commit 단계에서만 의미 있는 C/R이 가능하다.

## 핵심
Production LLM 에이전트에서 "코드를 쓰고 그대로 실행한다"는 관행에서 "LLM이 계획을 세우고 SDB 계약에 따라 검증-확정을 거쳐 실행한다"로 패러다임을 전환해야 한다. SDB가 명시적 계약이 되면, 하네스 설계가 에이전트-OS 번역의 구조적 무결성을 기계적으로 검증 가능해진다.

## 🏷️ 엔티티

- [[entities/stochastic-deterministic-boundary.md|stochastic-deterministic-boundary]]
- [[entities/sdb-contract.md|sdb-contract]]

## 📐 개념

- [[concepts/mediated-translation-principle.md|mediated-translation-principle]]

---
_LLM 분석으로 생성됨_
