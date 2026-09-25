# SpeakerMem-R1: Speaker-Centered Dual-Track Memory for Multi-Party Dialogue

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-24
**링크**: http://arxiv.org/abs/2609.26780v1

## 💡 핵심 인사이트

다자 대화 메모리의 병목은 콘텐츠 검색 정확도가 아니라 화자·대상·집단 관계라는 사회 구조의 보존에 있으며, 대화 메모리의 분해 축이 정보 유형(AutoViewMem)에서 사회 관계 구조로 이틀 만에 확장되고 있다.

## 📖 분석

### SpeakerMem-R1: Speaker-Centered Dual-Track Memory for Multi-Party Dialogue (2026-09-24)

다자 대화 장기 메모리의 요구를 5축으로 규정한다 — 누가 말했는가, 누구에 관한 것인가, 개인이 서로를 어떻게 지각하는가, 무엇이 집단에 공유되는가, 상태가 어떻게 변하는가. 범용 LLM 메모리 시스템이 인물·집단 관계를 잃거나 대화 전역에 분산된 단서를 통합하지 못한다는 진단은 [[memory-fragmentation-failure]]의 다자 확장이다 — 단일 화자 가정 위의 요약·벡터 검색이 사회적 속성을 구조적으로 소실시킨다는 병인을 제공한다.

AutoViewMem([[self-configuring-memory-schema]])이 정보 유형별 직교 뷰 분해를 제안한 지 이틀 뒤, 본 논문은 분해 축이 '정보 유형'에서 '사회 관계'로 확장됨을 보인다. 화자 트랙과 콘텐츠 트랙의 분리는 [[dual-trace-encoding]]의 관계적 버전으로, 화자 귀속을 사후 추론이 아닌 저장 계층의 1급 속성으로 격상시킨다. 대인 지각의 저장은 [[theory-of-mind]]가 추론 시점 능력에서 저장 데이터로 이동하는 전환점이며, 집단 공유 정보 추적은 [[collective-belief-formation]]의 메모리 측 구현, 상태 변화 추적은 [[knowledge-state-drift]]의 구조적 관리에 해당한다.

→ sources/2026-09-24-speakermem-r1-speaker-centered-dual-track-mem.md

## 🔗 관련 논문

- AutoViewMem: Self-Configuring Orthogonal Views for Conversat
- ConvMem: Convolutional Memory for Long-Context Reasoning
- An Interpretable Memory Decision Controller for LLM Agents B
- Bayesian Belief Layer for Controllable Opinion Dynamics in L
- LongSeeker: Elastic Context Orchestration for Long-Horizon S
- Rethinking Memory as Continuously Evolving Connectivity

## 🏷️ 엔티티

- [[entities/speakermem-r1.md|speakermem-r1]]
- [[entities/self-configuring-memory-schema.md|self-configuring-memory-schema]]
- [[entities/memory-fragmentation-failure.md|memory-fragmentation-failure]]
- [[entities/orthogonal-memory-views.md|orthogonal-memory-views]]
- [[entities/value-differential-memory-management.md|value-differential-memory-management]]
- [[entities/theory-of-mind.md|theory-of-mind]]
- [[entities/collective-belief-formation.md|collective-belief-formation]]
- [[entities/knowledge-state-drift.md|knowledge-state-drift]]
- [[entities/convmem.md|convmem]]
- [[entities/memory-management.md|memory-management]]

## 📐 개념

- [[concepts/speaker-attributed-memory.md|speaker-attributed-memory]]
- [[concepts/dual-track-memory.md|dual-track-memory]]
- [[concepts/interpersonal-perception-memory.md|interpersonal-perception-memory]]
- [[concepts/group-shared-state-tracking.md|group-shared-state-tracking]]
- [[concepts/orthogonal-memory-views.md|orthogonal-memory-views]]
- [[concepts/dual-trace-encoding.md|dual-trace-encoding]]
- [[concepts/semantic-interference-decoupling.md|semantic-interference-decoupling]]
- [[concepts/memory-representation-spectrum.md|memory-representation-spectrum]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-24-cliffcompaction-cost-efficient-compaction-for-long]]: 무한정 늘어나는 세션·대화 이력을 구조화된 메모리(자동 압축, 화자 중심 분해 트랙)로 이월하는 장기 기억 관리라는 공통 문제를 다룬다.
