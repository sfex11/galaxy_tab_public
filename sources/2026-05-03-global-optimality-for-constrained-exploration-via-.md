# Global Optimality for Constrained Exploration via Penalty Regularization

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-03
**링크**: http://arxiv.org/abs/2604.28144v1

## 💡 핵심 인사이트

엔트로피 최대화의 비가산성이 벨만 방정식의 적용을 근본적으로 차단하며, 이것이 제약 탐색에서 표준 RL이 '위양성 수렴'에 빠지는 구조적 원인이다.

## 📖 분석

# Global Optimality for Constrained Exploration via Penalty Regularization

**카테고리**: 강화학습/탐색 이론
**생성일**: 2026-05-03

## 정의

제약 조건(안전, 자원, 모방 요구사항 등)이 부과된 환경에서 상태-행동 점유 측도(occupancy measure)의 엔트로피를 최대화하는 탐색 문제에 대해, 페널티 정규화를 통해 전역 최적해를 도출하는 이론적 프레임워크.

## 핵심 기여

### 엔트로피의 비가산성 문제의 형식화
엔트로피 최대화는 가산적(additive) 구조를 갖지 않아 벨만 방정식 기반 방법이 적용 불가능하다는 근본적 난제를 형식적으로 정의한다. 이는 [[concepts/constrained-exploration.md|constrained exploration]]이 단순한 제약 최적화의 연장선이 아님을 수학적으로 보장한다.

### 제약 탐색의 전역 최적성 보장
페널티 정규화가 제약 탐색에서 전역 최적해에 수렴함을 증명하여, 기존 경험적 해법(GP 기반 안전 탐색 등)이 우회했던 근본 난제를 이론적으로 해결한다.

## 기존 Wiki와의 관계

### exploration-hacking에 대한 이론적 근거 제공
[[concepts/exploration-hacking.md|exploration hacking]]에서 모델이 '가장 쉬운 궤적'만 생성하여 [[concepts/false-positive-convergence.md|false positive convergence]]에 빠지는 현상은, 엔트로피의 비가산성이 만들어내는 최적화 지형의 구조적 특성과 직접 연결된다. 벨만 방정식이 적용 불가한 지형에서 표준 RL 알고리즘이 발견하는 '수렴'이 실제로는 지역 최적점일 가능성을 이론적으로 뒷받침한다.

### safety-aware-exploration의 근본 난제 해결
[[concepts/safety-aware-exploration.md|safety aware exploration]]에서 Hough transform 기반 GP 접근이 '엔트로피의 비가산성'이라는 근본 난제를 경험적으로 우회한 실증적 해법이었다면, 본 논문은 그 난제 자체를 정의하고 해결하는 이론적 경로를 제공한다.

## 관련 논문

- [[sources/2026-05-03-global-optimality-for-constrained-exploration-via-.md|Global Optimality for Constrained Exploration via Penalty Re]]

## 🔗 관련 논문

- 2026-05-01-safe-navigation-using-neural-radiance-fields-via-r.md
- 2026-05-02-exploration-hacking-can-llms-learn-to-resist-rl-tr.md
- 2026-04-24-a-hough-transform-approach-to-safety-aware-scalar-.md

## 🏷️ 엔티티

- [[entities/constrained-exploration.md|constrained-exploration]]
- [[entities/entropy-regularized-planning.md|entropy-regularized-planning]]
- [[entities/occupancy-measure-optimization.md|occupancy-measure-optimization]]
- [[entities/penalty-regularization.md|penalty-regularization]]
- [[entities/non-additive-entropy.md|non-additive-entropy]]
- [[entities/safety-aware-exploration.md|safety-aware-exploration]]
- [[entities/exploration-hacking.md|exploration-hacking]]

## 📐 개념

- [[concepts/non-additive-entropy.md|non-additive-entropy]]
- [[concepts/non-additive-exploration.md|non-additive-exploration]]
- [[concepts/false-positive-convergence.md|false-positive-convergence]]
- [[concepts/exploration-avoidance-tradeoff.md|exploration-avoidance-tradeoff]]
- [[concepts/exploration-strategy-corruption.md|exploration-strategy-corruption]]

---
_LLM 분석으로 생성됨_
