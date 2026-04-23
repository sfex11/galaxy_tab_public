# Cram Less to Fit More: Training Data Pruning Improves Memorization of Facts

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-13
**링크**: http://arxiv.org/abs/2604.08519v1

## 💡 핵심 인사이트

훈련 데이터의 정보량이 모델 용량을 초과하면 사실 정확도가 하락하며, 데이터 프루닝을 통해 정보 과부하를 줄이면 핵심 사실의 기억이 오히려 향상된다.

## 📖 분석

## Cram Less to Fit More: Training Data Pruning Improves Memorization of Facts

본 논문은 LLM의 사실 기억(fact memorization)을 정보이론적 관점에서 형식화하고, 훈련 데이터 분포가 사실 정확도에 미치는 영향을 분석한다. 핵심 발견은 훈련 데이터에 포함된 사실의 정보량이 모델 용량을 초과하면 사실 정확도가 용량 한계 이하로 떨어진다는 것이다. 이를 해결하기 위해 훈련 데이터 프루닝(pruning)을 제안하며, 덜 중요한 데이터를 제거함으로써 모델이 핵심 사실을 더 잘 기억하도록 유도한다.

### 기존 Wiki와의 관계

- **[[concepts/training-data-pruning.md|training data pruning]]**: 이전 버전(2026-04-11)에서 이미 다뤄진 개념으로, 본 논문은 프루닝이 단순한 효율성 개선을 넘어 사실 기억 품질 자체를 향상시킨다는 이론적 근거를 추가한다.
- **[[concepts/fact-memorization.md|fact memorization]]**: 기존 개념과 직접 연결되며, 정보이론적 프레임워크를 통해 기억 실패의 원인을 모델 용량 대비 정보 과부하로 설명한다.
- **[[concepts/knowledge-injection.md|knowledge injection]]**: SPA(2026-03-25) 등 지식 주입 연구와 상보적 관계. 지식을 추가하는 것이 아니라 불필요한 정보를 제거하여 기억을 개선하는 역방향 접근이다.
- **[[concepts/scaling-laws.md|scaling laws]]**: 모델 용량과 정보량의 관계를 정보이론으로 형식화한 점에서 스케일링 법칙 연구와 맥을 같이 한다.
- **[[concepts/model-pruning.md|model pruning]]**: 모델 가중치 프루닝이 아닌 훈련 데이터 프루닝이라는 점에서 구분되지만, 효율성 추구라는 공통 방향성을 가진다.

### 새로운 인사이트

정보이론적 용량 한계(capacity limit) 개념을 도입하여, "더 많은 데이터가 항상 더 나은 성능"이라는 통념에 반론을 제기한다. Adam's Law(2026-04-03)의 텍스트 빈도 법칙과도 연결되어, 훈련 데이터의 양보다 질과 분포가 사실 학습에 더 중요함을 시사한다.

## 🔗 관련 논문

- 2026 04 11 cram less to fit more training data pruning improv
- 2026 04 12 cram less to fit more training data pruning improv
- 2026 04 03 adams law textual frequency law on large language
- 2026 04 11 what do language models learn and when the implici

## 🏷️ 엔티티

- [[entities/llm.md|LLM]]

## 📐 개념

- [[concepts/training-data-pruning.md|training-data-pruning]]
- [[concepts/fact-memorization.md|fact-memorization]]
- [[concepts/knowledge-injection.md|knowledge-injection]]
- [[concepts/scaling-laws.md|scaling-laws]]
- [[concepts/model-pruning.md|model-pruning]]
- [[concepts/information-theoretic-capacity.md|information-theoretic-capacity]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-04-12-what-do-language-models-learn-and-when-the-implici]]: 둘 다 LLM 사전학습의 데이터-모델 상호작용을 분석하며, 전자는 데이터 프루닝이 사실 기억에 미치는 영향을, 후자는 학습 과정의 능력 습득 순서를 다룬다.
