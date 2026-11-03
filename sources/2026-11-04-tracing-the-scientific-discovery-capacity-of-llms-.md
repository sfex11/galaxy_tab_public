# Tracing the Scientific Discovery Capacity of LLMs to Their Training Data

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-04
**링크**: http://arxiv.org/abs/2611.03617v1

## 💡 핵심 인사이트

과학적 발견 실패를 모델 내부 한계가 아닌 훈련 데이터의 monofact(단일 노출 사실) 비율이라는 결측 확률 질량으로 설명함으로써, 능력의 원천 귀속이 모델 구조에서 데이터 구성으로 이동하고 데이터 귀속 연구가 출력 수준에서 능력 수준으로 확장된다.

## 📖 분석

본 논문은 LLM의 과학적 발견 능력을 훈련 데이터로 추적하는 문제를 '결측 확률 질량(missing probability mass)'의 문제로 재정식화한다. 핵심 개념은 monofact — 훈련 중 정확히 한 번 관측된 사실 — 이며, 이론적 분석에 따르면 발견 능력의 상한이 훈련 데이터 내 monofact 비율에 의해 설정된다. 재료 과학과 규제 유전체학 도메인에서 monofact 비율을 직접 조작하는 인과 실험으로 이 명제를 검증한다.

Wiki 관점에서 이 논문은 세 축을 확장한다. 첫째, [[data-attribution]] 계열(CATT)이 출력 수준 [[fact-tracing]]을 다뤘다면 본 논문은 귀속 대상을 능력 수준으로 상향한다 — '이 출력이 어느 데이터에서 왔는가'에서 '이 능력이 어떤 데이터 통계에 의해 설정되는가'로. 직접 조작 실험 설계는 [[controlled-variable-attribution-evaluation]]과 [[evaluation-confound-isolation]]의 단일 변수 통제 원리를 훈련 데이터 축으로 이식한 사례다. 둘째, [[fact-memorization]] 연구에 기능적 재해석을 제공한다 — [[digit-level-verbatim-retrieval]](Molecular Déjà Vu)이 희귀 사실의 검색 가능성을 위험으로 다뤘다면, 본 논문은 단일 노출 사실의 부재가 발견 실패로 현현하는 정반대 방향을 정량화한다. 이는 Knowledge Acquisition 계열([[auxiliary-views]], 반복·보조 뷰의 습득 이득)과 정확히 대칭을 이루는 하한 측정이다. 셋째, [[marginal-distribution-ceiling]]의 'P(y)가 능력 상한을 결정한다'는 원리에 monofact 비율이라는 구체적 데이터 통계를 부여하며, [[scaling-laws]]·[[implicit-curriculum]] 계열의 데이터 구성 변수 공간을 확장한다. [[unguided-scientific-discovery]]([[longchang]])가 발견 능력을 자유 탐색으로 평가했다면 본 논문은 그 상한의 원천을 훈련 데이터에서 설명하여, 평가 축과 훈련 축이 상보적으로 결합됨을 보여준다.

## 🔗 관련 논문

- Elucidating the Design Space of LM Data Attribution
- Molecular Déjà Vu: Digit-Level Retrieval of Published Values in Frontier LLMs
- Can LLMs Uncover Hidden Physical Laws through Free Exploration?
- Knowledge Acquisition During Pre-training? Large Language Models Learn

## 🏷️ 엔티티

- [[entities/data-attribution.md|data-attribution]]
- [[entities/fact-memorization.md|fact-memorization]]
- [[entities/scientific-discovery-capacity.md|scientific-discovery-capacity]]

## 📐 개념

- [[concepts/monofact.md|monofact]]
- [[concepts/missing-probability-mass.md|missing-probability-mass]]
- [[concepts/fact-tracing.md|fact-tracing]]
- [[concepts/marginal-distribution-ceiling.md|marginal-distribution-ceiling]]
- [[concepts/scaling-laws.md|scaling-laws]]
- [[concepts/implicit-curriculum.md|implicit-curriculum]]
- [[concepts/auxiliary-views.md|auxiliary-views]]
- [[concepts/controlled-variable-attribution-evaluation.md|controlled-variable-attribution-evaluation]]
- [[concepts/evaluation-confound-isolation.md|evaluation-confound-isolation]]
- [[concepts/unguided-scientific-discovery.md|unguided-scientific-discovery]]
- [[concepts/digit-level-verbatim-retrieval.md|digit-level-verbatim-retrieval]]
- [[concepts/data-efficiency-gains-from-pretraining.md|data-efficiency-gains-from-pretraining]]

---
_LLM 분석으로 생성됨_
