# 질문 2

 2: "검색만으로는 부족하다 — 기업 AI에 필요한 것은?"
새 논문 "Retrieval Is Not Enough"는 기업 지식 시스템이 '확정 결정/폐기 가설/쟁점/미해결'을 구분하지 못한다고 지적하며 인식론적 인프라(epistemic infrastructure)를 제안한다.
우리 Wiki의 논문들(특히 Governed Memory, PSI, 멀티에이전트 아키텍처)은 이 문제를 어떻게 다루고 있는가?
지식의 '신뢰 등급'이나 '확정 상태'를 추적하는 연구가 있는가?

답변은 한국어로, Wiki 지식을 구체적으로 인용하면서 작성해줘.

## Wiki 답변

## "검색만으로는 부족하다 — 기업 AI에 필요한 것은?"에 대한 Wiki 기반 답변

"Retrieval Is Not Enough"가 제기하는 핵심 문제 — 기업 지식 시스템이 **확정된 결정/폐기된 가설/쟁점/미해결 상태**를 구분하지 못한다는 점 — 에 대해 우리 Wiki의 논문들은 크게 **세 가지 축**에서 접근하고 있습니다.

---

### 1. 구조화된 메모리 거버넌스: 지식의 '상태'를 추적하는 아키텍처

**Governed Memory** ([2026-03-20](wiki/sources/2026-03-20-governed-memory-a-production-architecture-for-mult.md))는 이 문제를 가장 직접적으로 다룹니다. 이 논문은 멀티 에이전트 시스템에서 개별 에이전트 성능보다 **공유 메모리의 거버넌스 아키텍처**가 시스템 신뢰성의 핵심 병목이라고 진단하며, 다섯 가지 구조적 과제를 식별합니다:

- **메모리 사일로**: 에이전트 간 지식이 격리되어 상태 불일치 발생
- **거버넌스 파편화**: 지식의 생성·수정·폐기 규칙이 통일되지 않음
- **품질 저하**: 피드백 루프 없이 메모리가 누적되면 신뢰성 감소

이는 "Retrieval Is Not Enough"가 지적하는 '인식론적 인프라 부재'와 정확히 같은 문제입니다. 단순 검색은 정보를 찾아주지만, 그 정보가 **현재 유효한지, 폐기되었는지, 논쟁 중인지**를 알려주지 않습니다.

---

### 2. 공유 상태 버스(PSI)와 인식론적 마찰: 지식 간 관계와 경계 설정

**PSI: Shared State as the Missing Layer** ([2026-04-12](wiki/sources/2026-04-12-psi-shared-state-as-the-missing-layer-for-coherent.md))는 독립적으로 생성된 AI 모듈들을 **공유 상태 버스**로 연결하는 아키텍처를 제안합니다. 이는 검색(retrieval)을 넘어 **모듈 간 추론과 동기화**를 가능케 하는 인프라로, 지식 조각들이 서로의 맥락을 참조하고 일관성을 유지할 수 있게 합니다.

**Triadic Cognitive Architecture** ([2026-04-02](wiki/sources/2026-04-02-the-triadic-cognitive-architecture-bounding-autono.md))는 더 근본적인 차원에서 **인식론적 마찰(epistemic friction)**이라는 개념을 도입합니다. LLM 에이전트가 '인지적 무중력' 상태에서 무비판적으로 정보를 처리하는 문제를 지적하며, 아키텍처 수준에서 **지식의 경계와 불확실성을 명시적으로 부과**해야 한다고 주장합니다. 이것이 바로 '확정/미확정/쟁점'을 구분하는 구조적 기반입니다.

---

### 3. 신뢰도 추적과 믿음 모델링: 지식의 '확신 수준'을 정량화하는 연구

Wiki에는 지식의 신뢰 등급을 추적하는 연구가 **여러 갈래**로 존재합니다:

| 연구 | 접근 방식 |
|------|----------|
| **Dynamic Belief Graphs** ([2026-03-24](wiki/sources/2026-03-24-learning-dynamic-belief-graphs-for-theory-of-mind-.md)) | 믿음을 정적 상태가 아닌 **시간에 따라 진화하는 동적 그래프**로 모델링. 지식 상태의 변화와 상호의존성을 구조적으로 포착 |
| **Causal Confidence** ([2026-03-25](wiki/sources/2026-03-25-causal-evidence-that-language-models-use-confidenc.md)) | LLM이 내부 신뢰도를 단순 보고가 아닌 **행동 조절의 인과적 신호**로 활용한다는 실험적 증거. 기권(abstention) 등 불확실할 때 멈추는 메커니즘의 기초 |
| **VL-Calibration** ([2026-04-14](wiki/sources/2026-04-14-vl-calibration-decoupled-confidence-calibration-fo.md)) | 지각 실패와 추론 오류를 **분리하여 신뢰도를 보정**. 지식 유형별 차등적 확신 수준 추적의 사례 |
| **MemBoost** ([2026-03-30](wiki/sources/2026-03-30-memboost-a-memory-boosted-framework-for-cost-aware.md)) | **불확실성 기반 에스컬레이션** — 응답의 확신이 낮으면 상위 모델로 위임. 지식의 '미해결' 상태를 운영 수준에서 처리 |

---

### 4. 검증과 책임 추적: 지식의 '결정 이력'을 감사하는 구조

**SCRAT** ([2026-04-07](wiki/sources/2026-04-07-coupled-control-structured-memory-and-verifiable-a.md))는 에이전트의 제어·기억·검증을 **결합 설계**해야 한다고 주장하며, **검증 가능하고 감사 가능한 궤적(verifiable/auditable trajectories)**을 핵심 요소로 제시합니다. 이는 지식이 어떤 과정을 거쳐 '확정'되었는지를 추적하는 메커니즘입니다.

**DAO 거버넌스의 Belief Aggregation** ([2026-03-31](wiki/sources/2026-03-31-binary-decisions-in-daos-accountability-and-belief.md))은 다중 에이전트의 분산 합의에서 **선형 의견 풀과 사후 평가 기반 책임성 메커니즘**을 형식화합니다. 이 프레임워크는 집단적 지식 결정의 신뢰 등급 부여에 직접 적용 가능합니다.

---

### 종합: Wiki가 그리는 '인식론적 인프라'의 윤곽

우리 Wiki의 논문들을 종합하면, "Retrieval Is Not Enough"가 요구하는 인식론적 인프라는 다음 **네 개 계층**으로 구성됩니다:

1. **거버넌스 계층** (Governed Memory): 지식의 생성·수정·폐기 규칙 통일
2. **연결 계층** (PSI): 지식 조각 간 상태 동기화와 교차 참조
3. **신뢰도 계층** (Dynamic Belief Graphs, Confidence Calibration): 각 지식 단위의 확신 수준과 상태(확정/쟁점/미해결) 추적
4. **감사 계층** (SCRAT, DAO Belief Aggregation): 결정 이력의 검증 가능성과 책임 추적

단순 검색(RAG)은 이 중 어느 계층도 제공하지 않습니다. Wiki의 연구들은 각각 다른 각도에서 이 빈 공간을 채우고 있으며, **적응적 망각** (Novel Memory Forgetting, [2026-04-06](wiki/sources/2026-04-06-novel-memory-forgetting-techniques-for-autonomous-.md))까지 고려하면, 지식의 전 생애주기 — 생성→검증→확정→갱신→폐기 — 를 관리하는 프레임워크의 조각들이 이미 축적되어 있습니다.