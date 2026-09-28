# User Model Extraction via Belief Self-Distillation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-29
**링크**: http://arxiv.org/abs/2609.31603v1

## 💡 핵심 인사이트

LLM의 사용자에 대한 암묵적 신념은 동결 모델의 자기 증류만으로 선형 디코딩 가능하면서 인과적 재주입 가능한 단일 컴팩트 표현으로 추출되며, 판독과 조작이 동일 프레임워크에서 통합됨을 보여준다.

## 📖 분석

# User Model Extraction via Belief Self-Distillation (2026-09-29)

LLM이 대화에서 암묵적으로 형성하는 사용자 신념을, 동결 모델이 자기 교사가 되어 외부 주석 없이 컴팩트한 잠재 표현으로 추출하고(Belief Self-Distillation, BSD), 그 표현을 재주입해 행동을 인과적으로 조작하는 read-write 통합 프레임워크.

## 기존 Wiki 논의와의 관계

**판독-기록 통합의 실증**: [[steering-read-manipulation-duality]]와 [[read-write-symmetry]]가 예측한 대칭성의 사용자 신념 버전이다. 동일한 표현이 디코딩(판독)과 재주입(조작) 양쪽에 작동하며, 판독 가능성이 곧 조작 가능성임을 확정한다.

**신념 계층의 제2 경로**: [[explicit-belief-layer]]가 신념을 외부 아키텍처 구성요소로 승격했다면, BSD는 신념을 모델 내부 표현에서 추출해 조작 가능한 형태로 격상시키는 내재적 경로를 연다.

**ToM의 연산화 심화**: [[theory-of-mind]] 흐름에 이어 사용자 모델이 선형 디코딩 가능·인과 주입 가능한 잠재 변수임을 실증한다.

**동결 모델 유도의 확장**: [[router-within]]의 스킬 라우팅, [[frozen-model-external-memory-contradiction]]의 지식에 이어 '모델이 사용자에 대해 믿는 것'까지 자기 증류로 추출 가능함을 확장한다.

## 보안 시사점

사용자 신념의 판독 가능성은 악의적 쓰기(신념 조작)의 표면이기도 하다. 개인화 시스템에서 신념 벡터 조작은 [[sycophancy]] 증폭·사용자 인식 왜곡의 새 공격 벡터가 될 수 있다.

## 방법론적 기여

선형 프로빙(상관)과 인과 프로빙(개입)을 단일 자기 증류 프레임워크로 다리며, [[causal-mechanistic-interpretability]]의 판독-개입 통합 방향에 구체적 경로를 제공한다.

## 🔗 관련 논문

- Bayesian Belief Layer for Controllable Opinion Dynamics in LLM Agents
- Mind2Dialogue: Training Human-Aware Language Models by Simulating User
- The Router Within: Eliciting Native Skill Routing from a Frozen LLM
- Measuring LLM Sycophancy under Sustained Multi-Turn Pressure

## 🏷️ 엔티티

- [[entities/belief-self-distillation.md|belief-self-distillation]]
- [[entities/steering-read-manipulation-duality.md|steering-read-manipulation-duality]]
- [[entities/explicit-belief-layer.md|explicit-belief-layer]]
- [[entities/theory-of-mind.md|theory-of-mind]]
- [[entities/read-write-symmetry.md|read-write-symmetry]]
- [[entities/causal-mechanistic-interpretability.md|causal-mechanistic-interpretability]]
- [[entities/frozen-model-external-memory-contradiction.md|frozen-model-external-memory-contradiction]]
- [[entities/router-within.md|router-within]]
- [[entities/sycophancy.md|sycophancy]]
- [[entities/personal-ai-agent.md|personal-ai-agent]]

## 📐 개념

- [[concepts/read-write-symmetry.md|read-write-symmetry]]
- [[concepts/steering-read-manipulation-duality.md|steering-read-manipulation-duality]]
- [[concepts/user-belief-representability.md|user-belief-representability]]
- [[concepts/implicit-user-model.md|implicit-user-model]]

---
_LLM 분석으로 생성됨_
