# RAFT: A Stateful Retrieval-Augmented Framework for Troubleshooting Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-19
**링크**: http://arxiv.org/abs/2609.20754v1

## 💡 핵심 인사이트

지식의 검색 단위는 지식 자체의 구조적 실재(상태 프로세스 vs 정적 문서)를 반영해야 하며, 검색 단위-지식 구조의 불일치가 검색 품질의 구조적 상한을 결정한다.

## 📖 분석

RAFT는 엔터프라이즈 트러블슈팅 에이전트를 위한 상태 기반(stateful) RAG 프레임워크로, 폐쇄된 지원 케이스를 정적 문서가 아닌 타임라인 엔트리의 유향 체인(directed chain)으로 추상화하고 엔트리 수준에서 검색을 수행한다.

핵심 통찰은 **검색 단위가 지식의 구조적 실재를 반영해야 한다**는 것이다. 다단계 상태 프로세스인 케이스를 문서로 취급하는 기존 RAG는 [[schema-conflation-fallacy]]의 검색 도메인 발현이며, 이 단위-구조 불일치가 검색 품질의 구조적 상한을 결정한다.

Wiki 연결점:
- [[terminal-universe]]가 궤적을 학습 환경으로 재질화했다면, RAFT는 폐쇄 케이스(궤적)를 검색 지식으로 재질화하여 궤적 재활용 원리의 검색 축을 연다.
- [[retrieval-as-black-box]] 논의에 '검색 단위의 구조적 정합성' 차원을 추가한다.
- [[temporal-state-dependency]]가 평가 환경의 시점 간 연결성을 다뤘다면, RAFT는 동일 문제를 검색 지식 표현으로 이동시킨다.
- [[experience-reuse]]의 소비 스펙트럼(스킬·환경·코칭 신호)에 '상태 체인 검색 지식'이라는 제4 경로를 추가한다.

[[superintelligent-retrieval-agent]]가 제시한 검색 프론티어의 구체적 구현 방향이며, [[expert-prior-retrieval]]의 선험 검색을 현재 상태 조건부 엔트리 검색으로 정교화한다. 검색 개선의 병목이 쿼리 전략이 아닌 지식 표현 단위 설계에 있을 수 있음을 시사한다.

## 🔗 관련 논문

- Where Should a Document Live: Context Representation

## 🏷️ 엔티티

- [[entities/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[entities/retrieval-as-black-box.md|retrieval-as-black-box]]
- [[entities/superintelligent-retrieval-agent.md|superintelligent-retrieval-agent]]
- [[entities/terminal-universe.md|terminal-universe]]
- [[entities/experience-reuse.md|experience-reuse]]
- [[entities/schema-conflation-fallacy.md|schema-conflation-fallacy]]
- [[entities/temporal-state-dependency.md|temporal-state-dependency]]
- [[entities/expert-prior-retrieval.md|expert-prior-retrieval]]
- [[entities/stateful-retrieval.md|stateful-retrieval]]

## 📐 개념

- [[concepts/entry-level-retrieval.md|entry-level-retrieval]]
- [[concepts/timeline-entry-chain.md|timeline-entry-chain]]
- [[concepts/document-trajectory-conflation.md|document-trajectory-conflation]]

---
_LLM 분석으로 생성됨_
