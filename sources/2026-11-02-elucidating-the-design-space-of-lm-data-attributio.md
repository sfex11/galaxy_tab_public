# Elucidating the Design Space of LM Data Attribution

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-02
**링크**: http://arxiv.org/abs/2610.40655v1

## 💡 핵심 인사이트

데이터 귀속 평가가 여러 데이터셋 속성을 동시에 변이시키는 구조적 교란을 제거해야만, 귀속 알고리즘의 실패 원인을 진단할 수 있다.

## 📖 분석

LM 데이터 귀속(data attribution) 연구의 평가 방법론 자체를 문제화하는 논문이다. 기존 평가가 팩트 검색 같은 하류 태스크에서 여러 데이터셋 속성을 동시에 변이시켜, 귀속 알고리즘 실패의 원인을 분리 진단할 수 없다는 한계를 지적하고, 통제 실험 설계로 이를 해결한다.

[[data-attribution]] 엔티티의 원천 논문으로서, 귀속 평가의 설계 공간을 명시적으로 다루는 최초의 체계적 프레임워크를 제공한다. Controlled Attribution Benchmark(CATT)는 팩트 트레이싱을 위해 LLM을 특정 엔티티 문서로 미세조정한 뒤, 하나의 속성만 변이하는 통제 조건 하에서 귀속 알고리즘의 실패 원인을 격리한다.

기존 Wiki의 [[fact-memorization]] 논의와 직결된다 — 'Forgetting Only What Matters'가 기억의 존재와 제거 가능성을 다뤘다면, 본 논문은 특정 팩트가 모델에 학습된 것을 귀속 알고리즘이 정확히 추적할 수 있는가라는 감사 축을 추가한다. 기억 감사가 '있는가/없는가'에서 '어디서 왔는가'로 정밀화되는 단계다.

또한 [[evaluation-confound-isolation]] 및 [[controlled-variable-attribution-evaluation]]과 연결되어, 벤치마크 설계에서 속성 변이를 격리하는 원리를 데이터 귀속 도메인에 적용한 사례가 된다. [[benchmark-specification-gap]]의 일반 원리 — 평가 설계가 측정 대상을 결정한다 — 가 귀속 평가에서 재현되는 구조이며, [[meaning-insensitive-metric]]이 지적한 '무엇을 측정하는가'의 명세 문제와도 공명한다.

ML 해석가능성과 학습 데이터 거버넌스를 잇는 다리로서, [[data-contamination-resistance]] 및 [[benchmark-contamination-audit]] 논의에 '귀속 기반 감사'라는 새로운 방법론적 축을 공급한다.

## 🔗 관련 논문

- 2026-10-31-elucidating-the-design-space-of-lm-data-attributio

## 🏷️ 엔티티

- [[entities/data-attribution.md|data-attribution]]
- [[entities/fact-memorization.md|fact-memorization]]
- [[entities/evaluation-confound-isolation.md|evaluation-confound-isolation]]
- [[entities/controlled-variable-attribution-evaluation.md|controlled-variable-attribution-evaluation]]
- [[entities/data-contamination-resistance.md|data-contamination-resistance]]

## 📐 개념

- [[concepts/controlled-attribution-benchmark.md|controlled-attribution-benchmark]]
- [[concepts/attribution-failure-isolation.md|attribution-failure-isolation]]
- [[concepts/fact-tracing.md|fact-tracing]]

---
_LLM 분석으로 생성됨_
