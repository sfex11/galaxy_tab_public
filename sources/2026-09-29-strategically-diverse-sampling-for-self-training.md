# Strategically Diverse Sampling for Self-Training

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-29
**링크**: http://arxiv.org/abs/2609.31571v1

## 💡 핵심 인사이트

정답 필터링만으로 구축된 셀프트레이닝 데이터는 모델이 이미 선호하는 전략을 증폭하므로, 학습 신호의 선택 기준을 '정확성'에서 '정확성 × 전략적 다양성'으로 이동해야 한다.

## 📖 분석

본 논문은 RL·테스트타임 스케일링·셀프트레이닝이 공유하는 'IID 반복 샘플링 + 정답 필터링' 파이프라인의 구조적 한계를 진단한다: 정답만 걸러내면 모델이 이미 선호하는 전략이 과대표현되어, 정답의 양은 늘어도 접근 방식의 공간은 확장되지 않는다. 이는 [[search-policy-learning]] 계열(ExpBoN의 노이즈 주입, Beyond Repeated Sampling의 의미 조향)이 추론 단계에서 밝힌 근접 중복 문제의 훈련 데이터 구축 단계 발현이며, [[concept-conditioned-sampling]]과 함께 다양성 확보가 테스트타임과 훈련타임 양축으로 분화·확장되는 계층 구조를 완성한다. 제안된 전략적 다양성은 출력의 표면 변이가 아닌 문제 접근 방식의 실질적 변이로, [[training-data-pruning]]의 '고정 예산 내 무엇으로 채울 것인가' 질문에 '서로 다른 방식의 정답으로 채운다'는 응답을 제공하며, [[auxiliary-views]]의 사전학습 통찰(보조 뷰의 인과적 지식 습득 효과)을 셀프트레이닝 영역으로 확장한다. 번역 결정 공간([[alternative-decision-trajectory]])이 입력당 다중 유효 실현의 존재를 진단했다면 본 논문은 그것을 훈련 신호로 수확하는 경로를 열고, [[exploration-absorption-decoupling]] 관점에서 흡수(SFT) 단계가 탐색 분포의 편향을 무비판적 상속하지 않도록 데이터 큐레이션을 독립적 설계 대상으로 격상시킨다.

## 🔗 관련 논문

- Beyond Repeated Sampling: Learning Search Policies for LLM Reasoning
- ExpBoN: Exponential-Noise Best-of-$n$ for Efficient Test-Tim
- SAGE: Mitigating Long-Horizon Reasoning Biases via Topologic
- Knowledge Acquisition During Pre-training? Large Language Models Learn

## 🏷️ 엔티티

- [[entities/strategic-diversity.md|strategic-diversity]]
- [[entities/search-policy-learning.md|search-policy-learning]]
- [[entities/test-time-scaling.md|test-time-scaling]]
- [[entities/training-data-pruning.md|training-data-pruning]]
- [[entities/concept-conditioned-sampling.md|concept-conditioned-sampling]]
- [[entities/exploration-absorption-decoupling.md|exploration-absorption-decoupling]]
- [[entities/self-improving-agent.md|self-improving-agent]]

## 📐 개념

- [[concepts/strategic-diversity.md|strategic-diversity]]
- [[concepts/self-training-data-construction.md|self-training-data-construction]]
- [[concepts/iid-correctness-filter-bias.md|iid-correctness-filter-bias]]
- [[concepts/strategy-coverage-scaling.md|strategy-coverage-scaling]]
- [[concepts/search-policy-learning.md|search-policy-learning]]
- [[concepts/exploration-absorption-decoupling.md|exploration-absorption-decoupling]]

---
_LLM 분석으로 생성됨_
