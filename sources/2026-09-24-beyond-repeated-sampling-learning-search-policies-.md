# Beyond Repeated Sampling: Learning Search Policies for LLM Reasoning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-24
**링크**: http://arxiv.org/abs/2609.26704v1

## 💡 핵심 인사이트

탐색을 국소 디코딩 노이즈에 맡기는 대신 문제별 개념·힌트를 먼저 샘플링하는 학습된 탐색 정책으로 의미 수준에서 조향하면, 반복 샘플링의 근접 중복 문제 없이 진짜로 다른 아이디어를 탐색할 수 있다.

## 📖 분석

테스트타임 스케일링의 지배 전략인 단순 반복 샘플링(best-of-n)이 국소 디코딩 노이즈에만 의존해 근접 중복 시도를 대량 생산한다는 진단을 내리고, 탐색을 의미 수준에서 조향하는 학습된 탐색 정책을 제안한다. 문제별 개념·힌트·구조를 해 이전에 샘플링하고 그에 조건화된 해를 생성함으로써 진짜로 다른 아이디어 간 탐색이 가능해진다.

[[soft-best-of-n]](ExpBoN)이 노이즈 주입으로 best-of-n 탐색을 개선하려 한 것과 대비되는 제2의 축이다 — 노이즈 구조화가 디코딩 계층 내 최적화라면 본 논문은 탐색 공간 자체를 의미 변수로 상승시켜 국소 노이즈의 한계를 구조적으로 회피한다. [[decoder-primitive-redefinition]] 계열의 적응 진화(선택 연산 재설계)에 '탐색의 의미적 상승'이라는 제4세대 후보를 추가한다.

[[unrealized-branch-diversity-source]]의 원리 — 다양성의 진짜 원천은 미실현 분기 — 를 테스트타임에 직접 실현하는 사례다. 반복 샘플링이 실현된 경로의 노이즈 변주에 머무는 반면 개념 우선 샘플링은 미실현 의미 분기를 먼저 개척한다. [[alternative-decision-trajectory]]와 [[parallel-strategy-exploration]]이 수렴 전 대안 공간 유지를 다뤘다면, 본 논문은 그 공간의 생성 원천을 디코딩 노이즈에서 의미 표본으로 이동시킨 것이며, 예산을 어디에 쓸지를 학습한다는 점에서 [[inference-budget-progressive-investment]]와도 연결된다.

## 🔗 관련 논문

- ExpBoN: Exponential-Noise Best-of-$n$ for Efficient Test-Time Scaling
- Beyond Truncation: Rethinking LLM Decoding as Ensemble Pruning
- Translation as a Decision Space: A Multi-Agent Perspective on Low-Resource Dialect Generation
- Stellar Colosseum: A Many-Agent Harness for Long-Horizon Research in Mathematics

## 🏷️ 엔티티

- [[entities/test-time-scaling.md|test-time-scaling]]
- [[entities/soft-best-of-n.md|soft-best-of-n]]
- [[entities/semantic-exploration-steering.md|semantic-exploration-steering]]
- [[entities/search-policy-learning.md|search-policy-learning]]
- [[entities/concept-conditioned-sampling.md|concept-conditioned-sampling]]

## 📐 개념

- [[concepts/decoder-primitive-redefinition.md|decoder-primitive-redefinition]]
- [[concepts/unrealized-branch-diversity-source.md|unrealized-branch-diversity-source]]
- [[concepts/alternative-decision-trajectory.md|alternative-decision-trajectory]]
- [[concepts/parallel-strategy-exploration.md|parallel-strategy-exploration]]
- [[concepts/inference-budget-progressive-investment.md|inference-budget-progressive-investment]]
- [[concepts/kl-regularized-reward-maximization.md|kl-regularized-reward-maximization]]
- [[concepts/extra-probabilistic-adjudication.md|extra-probabilistic-adjudication]]

---
_LLM 분석으로 생성됨_
