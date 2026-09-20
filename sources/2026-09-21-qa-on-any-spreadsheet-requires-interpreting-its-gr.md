# Q&A on Any Spreadsheet Requires Interpreting Its Grid Structure

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-21
**링크**: http://arxiv.org/abs/2609.20732v1

## 💡 핵심 인사이트

구조 주석의 이득은 검색이 아닌 생성 계층에서 발현되며, 스프레드시트의 연속적 2차원 관계는 어떤 이산 청킹으로도 완전 포착할 수 없는 경질 천장을 형성한다.

## 📖 분석

스프레드시트 QA를 셀 역할 주석 기반 구조 인식 청킹으로 접근한다. 스프레드시트를 평면 텍스트가 아닌 2차원 격자 구조로 이해하고, 각 셀의 역할(헤더·데이터·집계 등)을 주석화하여 해석 가능한 청크로 분할하는 프레임워크를 제안하고 SOTA를 달성한다.

핵심 발견은 셋이다. 첫째, 의미론적 셀 주석은 검색 정확도가 아닌 답변 생성을 개선한다([[generation-not-retrieval-gain]]) — 구조 정보가 효과를 발휘하는 지점은 리트리버의 매칭이 아니라 LLM이 컨텍스트를 소비하는 계층이다. 둘째, SOTA를 넘어서도 경질 천장에 봉착하는데, 원인은 스프레드시트가 연속적 관계와 무한한 셀 조합을 가진 2차원 비정형 데이터라는 존재론적 성질이다([[continuous-structure-discretization-ceiling]]) — 어떤 청킹도 연속 관계의 이산화 손실을 회피할 수 없다. 이는 [[algorithm-system-translation-gap]]의 데이터 도메인 발현으로, 2차원 관계 구조의 선형 청크 강제 직렬화가 만드는 구조적 손실이다. 셋째, [[text-to-sql]] 계열(TeCoD)과 입출력 양단의 대비를 형성한다 — TeCoD가 반복 질의를 출력 측 제약 디코딩으로 다루었다면 본 논문은 임의 질의를 입력 측 구조 인식 청킹([[structure-grounded-chunking]])으로 공략하며, 구조화 데이터 이해의 병목이 쿼리 생성 능력이 아닌 입력 표현 설계에 있을 수 있음을 시사한다. 셀 역할 주석은 검색 매체로서의 경량 도메인 스키마이기도 하다.

## 🔗 관련 논문

- Reliable Answers for Recurring Questions: Boosting Text-to-SQL Accuracy
- RAFT: A Stateful Retrieval-Augmented Framework for Troubleshooting Agents
- Semantic Action Graph: A Shared Representation for Agent Grounding

## 🏷️ 엔티티

- [[entities/spreadsheet-grid-structure.md|spreadsheet-grid-structure]]
- [[entities/semantic-cell-annotation.md|semantic-cell-annotation]]
- [[entities/structure-grounded-chunking.md|structure-grounded-chunking]]
- [[entities/generation-not-retrieval-gain.md|generation-not-retrieval-gain]]
- [[entities/continuous-structure-discretization-ceiling.md|continuous-structure-discretization-ceiling]]
- [[entities/text-to-sql.md|text-to-sql]]
- [[entities/algorithm-system-translation-gap.md|algorithm-system-translation-gap]]
- [[entities/lightweight-domain-schema.md|lightweight-domain-schema]]

## 📐 개념

- [[concepts/structure-grounded-chunking.md|structure-grounded-chunking]]
- [[concepts/generation-not-retrieval-gain.md|generation-not-retrieval-gain]]
- [[concepts/continuous-structure-discretization-ceiling.md|continuous-structure-discretization-ceiling]]
- [[concepts/semantic-cell-annotation.md|semantic-cell-annotation]]
- [[concepts/spreadsheet-grid-structure.md|spreadsheet-grid-structure]]

---
_LLM 분석으로 생성됨_
