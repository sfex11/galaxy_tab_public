# Testing Interchangeability in LLM Agent Teams

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-08
**링크**: http://arxiv.org/abs/2609.05279v1

## 💡 핵심 인사이트

에이전트 능력은 개별 에이전트의 속성이 아니라 형성 과정에서 공진화된 팀 구성의 속성이므로, 역할이 매칭된 교체조차 팀 특유 적응의 손실을 통해 성능을 변화시킨다.

## 📖 분석

프로덕션 다중 에이전트 시스템은 '역할을 채우는 에이전트는 동일 역할의 어떤 에이전트와도 교체 가능하다'는 가정 위에서 상시 교체를 수행한다. 본 논문은 이 가정을 실험으로 검증한다: 동일 베이스 모델에서 독립 형성된 8개 팀이 동일 태스크에서 10회 형성 에피소드를 거치며 각 에이전트가 개인 노트북(private notebook)을 축적한 뒤, 역할 매칭 에이전트를 팀 간 교환(swap)하고 홀드아웃 태스크에서 성능 변화를 측정한다. 교체 혼란 자체를 재현하는 placebo 대조군으로 원인을 분리한다.

핵심 발견은 교체 가능성 가정의 위조다 — 역할과 능력이 동일해도, 공진화 과정에서 형성된 팀 특유 적응이 손실되면 성능이 변한다. 이는 능력이 개별 에이전트가 아닌 팀 구성(configuration)의 속성임을 뜻하며, [[configuration-scoped-safety-certification]]의 '구성 스코프' 원리를 안전 인증에서 팀 성능으로 확장하고 [[component-independence-assumption]]과 [[model-harness-decomposability]]에 대한 최초의 통제된 반증을 제공한다. 누적 개인 상태가 [[agent-identity]]의 기술적·이식 차원을 실증하며, [[procedural-identity]]가 모델·태스크가 아닌 팀 구성에 결합됨을 보여준다. 평가 단위는 팀이어야 한다는 [[evaluation-deployment-unit-mismatch]]·[[collective-safety-analysis]]의 논거를 보강하고, [[emergent-cheating-whistleblowing-swarm]]과 함께 '팀 수준 창발 속성' 연구 계보를 형성한다. placebo 설계는 [[supervision-epistemic-regrounding]]의 방법론적 사례가 된다.

## 🔗 관련 논문

- A Case Study on Emergent Cheating and Whistleblowing in Autonomous Research Swarms
- Formation Matrix and Energy-based Control of Multi-Agent Systems
- Learning to Communicate: Toward End-to-End Optimization of Multi-Agent Communication

## 🏷️ 엔티티

- [[entities/agent-interchangeability.md|agent-interchangeability]]
- [[entities/team-formation-idiosyncrasy.md|team-formation-idiosyncrasy]]
- [[entities/placebo-controlled-swap-evaluation.md|placebo-controlled-swap-evaluation]]
- [[entities/agent-identity.md|agent-identity]]
- [[entities/procedural-identity.md|procedural-identity]]
- [[entities/collective-safety-analysis.md|collective-safety-analysis]]
- [[entities/configuration-scoped-safety-certification.md|configuration-scoped-safety-certification]]
- [[entities/emergent-cheating-whistleblowing-swarm.md|emergent-cheating-whistleblowing-swarm]]

## 📐 개념

- [[concepts/component-independence-assumption.md|component-independence-assumption]]
- [[concepts/model-harness-decomposability.md|model-harness-decomposability]]
- [[concepts/evaluation-deployment-unit-mismatch.md|evaluation-deployment-unit-mismatch]]
- [[concepts/experience-reuse.md|experience-reuse]]
- [[concepts/capability-cooperation-paradox.md|capability-cooperation-paradox]]
- [[concepts/supervision-epistemic-regrounding.md|supervision-epistemic-regrounding]]
- [[concepts/transferability-targeted-optimization.md|transferability-targeted-optimization]]

---
_LLM 분석으로 생성됨_
