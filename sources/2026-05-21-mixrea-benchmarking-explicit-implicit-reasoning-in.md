# MixRea: Benchmarking Explicit-Implicit Reasoning in Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-21
**링크**: http://arxiv.org/abs/2605.20128v1

## 💡 핵심 인사이트

LLM 평가의 '명시적 성능'과 '은연적 이해'를 분리 불가능하게 혼합하는 기존 벤치마크의 구조적 한계를, 인지 심리학의 주의적 맹점 이론을 빌려 새로운 평가 차원을 도입하여 해결한다.

## 📖 분석

# MixRea: 인지적 맹점과 LLM 추론 평가의 교차점

MixRea는 인지 심리학의 **주의적 맹점(inattentional blindness)** — 명시적 자극이 암시적 맥락을 억압한다는 인지적 한계 — 를 LLM 평가에 도입한다. LLM이 사람 선호 코퍼스에 내재된 주의 편향으로 학습되었기 때문에, 명시적 지시가 있는 상황에서도 은연적 맥락이 중요한 맥락을 무시하는 현상이 인간의 주의적 맹점과 구조적으로 동형적임을 제안한다.

이는 기존 [[reasoning-integrity]]에 새로운 차원을 추가한다. 추론 무결성이 논리적 타당성뿐 아니라 **주의적 완전성** 차원에서도 평가되어야 함을 시사한다. ceiling-performance-prorupt과도 직접 연결된다 — 기존 벤치마크가 명시적 지시만을 측정하므로 은연적 차원의 실패를 포착하지 못하는 구조적 누락이다.

[[shortcut-learning]]과의 관계도 흥미롭다. 주의적 맹점이 shortcut-learning의 한 특수 형태로, 명시적 큐에에 대한 과도 의존이 은연적 큐에에 대한 무시로 구현됨을 보여준다. MixRea는 이 메커니즘을 벤치마크로 포착 가능하게 만든다는 점에서, 기존 adversarial-problem-generation 계열(MathDuels, VHG 등)이 놓친 '난이도' 축에 '주의 편향' 축이라는 새로운 적대적 차원을 제안한다.

## 🏷️ 엔티티

- [[entities/inattentional-blindness.md|inattentional-blindness]]
- [[entities/mixrea.md|mixrea]]

## 📐 개념

- [[concepts/explicit-implicit-reasoning.md|explicit-implicit-reasoning]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-05-21-copt-contrastive-on-policy-thinking-with-continuou]]: 두 논문 모두 LLM의 추론 과정에서 명시적 사고와 암시적 이해의 상호작용을 분석하고 개선 방안을 제시한다.
