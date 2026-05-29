# Learn from Weaknesses: Automated Domain Specialization for Small Computer-Use Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-29
**링크**: http://arxiv.org/abs/2605.28775v1

## 💡 핵심 인사이트

이 논문은 small CUA의 도메인별 약점을 '데이터 부족'가 아니라 '학습 부족' 문제로 재정의하며, skill-consumption-gap의 본질성을 구체화한다. 소형 에이전트에게 단순한 도메인 데이터 합성만으로는 근본적 접근의 효과를 보여하며, 에이전트의 실제 약점을 기반으로 한 하네스 데이터를 자동 생성하는 방식으로, 하네스 스케일링이 모델 스케일링과 독립적인 두 축을 갖는 구조적 간극을 해소한다.

## 📖 분석

# automated-domain-specialization

**카테고리**: 미분류
**생성일**: 2026-05-29

## 정의
소형 computer-use agent(CUA)의 도메인별 약점은 대규모 전문을 대상으로 한 데이터 합성만으로는 미미약한 개선을 낳는다. 본련 논문은 이 문제를 '데이터 부족'가 아니라 '학습 부족' 문제로 재정의하며, 에이전트의 실제 약점을 자동으로 식별하여 그에 특화된 훈련 데이터를 합성하는 프레임워크다. 이는 단순한 도메인 데이터 합성이 효과하지만 소형 에이전트의 근본적 약점은 모델 스케일업과 무관하게 지속된다는 발견을 통해, skill-consumption-gap의 본질성을 구체화한다.

## 관련 논문
- sources/2026-05-29-learn-from-weaknesses-automated-domain-specification-for-small-c.md

---
# skill-consumption-gap
**카테고리**: 미분류
**생성일**: 2026-05-26

## 정의
에이전트가 원시도메 디버그 문제를 겪은 후, 그 경험을 구조화된 스킬로서 외부 저장소에 축적하는 대신, 실패 경험을 실제로 소모할 수 있는 스킬로 변환하는 것은 에이전트의 능력을 외부 인프라에 의존시키는 구조적 한계이다. 이 한계층에서는 데이터 기반 접근(모벸이 '올바른 답'을 보여주는 데이터를 많이 줄 수록)이 아닌라 에이전트가 자신의 실패 패턴에서 학습하지 못하는 원인을 제공한다. automated-domain-specialization은 이 한계층의 문제를 자동화된 약점 식별과 타겟 데이터 합성으로 해결하려 시도, 실패 경험의 '어떤 부분'에서만 데이터를 생성하면 에이전트가 이미 가진 능력을 위협하는 정책(positive-only-policy-optimization의 역설과 유사)에 빠질 가능성을 경고한다.
## 관련 논문
- sources/2026-05-29-learn-from-weaknesses-automated-domain-specification-for-small-c.md
---
# from-raw-experience-to-skill-consumption
**카테고리**: 미분류
**생성일**: 2026-05-26
## 정의
에이전트의 원시도메 디버그 문제를 겪은 후, 그 경험을 구조화된 스킬로 외부 저장소에 축적하는 대신, 실패 경험을 실제로 소모할 수 있는 스킬로 변환하는 것은 에이전트의 능력을 외부 인프라에 의존시키는 구조적 한계이다. 이 한계층에서는 데이터 기반 접근(모벨이 '올바른 답'을 보여주는 데이터를 많이 줄 수록)이 아닌라 에이전트가 자신의 실패 패턴에서 학습하지 못하는 원인을 제공한다. automated-domain-specialization은 이 한계층의 문제를 자동화된 약점 식별과 타겟 데이터 합성으로 해결하려 시도, 실패 경험의 '어떤 부분'에서만 데이터를 생성하면 에이전트가 이미 가진 능력을 위협하는 정책(positive-only-policy-optimization의 역설과 유사)에 빠질 가능성을 경고한다.
## 관련 논문
- sources/2026-05-29-learn-from-weaknesses-automated-domain-specification-for-small-c.md
---
# system-scaling
**카테고리**: 미분류
**생성일**: 2026-05-27
## 정의
기존 Wiki에서 '모델 스케일링(파라미터·데이터·컴퓨트·스텝�)'을 중심으로 한 하네스 스케일링 프레임워크다. 이 프레임워크는 모델 자체의 능력 상한을 높이는 것이 아니라, 에이전트를 둘러가 작동하는 인프라(하네스)를 감사 가능·지속·모듈러로 확장하는 네 가지 중 하나의 축이다. automated-domain-specialization은 이 하네스 스케일링의 '데이터 파이프라인' 축에서, 단순히 도메인 데이터를 쏟아 넣는 것이 아니라 에이전트의 실제 약점을 기반으로 한 하네스 데이터를 자동 생성하는 방식으로, 하네스 스케일링이 모델 스케일링과 독립적인 두 축을 갖는 구조적 간극을 해소한다.
## 관련 논문
- sources/2026-05-27-from-model-scaling-to-system-scaling-scaling-the-h.md
---

## 🏷️ 엔티티

- [[entities/automated-domain-specialization.md|automated-domain-specialization]]

## 📐 개념

- [[concepts/automated-domain-specialization.md|automated-domain-specialization]]

---
_LLM 분석으로 생성됨_
