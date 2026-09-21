# retrieval-augmented-generation

**카테고리**: 미분류
**생성일**: 2026-04-24

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-04-24-automatic-ontology-construction-using-llms-as-an-e.md|Automatic Ontology Construction Using LLMs as an External La]]

### HealthNLP_Retrievers at ArchEHR-QA 2026: Cascaded LLM Pipeline for Gro (2026-05-01)

일반적 지식 검색 RAG를 넘어 EHR 문서에 대한 근거 추적성(evidence traceability)이라는 도메인 특화 제약을 부과함으로써, RAG의 충실도 문제를 임상 설정에서 구체적으로 문제화한다.

### Superintelligent Retrieval Agent: The Next Frontier of Information Ret (2026-05-10)

기존 RAG가 검색 충실도 문제로 다루어지던 맥락을 넘어, 에이전트의 검색 활용 패턴 자체(탐색적 vs. 전문가적)가 RAG 성능의 결정적 변수임을 구체화한다. 특히 검색 라운드 축소가 레이턴시와 토큰 비용에 미치는 영향을 명시하여 RAG를 파이프라인 서빙 최적화의 관점에서 재문제화한다.

### Measurement-Driven Sub-Network Selection for On-Premise Retrieval-Augm (2026-09-04)

검색 그라운딩 적응이 모델 크기에 따른 품질 격차를 축소하는 평탄화 효과를 실증하여, RAG를 단순 지식 주입이 아닌 '모델 규모 간 능력 등화 메커니즘'으로 재해석한다.

### Does Your Agent's Memory Survive a Model Upgrade? A Controlled Study o (2026-09-08)

청킹+임베딩 파이프라인의 숨은 결합 의존성을 드러낸다. 검색 인덱스가 생성 시점의 임베딩 모델 버전에 결합되어 버전 혼재 시 검색이 구조적으로 깨진다는 것은, RAG를 상태 없는 조회 시스템이 아니라 모델 교체에 취약한 상태저장 시스템으로 재분류한다.

### ReCite: Agentic Reasoning for Faithful Citation (2026-09-10)

RAG 아키텍처가 존재하지 않는 참조의 조작은 대체로 해소했으나 실존 문헌의 잘못된 귀속 문제는 남긴다는 한계 정밀화를 제공한다. 검색 성공(문헌 존재성)과 인용 성공(주장 지지성)의 분리라는 새로운 평가 축을 도입한다.

### MeClear: Cooperative Game-Theoretic Attribution and Risk-Aware Memory  (2026-09-10)

RAG의 semantic similarity 중심 검색이 downstream utility와 무관함을 실증하며, 검색 이후 정리(clearance)라는 상류 개입 계층을 제안한다. 검색-정리 이중 축으로 RAG 파이프라인 설계가 재구성된다.

### RAFT: A Stateful Retrieval-Augmented Framework for Troubleshooting Age (2026-09-19)

RAG의 '정적 문서 = 지식 단위' 전제가 다단계 상태 프로세스인 트러블슈팅 케이스에서 구조적으로 불충분함을 실증한다. 지식 표현이 시간적·상태적 구조를 보존해야 한다는 stateful RAG 방향을 제시하여 RAG 설계 공간에 '검색 단위의 상태성'이라는 새 축을 추가한다.

### Q&A on Any Spreadsheet Requires Interpreting Its Grid Structure (2026-09-19)

구조 인지 청킹이 RAG의 검색이 아닌 생성 계층을 개선함을 실증한다. 청킹 전략의 평가 축에 '해석 가능성에 의한 컨텍스트 풍부화'를 추가하고, 검색 정확도와 하류 답변 품질이 직교할 수 있음을 보여준다.

### RAFT: A Stateful Retrieval-Augmented Framework for Troubleshooting Age (2026-09-21)

RAG의 정적 문서 검색 전제를 붕괴시키는 사례로, 검색 대상의 상태성이 검색 프레임워크 설계 자체를 바꾸어야 함을 시사한다.

→ [[sources/2026-09-21-raft-a-stateful-retrieval-augmented-framework-for-.md|상세 보기]]

### An Interpretable Memory Decision Controller for LLM Agents Based on Th (2026-09-22)

RAG의 맹목 주입 문제에 대한 결정적 진단을 제공한다 — 충돌 메모리 환경에서 RAG의 환각률이 메모리-free 기준선보다 높다는 역설적 실증으로, 검색 품질 최적화만으로는 RAG 신뢰성이 담보되지 않으며 검색 후 신뢰 조정 계층이 필수임을 보여준다.

→ [[sources/2026-09-22-an-interpretable-memory-decision-controller-for-ll.md|상세 보기]]
