# Elucidating the Design Space of LM Data Attribution

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-31
**링크**: http://arxiv.org/abs/2610.40655v1

## 💡 핵심 인사이트

LM 데이터 귀속의 병목은 귀속 알고리즘이 아니라 평가 설계에 있으며, 데이터셋 속성의 단일 변수 통제 변이만이 실패 원인의 인과적 진단을 가능하게 한다.

## 📖 분석

## 데이터 귀속 평가의 설계 공간

LLM 데이터 귀속(data attribution) 연구의 평가 방법론 설계 공간을 체계화한다. 기존 평가는 사실 검색 같은 하류 태스크에서 여러 데이터셋 속성을 동시에 변이시켜, 귀속 알고리즘이 왜 실패하는지 원인을 분리할 수 없다는 문제를 진단한다. 이를 위해 Controlled Attribution Benchmark(CATT)를 제안한다 — 엔티티 단위 미세조정으로 사실 추적(fact tracing)을 수행하되, 데이터셋 속성을 한 번에 하나씩 통제 변이시켜 실패 원인을 격리한다.

이 접근은 [[matched-condition-comparison]]의 귀속 도메인 확장이다 — 분포 이동을 성분별로 분해해 사전학습 이득을 격리했던 것과 동일한 '성분 분해로 인과 격리' 원리가 귀속 평가에 적용된다. [[benchmark-specification-gap]]에도 정밀화를 공급한다: 명세 간극이 '무엇을 측정할지'의 문제였다면, 본 논문은 '교란 변수를 어떻게 통제할지'라는 방법론 차원을 추가한다.

데이터 귀속은 [[layer-selective-unlearning]] 계열 표적 제거의 전제 조건이기도 하다 — 어떤 데이터가 특정 출력에 기여했는지를 알아야 선택적 제거가 가능하며, 본 논문은 그 귀속 능력 자체의 신뢰성을 측정 가능하게 만든다. [[fact-memorization]]과의 접점에서, 자릿수 수준 검색이 '기억되었는가'를 감사했다면 CATT는 '무엇으로부터 기억되는가'를 감사하여 기억 연구의 질문을 훈련 데이터 원천으로 소급시킨다.

## 🔗 관련 논문

- How Does Distribution Shift Shape Pretraining Gains in Neural PDE Surrogates
- Molecular Déjà Vu: Digit-Level Retrieval of Published Values in Frontier LLMs
- Forgetting Only What Matters: Layer-Selective Unlearning toward Robust Unlearning

## 🏷️ 엔티티

- [[entities/data-attribution.md|data-attribution]]
- [[entities/matched-condition-comparison.md|matched-condition-comparison]]
- [[entities/benchmark-specification-gap.md|benchmark-specification-gap]]
- [[entities/fact-memorization.md|fact-memorization]]
- [[entities/layer-selective-unlearning.md|layer-selective-unlearning]]

## 📐 개념

- [[concepts/controlled-variable-attribution-evaluation.md|controlled-variable-attribution-evaluation]]
- [[concepts/fact-tracing.md|fact-tracing]]
- [[concepts/evaluation-confound-isolation.md|evaluation-confound-isolation]]

---
_LLM 분석으로 생성됨_
