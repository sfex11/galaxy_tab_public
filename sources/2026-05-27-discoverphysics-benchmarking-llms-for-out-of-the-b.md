# DiscoverPhysics: Benchmarking LLMs for Out-of-the-Box Scientific Thinking

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-27
**링크**: http://arxiv.org/abs/2605.26087v1

## 💡 핵심 인사이트

기존 벤치마크는 '어려운 문제를 더 어렵게 만드어'는 방식으로 천장 성능 문제를 해결하지 못한다. DiscoverPhysics는 이 문제의 근본 원인—표준 물리 법칙에 대한 사전 지식이 추론의 도구가 되는 현상—을 직접적으로 노출한다. adversarial problem generation이 문제를 더 어렵게 만드는 것과 구조적으로 유사하면서, 환경 자체를 변형하여 '힌(기억)'을 비활성으로 변환하는 이중 해결책이다.

## 📖 분석

# counterfactual-physics-reasoning

**카테고리**: 미분류
**생성일**: 2026-05-27

## 정의
표준 물리 법칙에 대한 사전 학습 지식이 오히려려리는 도구가 되는 역설적 상황에서, 의도적으로 물리 법칙이 편향된 환경에서 제1원리부터 물리 법칙을 발견하도록 하는 추론 능력. 기존 벤치마크(standard physics)의 천장 성능 문제와 sandbox-liveworld-gap(시�론과 시뮬의 격차)를 구조적으로 해결하는 전략이다.

## 관련 논문
- sources/2026-05-27-discoverphysics-benchmarking-llms-for-out-of-the-box-scientific.md

---

# sandbox-liveworld-gap
**카테고리**: 미분류
**생성일**: 2026-04-16
## 정의
통제된 샌드박스 벤치마크에서의 에이전트 성능·안전성 검증 결과가 실제 라이브 환경 배포 시 급격히 저하되는 현상. DiscoverPhysics가 이 간극에 대한 하나의 해결책을 제시한다—표준 물리를 비표준과 다른 물리로 대체하여 생성한 22개의 세계에서 에이전트의 제1원리 추론을 테스트함으로써, 시뮬론의 '힌'을 정보가 아닌 '환경'으로 치환하여 검증과 환경 간극을 동시에 해소한다.

## 관련 논문
- sources/2026-05-27-discoverphysics-benchmarking-llms-for-out-of-the-box-scientific.md

---

# scientific-finding-reproducibility
**카테고리**: 미분류
**생성일**: 2026-05-27
## 정의
동일한 연구 질문을 재현하는 것이 아니라, 근본적으로 다른 물리 법칙 구조를 가진 22개 세계에서 동일한 발견 과정이 재현되는지를 검증함으로써, 재현성의 개념를 '동일 결과의 재현'에서 '동일 과정의 재현'으로 격상함. 기존 sources/2026-05-05-can-coding-agents-reproduce-findings-in-computatio.md가 재현 가능성의 실증을 요구하던 문제에 대한 구조적 해법을 제공한다.

## 관련 논문
- sources/2026-05-27-discoverphysics-benchmarking-llms-for-for-out-of-the-box-scientific.md

---

## 🏷️ 엔티티

- [[entities/counterfactual-physics-reasoning.md|counterfactual-physics-reasoning]]
- [[entities/sandbox-liveworld-gap.md|sandbox-liveworld-gap]]
- [[entities/scientific-finding-reproducibility.md|scientific-finding-reproducibility]]

---
_LLM 분석으로 생성됨_
