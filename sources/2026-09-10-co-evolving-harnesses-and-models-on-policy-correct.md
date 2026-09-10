# Co-Evolving Harnesses and Models: On-Policy Correction Helps Weaker Models Catch Up Where Imitation Fails

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-10
**링크**: http://arxiv.org/abs/2609.09134v1

## 💡 핵심 인사이트

하네스 진화와 모델 파인튜닝의 결합은 학습 방법이 모델 강도에 조건부임을 요구한다 — 교사 모방이 실패하는 약한 모델 영역에서, 진화된 하네스 하의 온폴리시 정정만이 따라잡기를 가능하게 한다.

## 📖 분석

이 논문은 에이전트 하네스(시스템 프롬프트, 도구 집합, 실행 훅, 컨텍스트 관리 스캐폴딩)와 모델 가중치의 공진화를 능력·비용 도메인에서 통제 실험한다. 7개 엔터프라이즈 태스크에서 하네스 진화만으로 소형 모델이 프론티어 비용의 일부로 도메인 태스크를 수행함을 보이고, '하네스 진화와 경량 파인튜닝을 어떻게 결합할 것인가'에 대해 모방이 실패하는 약한 모델 영역에서 온폴리시 정정이 따라잡기를 가능하게 함을 실증한다.

Wiki 맥락에서 본 논문은 [[harness-model-co-evolution]]의 능력 도메인 확장이다. SafeEvolve([[harness-policy-co-evolution]])가 안전 정렬을 위한 공진화를 제안했다면, 본 논문은 동일 구조가 비용 효율적 능력 확장에서도 작동함을 보여 공진화가 목표 불문 원리임을 강화한다. [[harness-side-compensation]]의 최대 규모 실증이기도 하다 — 단일 기능 오프로딩(SENTINEL-RL)을 넘어 하네스 전체의 진화적 재설계만으로 소형 모델이 프론티어급 수행에 도달한다.

핵심 발견은 학습 방법 선택이 모델 강도에 조건부라는 점이다. 교사 궤적 모방은 약한 모델이 흡수하지 못해 실패하지만, 진화된 하네스 하에서 모델 자신의 행동 분포 내 정정 학습은 성공한다. 이는 [[on-policy-environment-coupling]]의 훈련 측 실증이며 [[harness-native-training]]의 완전한 실현 사례다. [[slm-reasoning-gap]]에는 선택·증류에 이은 제3의 해법 경로를 연다.

## 🔗 관련 논문

- SafeEvolve: Harness-Policy Co-Evolution from Agent Experienc
- Environment Evolution for Terminal Agents
- Distill Globally, Adapt Locally: Reasoning Distillation and Product-Ty
- Agentic Harness Engineering: Observability-Driven Automatic 
- Select to Think: Unlocking SLM Potential with Local

## 🏷️ 엔티티

- [[entities/harness-model-co-evolution.md|harness-model-co-evolution]]
- [[entities/harness-side-compensation.md|harness-side-compensation]]
- [[entities/harness-native-training.md|harness-native-training]]
- [[entities/slm-reasoning-gap.md|slm-reasoning-gap]]
- [[entities/agentic-harness-engineering.md|agentic-harness-engineering]]

## 📐 개념

- [[concepts/harness-policy-co-evolution.md|harness-policy-co-evolution]]
- [[concepts/safeevolve.md|safeevolve]]
- [[concepts/on-policy-environment-coupling.md|on-policy-environment-coupling]]
- [[concepts/sft-rl-budget-allocation.md|sft-rl-budget-allocation]]
- [[concepts/dual-axis-alignment-dispersion.md|dual-axis-alignment-dispersion]]

---
_LLM 분석으로 생성됨_
