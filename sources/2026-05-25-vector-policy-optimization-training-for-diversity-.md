# Vector Policy Optimization: Training for Diversity Improves Test-Time Search

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-25
**링크**: http://arxiv.org/abs/2605.22817v1

## 💡 핵심 인사이트

표준 RL 사후학습의 스칼라 보상은 '탐색에 필요한 다양성'이라는 인지적 요구를 충족하지 못하는 근본적 설계 결함을 VPO가 보상 벡터화로 해결한다. 스칼라 보상이 특정 엔트로피 지역으로 수렴하는 데 반해, 벡터 보상이 다양한 탐색 경로로 확률 분포를 장려하도록 모델을 학습시킨다는 구조적 제안이다.

## 📖 분석

# vector-policyoptimization

**카테고리**: 미분류
**생성일**: 2026-05-25

## 정의
표준 사후학습에서 사전 정의된 스칼라 보상을 최적화하면 언어 모델이 낮은 엔트로피 출력 분포를 학습하게 되어, AlphaEvolve 같은 추론 시점 탐색 절차에 필요한 다양성을 발�하지 못하는 문제를 다룬다. Vector Policy Optimization(VPO)은 스칼라 보상을 텍스트가 아닌 과제 특화 보상 벡터로 대체하여, 학습된 모델이 추론 시점 탐색의 다양한 보상 함수에 걸쳐 확률 분포를 학습하도록 설계하는 사후학습 방법론이다.

## 관련 논문
- sources/2605.22817-vector-policy-optimization-training-for-diversity-improves-test-time-sear.md

---

# output-entropy-degradation
**카테고리**: 미분류
**생성일**: 2026-05-25

## 정의
표준 사후학습의 스칼라 보상 최적화가 모델의 출력 분포의 엔트로피를 점진적으로 감소시키는 현상이다. 모델이 스칼라 보상을 극대화하는 '안전한' 저엔트로피 지역을 학습하게 되어, 탐색 기반 추론 시스템이 요구하는 높은 다양성의 탐색 경로를 탐색할 수 없게 된다.

## 관련 논문
- sources/2605.22817-vector-policy-optimization-training-for-diversity-improves-test-time-sear.md

---

---
```

## 🏷️ 엔티티

- [[entities/vector-policyoptimization.md|vector-policyoptimization]]
- [[entities/output-entropy-degradation.md|output-entropy-degradation]]

## 📐 개념

- [[concepts/output-entropy-degradation.md|output-entropy-degradation]]

---
_LLM 분석으로 생성됨_
