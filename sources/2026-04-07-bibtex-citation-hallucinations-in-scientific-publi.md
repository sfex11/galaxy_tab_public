# BibTeX Citation Hallucinations in Scientific Publishing Agents: Evaluation and Mitigation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-07
**링크**: http://arxiv.org/abs/2604.03159v1

## 💡 핵심 인사이트

웹 검색이 통합된 LLM 에이전트도 BibTeX 인용에서 광범위한 필드 수준 hallucination을 보이며, 인용 빈도가 낮거나 최신 논문일수록 오류율이 증가하여 파라메트릭 메모리와 검색 의존도의 상호작용이 핵심 변수임을 밝혔다.

## 📖 분석

## BibTeX Citation Hallucinations in Scientific Publishing Agents: Evaluation and Mitigation

웹 검색 기능을 갖춘 LLM 기반 과학 출판 에이전트가 BibTeX 인용 항목에서 광범위한 필드 수준 오류(hallucination)를 생성하는 문제를 체계적으로 평가한 연구이다. 기존 평가들은 검색 기능 없는 기본 모델만 테스트했으나, 본 연구는 실제 사용 패턴을 반영하여 웹 검색이 통합된 환경에서 평가를 수행했다.

4개 과학 분야에 걸쳐 931편의 논문으로 벤치마크를 구축했으며, 인용 빈도에 따라 인기 논문(popular), 저인용 논문(low-citation), 최신 논문(post-cutoff) 세 가지 티어로 구분했다. 이는 모델의 파라메트릭 메모리와 검색 의존도를 분리하여 분석하기 위한 설계이다. 버전 인식(version-aware) 기반 ground truth를 활용하여 정밀한 평가를 가능하게 했다.

이 연구는 LLM 에이전트의 신뢰성 문제를 인용 생성이라는 구체적 태스크에서 드러낸다. 검색 증강(RAG) 기능이 있어도 hallucination이 지속된다는 점은 retrieval-augmented-generation 연구의 한계를 보여주는 중요한 사례이다. 또한 과학 출판 워크플로우에서 LLM 에이전트의 실질적 배포 시 발생하는 문제를 다루며, LLM 벤치마크 설계 방법론에도 기여한다. 인용 티어별 분석은 모델의 학습 데이터 분포와 검색 능력 간의 상호작용을 이해하는 데 유용한 프레임워크를 제공한다.

## 🔗 관련 논문

- 2026 04 10 a systematic study of retrieval pipeline design fo
- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 09 paper circle an open source multi agent research d

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/reasoning-integrity.md|reasoning-integrity]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[concepts/citation-hallucination.md|citation hallucination]]

---
**관련**: [[entities/ast-citation-parsing.md|ast citation parsing]]

---
**관련**: [[concepts/citation-verifiability-gap.md|citation verifiability gap]]

---
**관련**: [[concepts/citation-claim-decoupling.md|citation claim decoupling]]

---
**관련**: [[concepts/sft-hallucination-mechanism.md|sft hallucination mechanism]]
