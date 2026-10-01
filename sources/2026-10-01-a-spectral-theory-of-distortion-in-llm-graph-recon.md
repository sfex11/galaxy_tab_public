# A Spectral Theory of Distortion in LLM Graph Reconstruction: Sharp Bounds and Empirical Characterization

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-01
**링크**: http://arxiv.org/abs/2609.38161v1

## 💡 핵심 인사이트

라플라시안 스펙트럼 간 Wasserstein 거리라는 단일 집계 지표는 에지 순변화와 대칭차 사이에 정확히 브래킷되며, 재구성이 에지를 한 방향으로만 변화시킬 때 두 한계가 일치하여 지표가 에지 카운트 이외의 어떤 정보도 담지 못함을 정밀하게 증명한다.

## 📖 분석

## 그래프 재구성 평가의 스펙트럴 이론

LLM 그래프 재구성 평가가 통상 단일 집계 거리를 보고하는 관행에 대해, 본 논문은 라플라시안 스펙트럼 간 Wasserstein 거리가 두 에지 카운트 — 에지 순변화(하한)와 대칭차(상한) — 를 2/n 계수로 정확히 브래킷함을 증명한다. 브래킷은 sharp하며, 재구성이 에지를 한 방향으로만 변화시킬 때(추가만 또는 삭제만) 양끝이 일치하여 지표가 에지 카운트의 자명한 함수로 퇴화한다.

### 기존 Wiki와의 관계

- [[meaning-insensitive-metric]]·[[average-metric-concealment]]: 단일 지표의 구조적 은폐 비판에 '지표가 언제 의미 없는 상태로 붕괴하는가'의 형식적 조건을 부여한다.
- [[single-surface-signal-insufficiency]]: 왜곡 유형(순추가 vs 재배선) 판별에 단일 스칼라가 원리적으로 불충분함을 sharp bound에서 도출한다.
- [[benchmark-specification-gap]]: 재구성 벤치마크가 측정 대상을 명세하지 않으면 에지 카운트 프록시를 측정하고 있을 수 있음을 정량화한다.
- [[graph-topology-refinement]]·[[event-knowledge-graph]]: LLM 그래프 구축·정제 연구에 '브래킷 성분 분해 보고'라는 방법론적 요구를 제시한다.

### 새 인사이트

측정 지표의 정보량을 상하 한계 간극으로 인증하는 메타-평가 원리 — 간극이 닫히면 지표는 자명해지고, 벌어지면 재배선 왜곡의 존재를 증언한다.

## 🔗 관련 논문

- ARGUS: Role-Aware Event Knowledge Graphs for U.S. Employment-Discrimin
- LLM as Clinical Graph Structure Refiner: Enhancing Represent
- A Multimodal Text- and Graph-Based Approach for Open-Domain Event Extr

## 🏷️ 엔티티

- [[entities/spectral-distortion-bracketing.md|spectral-distortion-bracketing]]
- [[entities/graph-reconstruction-evaluation.md|graph-reconstruction-evaluation]]
- [[entities/meaning-insensitive-metric.md|meaning-insensitive-metric]]
- [[entities/average-metric-concealment.md|average-metric-concealment]]
- [[entities/single-surface-signal-insufficiency.md|single-surface-signal-insufficiency]]
- [[entities/benchmark-specification-gap.md|benchmark-specification-gap]]
- [[entities/graph-topology-refinement.md|graph-topology-refinement]]
- [[entities/event-knowledge-graph.md|event-knowledge-graph]]

## 📐 개념

- [[concepts/spectral-distortion-bracketing.md|spectral-distortion-bracketing]]
- [[concepts/metric-informativeness-gap.md|metric-informativeness-gap]]
- [[concepts/graph-reconstruction-evaluation.md|graph-reconstruction-evaluation]]
- [[concepts/meaning-insensitive-metric.md|meaning-insensitive-metric]]
- [[concepts/average-metric-concealment.md|average-metric-concealment]]
- [[concepts/single-surface-signal-insufficiency.md|single-surface-signal-insufficiency]]
- [[concepts/benchmark-specification-gap.md|benchmark-specification-gap]]

---
_LLM 분석으로 생성됨_
