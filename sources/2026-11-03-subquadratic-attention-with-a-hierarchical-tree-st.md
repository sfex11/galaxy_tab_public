# Subquadratic Attention with a Hierarchical Tree-Structured Indexer

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-03
**링크**: http://arxiv.org/abs/2610.42112v1

## 💡 핵심 인사이트

어텐션의 2차 병목 돌파는 표현력 희생(선형·윈도우)이나 상수배 가속(희소)이 아니라, 인덱싱 구조 자체를 계층적 트리로 재설계하여 점근적 subquadratic을 달성하는 데서 나온다.

## 📖 분석

이 논문은 어텐션의 2차 스케일링 병목을 점근적으로 하위 2차(subquadratic) 복잡도로 돌파하는 계층적 트리 구조 인덱서를 제시한다. 기존 접근의 두 한계를 동시에 극복한다: 고정 크기 상태의 슬라이딩 윈도우·선형 어텐션은 표현력을 상실하고([[linear-attention]]), 희소 어텐션 방법은 인덱서 자체가 2차 스케일링하여 상수배 가속에 머문다. 트리 인덱서는 인덱싱 연산 자체를 계층 탐색 구조로 재설계하여 이 딜레마을 해소한다. [[sparse-attention-unification]]이 희소 어텐션과 계층적 메모리를 통합했다면, 본 논문은 그 통합이 지향하던 점근적 목표를 달성하되 계층 구조의 구현 위치를 메모리 조직에서 인덱서의 탐색 구조로 이동시킨다. [[on-demand-attention]]과 상보적이다 — recall head가 '언제 전역 읽기를 할까'를 판단하는 능력 축이라면, 본 논문은 '전역 읽기를 얼마나 싸게 만들까'의 비용 축을 공략하여 지역 우선 디코딩의 경제성 전제를 강화한다.

## 🔗 관련 논문

- Unifying Sparse Attention with Hierarchical Memory for Scalable Long-Context
- On-Demand Attention: Language Models Know When to Recall

## 🏷️ 엔티티

- [[entities/sparse-attention-unification.md|sparse-attention-unification]]
- [[entities/hierarchical-kv-memory.md|hierarchical-kv-memory]]
- [[entities/linear-attention.md|linear-attention]]
- [[entities/on-demand-attention.md|on-demand-attention]]
- [[entities/long-context.md|long-context]]

## 📐 개념

- [[concepts/subquadratic-attention.md|subquadratic-attention]]
- [[concepts/hierarchical-tree-indexer.md|hierarchical-tree-indexer]]
- [[concepts/indexer-quadratic-bottleneck.md|indexer-quadratic-bottleneck]]
- [[concepts/expressiveness-efficiency-dilemma.md|expressiveness-efficiency-dilemma]]

---
_LLM 분석으로 생성됨_
