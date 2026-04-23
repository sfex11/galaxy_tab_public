# Cram Less to Fit More: Training Data Pruning Improves Memorization of Facts

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-12
**링크**: http://arxiv.org/abs/2604.08519v1

## 💡 핵심 인사이트

학습 데이터의 정보량이 모델 용량을 초과하면 사실 정확도가 저하되며, 데이터 pruning을 통해 정보 밀도를 최적화하면 동일 용량에서 더 많은 사실을 정확히 기억할 수 있다.

## 📖 분석

## Cram Less to Fit More: Training Data Pruning Improves Memorization of Facts

본 논문은 LLM의 사실 기억(fact memorization) 문제를 정보이론적 관점에서 형식화하고, 학습 데이터 분포가 사실 정확도에 미치는 영향을 분석한다.

### 핵심 기여
- **정보이론적 형식화**: 학습 데이터에 포함된 사실의 정보량이 모델 용량을 초과하면 사실 정확도가 최적 이하(capacity limit 미달)가 됨을 이론적으로 증명
- **Training Data Pruning**: 중복되거나 노이즈가 있는 학습 데이터를 제거함으로써, 동일한 모델 용량에서 더 많은 사실을 정확히 기억할 수 있음을 실증
- **용량-정보 트레이드오프**: 모델이 "더 적게 cramming"할수록 실제로 "더 많이 fit"할 수 있다는 역설적 결과 제시

### 기존 연구와의 관계
- [[concepts/training-data-pruning.md|training data pruning]] 개념의 핵심 이론적 근거를 제공하며, 기존 데이터 pruning이 단순 효율성을 넘어 기억 품질 향상에 기여함을 보임
- [[concepts/fact-memorization.md|fact memorization]] 개념을 정보이론적으로 정식화한 최초 시도로, hallucination 감소와 직접 연결
- [[concepts/knowledge-injection.md|knowledge injection]]과 관련하여, 외부 지식 주입 전에 학습 데이터 품질 최적화가 선행되어야 함을 시사
- [[concepts/scaling-laws.md|scaling laws]]와 연결: 모델 크기 증가만이 아닌 데이터 분포 최적화를 통한 성능 향상 경로 제시
- [[concepts/curriculum-learning.md|curriculum learning]]의 데이터 선별 전략과 상호보완적 관계

### 시사점
정보이론적 capacity limit 개념은 LLM의 사실 기억 한계를 이해하는 새로운 프레임워크를 제공하며, 합성 데이터 생성([[concepts/synthetic-data-generation.md|synthetic data generation]]) 시에도 정보 밀도 최적화가 중요함을 암시한다.

## 🔗 관련 논문

- 2026 04 11 cram less to fit more training data pruning improv
- 2026 04 11 what do language models learn and when the implici
- 2026 04 03 adams law textual frequency law on large language

## 🏷️ 엔티티

- [[entities/llm.md|LLM]]

## 📐 개념

- [[concepts/training-data-pruning.md|training-data-pruning]]
- [[concepts/fact-memorization.md|fact-memorization]]
- [[concepts/knowledge-injection.md|knowledge-injection]]
- [[concepts/scaling-laws.md|scaling-laws]]
- [[concepts/curriculum-learning.md|curriculum-learning]]
- [[concepts/synthetic-data-generation.md|synthetic-data-generation]]
- [[concepts/model-pruning.md|model-pruning]]

---
_LLM 분석으로 생성됨_
