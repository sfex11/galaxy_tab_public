# Fine-Tuning LLMs for Translation: General Forgetting Mitigation Does Not Preserve MT-Specific Instruction Following

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-25
**링크**: http://arxiv.org/abs/2609.28395v1

## 💡 핵심 인사이트

일반 벤치마크 유지율로 평가된 망각 완화는 MT 특화 지시 수행을 보존하지 않는다 — 망각 보존은 측정 축에 조건부인 다차원 속성이며, 단일 프록시 유지율은 태스크 특화 능력의 소실을 은폐한다.

## 📖 분석

MT 병렬 데이터 파인튜닝이 번역 품질을 높이지만 catastrophic forgetting을 유발하며, 완화 기법들이 통상 일반 벤치마크 유지율로 평가된다는 관행에 대한 도메인 특화 반례다. 논문은 MT 파인튜닝과 MT-IF(형식성·문법적 성별·길이 제어 같은 번역 수정 지시 수행)라는 두 측정 축을 분리하여, 일반 벤치마크 유지율이 MT-IF 보존을 담보하지 않음을 실증한다.

Wiki 관점에서 핵심 기여는 셋이다. 첫째, learning-forgetting-tradeoff에 '측정 축 조건부' 구조를 추가한다 — 보존 판정이 무엇을 측정하는가에 따라 뒤집히는 벤치마크 의존적 속성임을 보인다(Benchmarking World Models의 컨티뉴얼 벤치마크, TM-APR과 병렬). 둘째, fine-tuning-knowledge-erosion의 침식 진단을 MT 도메인과 지시 수행 능력으로 확장한다 — 품질 향상과 지시 수행 소실이 비동기적으로 진행됨을 확정한다. 셋째, evaluation-target-substitution의 실측 사례를 제공한다 — 측정 가능한 일반 유지율 프록시가 MT-IF 보존이라는 실제 목표를 대체하며, 단일 표면 신호의 불충분성 원리를 재확인한다.

보조 데이터·모델 출력·교사 출력에 각각 앵커링된 완화 기법 비교는 parameter-decoupling과 연결된다: 일반 능력 보존과 태스크 특화 지시 수행은 분해 가능한 별도 축이며, 앵커링 선택이 두 축 간 트레이드오프 배분을 결정한다. 이는 LOCUS가 품질-비용을 부공간으로 분해한 것의 보존 목표 버전이다.

## 🔗 관련 논문

- Benchmarking World Models for Continual Learning on Compositional Tasks
- TM-APR: Thermal Temporal-Memory Localization via Analytic Online Adaptation
- LOCUS: Task-Aware Low-Rank Post-Training for Token-Efficient Language Models
- Translation as a Decision Space: A Multi-Agent Perspective on Low-Resource Dialect Generation
- SWE-Gate: Passing Functional Tests Is Not Enough for Software Engineering

## 🏷️ 엔티티

- [[entities/learning-forgetting-tradeoff.md|learning-forgetting-tradeoff]]
- [[entities/fine-tuning-knowledge-erosion.md|fine-tuning-knowledge-erosion]]
- [[entities/benchmark-specification-gap.md|benchmark-specification-gap]]
- [[entities/evaluation-target-substitution.md|evaluation-target-substitution]]
- [[entities/parameter-decoupling.md|parameter-decoupling]]
- [[entities/machine-translation.md|machine-translation]]
- [[entities/single-surface-signal-insufficiency.md|single-surface-signal-insufficiency]]
- [[entities/continual-learning.md|continual-learning]]

## 📐 개념

- [[concepts/mt-instruction-following.md|mt-instruction-following]]
- [[concepts/retention-proxy-mismatch.md|retention-proxy-mismatch]]

---
_LLM 분석으로 생성됨_
