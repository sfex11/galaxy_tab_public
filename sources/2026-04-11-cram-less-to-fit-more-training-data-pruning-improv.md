# Cram Less to Fit More: Training Data Pruning Improves Memorization of Facts

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-11
**링크**: http://arxiv.org/abs/2604.08519v1

## 💡 핵심 인사이트

학습 데이터의 사실 정보량이 모델 용량을 초과하면 기억 정확도가 저하되며, 데이터 프루닝을 통해 정보량을 줄이면 오히려 사실 기억이 향상된다.

## 📖 분석

## Cram Less to Fit More: Training Data Pruning Improves Memorization of Facts

본 논문은 LLM의 사실 기억(fact memorization) 문제를 정보 이론적 관점에서 형식화한 연구이다. 핵심 발견은 학습 데이터에 포함된 사실 정보량이 모델 용량을 초과하면 사실 정확도가 최적 이하로 떨어진다는 것이며, 이를 해결하기 위해 학습 데이터 프루닝(data pruning)을 제안한다. 즉, 더 적게 넣을수록 더 잘 기억한다는 역설적 결과를 보여준다.

### 기존 Wiki와의 관계

- **LLM**: 본 논문의 직접적 연구 대상. LLM의 파라미터에 사실 지식을 저장하는 메커니즘과 한계를 분석한다.
- **knowledge-injection**: 사실 지식을 모델에 주입하는 관점에서 밀접한 관련이 있다. SPA(2026-03-25) 논문이 합성 데이터를 통한 지식 주입을 다뤘다면, 본 논문은 기존 데이터의 프루닝을 통해 지식 흡수율을 높이는 상보적 접근이다.
- **model-pruning / model-compression**: 모델 가중치 프루닝이 아닌 학습 데이터 프루닝이라는 점에서 구별되지만, '불필요한 것을 제거하여 성능을 향상시킨다'는 철학을 공유한다.
- **synthetic-data-generation**: 학습 데이터 분포 최적화라는 측면에서, 합성 데이터 생성과 데이터 프루닝은 동전의 양면이다.

### 핵심 기여

정보 이론적 용량 한계(capacity limit)라는 개념을 도입하여, LLM의 사실 기억 실패(hallucination)를 데이터 과잉의 관점에서 설명한 점이 독창적이다. 이는 단순히 모델을 키우는 것이 아니라 데이터 분포를 최적화하는 것이 hallucination 감소에 효과적일 수 있음을 시사한다.

## 🔗 관련 논문

- 2026 03 25 spa a simple but tough to beat baseline for knowle
- 2026 04 08 how ai aggregation affects knowledge

## 🏷️ 엔티티

- [[entities/llm.md|LLM]]

## 📐 개념

- [[concepts/knowledge-injection.md|knowledge-injection]]
- [[concepts/model-pruning.md|model-pruning]]
- [[concepts/synthetic-data-generation.md|synthetic-data-generation]]
- [[concepts/training-data-pruning.md|training-data-pruning]]
- [[concepts/fact-memorization.md|fact-memorization]]

---
_LLM 분석으로 생성됨_
