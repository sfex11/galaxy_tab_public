# Distill Globally, Adapt Locally: Reasoning Distillation and Product-Type Test-Time Training for Scalable Trade-Up Recommendation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-08
**링크**: http://arxiv.org/abs/2609.05363v1

## 💡 핵심 인사이트

LLM 추론의 대규모 배포 비경제성을 해결하는 길은 소형 모델의 추론 능력 향상이 아니라, 생성 능력을 버리고 판단 기준만 이전하는 증류(글로벌)와 도메인별 기준의 테스트타임 적응(로컬)의 분업이다.

## 📖 분석

Trade-up 추천에서 LLM 추론을 두 단계로 활용하는 프레임워크를 제시한다: Level 1에서 LLM 추론을 효율적 비생성적 학생 모델로 증류하고(글로벌), Level 2에서 제품 유형별 트레이드업 기준에 테스트타임 훈련(TTT)으로 결정 경계를 적응시킨다(로컬).

Wiki 관점의 기여는 세 층위다. 첫째, knowledge-distillation의 대상을 재정의한다 — TIDE가 확산 LLM 간 지식 전이였다면 본 논문은 생성적 추론기를 생성 능력조차 없는 판별 모델로 증류하여, 전이되는 것이 토큰 분포가 아닌 '무엇이 업그레이드이고 무엇이 의도 이탈인가'라는 판단 기준임을 보여준다. 위키가 축적한 생성 모델 간 증류 논의와 구별되는 '추론→결정 논리 전이' 축이며, 교사 추론 품질이 학생 상한을 규정한다는 점에서 marginal-distribution-ceiling의 교사-학생 버전이기도 하다.

둘째, test-time-training을 '테스트 데이터 제자리 학습'에서 '배포 후 도메인별 기준 적응'으로 확장한다. 글로벌 능력은 설계 시점 증류에, 로컬 기준은 런타임 TTT에 배치하는 구조는 설계-런타임 정렬 이중성의 추천 도메인 발현이다.

셋째, 수억 상품 쌍에 LLM을 직접 적용하는 비경제성이 아키텍처를 결정함으로써, slm-reasoning-gap을 '추론 능력 향상'이 아닌 '추론 필요성 제거'로 해소하는 우회 경로를 제공한다 — 교사가 추론하고 학생은 결정만 수행한다.

## 🔗 관련 논문

- In-Place Test-Time Training
- Select to Think: Unlocking SLM Potential with Local Sufficiency
- Turning the TIDE: Cross-Architecture Distillation for Diffusion Large Language Models
- Standing on the Shoulders of Giants: Stabilized Knowledge Distillation

## 🏷️ 엔티티

- [[entities/knowledge-distillation.md|knowledge-distillation]]
- [[entities/test-time-training.md|test-time-training]]
- [[entities/slm-reasoning-gap.md|slm-reasoning-gap]]
- [[entities/marginal-distribution-ceiling.md|marginal-distribution-ceiling]]
- [[entities/reasoning-distillation.md|reasoning-distillation]]
- [[entities/distill-globally-adapt-locally.md|distill-globally-adapt-locally]]

## 📐 개념

- [[concepts/recommendation-system.md|recommendation-system]]
- [[concepts/design-runtime-alignment-duality.md|design-runtime-alignment-duality]]

---
_LLM 분석으로 생성됨_
