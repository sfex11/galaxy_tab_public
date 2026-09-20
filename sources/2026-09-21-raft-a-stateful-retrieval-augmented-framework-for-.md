# RAFT: A Stateful Retrieval-Augmented Framework for Troubleshooting Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-21
**링크**: http://arxiv.org/abs/2609.20754v1

## 💡 핵심 인사이트

다단계 절차 지식의 검색 품질 병목은 쿼리 최적화가 아니라 검색 대상의 표현 단위 설계 — 정적 문서가 아닌 상태 조건부 엔트리 체인 — 에 있다.

## 📖 분석

RAFT는 트러블슈팅 에이전트를 위한 상태 저장형 RAG 프레임워크다. 기존 검색 증강 시스템이 지원 사례를 정적 문서로 취급한 것과 달리, 종결된 사례를 타임라인 엔트리의 방향성 체인으로 추상화하고 현재 문제 해결 상태에 조건부로 엔트리 수준 검색을 수행한다.

핵심 진단은 [[document-trajectory-conflation]]이다 — 다단계 절차 지식을 문서로 평탄화하는 것이 검색 품질의 근본 한계이며, 이는 [[algorithm-system-translation-gap]]의 검색 도메인 발현이다. 지식 표현 단위의 선택이 검색 계약의 실질을 결정한다.

[[superintelligent-retrieval-agent]]가 쿼리 생성을 병목으로 지목했다면, RAFT는 병목이 지식 표현 단위 설계에 있을 수 있음을 보이는 상보 축을 제공한다. 검색 개선이 질의 최적화가 아닌 검색어가 노리는 대상의 구조화에서 출발할 수 있음을 실증한다.

[[experience-reuse]] 관점에서 궤적 소비의 제4 경로를 연다 — 과거 사례 궤적이 스킬·환경·코칭 신호 외에 상태 조건부 검색 체인으로 재질화된다. [[timeline-entry-chain]]은 [[procedural-graph]]의 검색 버전으로, 실행 구조의 체인화가 자기 개선이 아닌 지식 재사용에서도 유효함을 보여준다. 또한 검색 조건이 쿼리 텍스트가 아닌 추론 상태가 된다는 점에서 [[reasoning-conditioned-retrieval]]과 [[knowledge-state-orchestration]]을 연결하며, 검색 외부화 논의([[retrieval-as-black-box]])에 '무엇을 검색 단위로 삼을 것인가'라는 표현 계층 질문을 추가한다.

## 🔗 관련 논문

- RAFT: A Stateful Retrieval-Augmented Framework for Troubleshooting Age
- Superintelligent Retrieval Agent: The Next Frontier of Information Ret
- SkillOS: Learning Skill Curation for Self-Evolving Agents
- Procedural Graphs: Self-Evolving Execution Structures for LLM Agents
- Terminal-Universe: Turning Agent Trajectories into Scalable Terminal E
- Learning to Coach for Experiential Learning
- ADEMA: A Knowledge-State Orchestration Architecture for Long

## 🏷️ 엔티티

- [[entities/stateful-retrieval.md|stateful-retrieval]]
- [[entities/timeline-entry-chain.md|timeline-entry-chain]]
- [[entities/document-trajectory-conflation.md|document-trajectory-conflation]]
- [[entities/temporal-state-dependency.md|temporal-state-dependency]]
- [[entities/schema-conflation-fallacy.md|schema-conflation-fallacy]]
- [[entities/superintelligent-retrieval-agent.md|superintelligent-retrieval-agent]]
- [[entities/expert-prior-retrieval.md|expert-prior-retrieval]]
- [[entities/experience-reuse.md|experience-reuse]]
- [[entities/retrieval-as-black-box.md|retrieval-as-black-box]]
- [[entities/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[entities/reasoning-conditioned-retrieval.md|reasoning-conditioned-retrieval]]
- [[entities/knowledge-state-orchestration.md|knowledge-state-orchestration]]

## 📐 개념

- [[concepts/stateful-retrieval.md|stateful-retrieval]]
- [[concepts/timeline-entry-chain.md|timeline-entry-chain]]
- [[concepts/document-trajectory-conflation.md|document-trajectory-conflation]]
- [[concepts/temporal-state-dependency.md|temporal-state-dependency]]
- [[concepts/schema-conflation-fallacy.md|schema-conflation-fallacy]]
- [[concepts/entry-level-retrieval.md|entry-level retrieval]]
- [[concepts/상태-조건부-검색.md|상태 조건부 검색]]

---
_LLM 분석으로 생성됨_
