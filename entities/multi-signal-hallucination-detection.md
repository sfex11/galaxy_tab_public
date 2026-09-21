# multi-signal-hallucination-detection

**카테고리**: 미분류
**생성일**: 2026-09-12

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-09-12-domain-specific-hallucination-detection-in-large-l.md|Domain-Specific Hallucination Detection in Large Language Mo]]

### Domain-Specific Hallucination Detection in Large Language Models (2026-09-13)

본 논문이 이 엔티티의 원천 구현이다. 미세조정 분류기·MC Dropout 불확실성·온도 스케일링 보정이라는 3신호 결합 파이프라인으로 '다중 신호'가 단순한 앙상블이 아니라 직교 정보원(의미·확신·보정)의 결합임을 HaluEval 실증(F1=0.915, AUROC=0.977)으로 확립한다.

### Look Before You Leap: Factual Decoding with Internal Attribution Signa (2026-09-16)

동일 환각 문제에 대한 시간축 반대편 해법을 제공한다 — 3신호(분류·불확실성·보정) 결합이 '생성 완료 후' 감지라면 DescaPE는 내부 귀속 신호로 '생성 중' 환각 궤적을 억제하여, 환각 개입이 사후 감지와 선제 억제의 이중 구조로 분화함을 보여준다.

### Predictable Failure in Multi-Hop Retrieval: Score-Distributional Confi (2026-09-22)

직교 정보원 결합 원리의 검색 도메인 대응물을 제공한다 — LLM-judge 특징과 dense 특징의 상보성이 어느 단일 신호원만으로는 confident-failure 감축이 불완전함을 이론적으로 확립하여, 다중 신호 파이프라인의 필요성을 환각 감지 너머 검색 품질 감시로 확장한다.

→ [[sources/2026-09-22-predictable-failure-in-multi-hop-retrieval-score-d.md|상세 보기]]

### An Interpretable Memory Decision Controller for LLM Agents Based on Th (2026-09-22)

다중 신호 결합 원리의 위상 전환을 제공한다 — 환각을 사후 감지하는 분류·불확실성·보정 파이프라인과 달리, 본 논문은 동일 다중 신호 원리를 메모리 수용 판단에 배치하여 감지에서 예방으로 이동시킨다.

→ [[sources/2026-09-22-an-interpretable-memory-decision-controller-for-ll.md|상세 보기]]
