# S1-Evo: Experience-Guided Evidence Competition Attacks on Typed System-1 Decision Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-14
**링크**: http://arxiv.org/abs/2611.16937v1

## 💡 핵심 인사이트

S1/S2 아키텍처 분할은 추론 비용 절감 수단인 동시에 위협 모델의 분기점이다 — 자기회귀 모델용 공격은 타이핑된 결정 계약에 전이되지 않으며, 결정 모델의 고정 스코어링 인터페이스 자체가 별도의 공격 최적화 대상이 된다.

## 📖 분석

S1-Evo는 LLM 에이전트의 추론 비용 절감을 위해 배포되는 Typed System-1(S1) 결정 모델(라우팅·모더레이션·권한 부여)에 대한 자기 진화적 공격 프레임워크를 제시한다.

핵심 발견은 S1/S2 아키텍처 분할이 공격 표면의 분기를 수반한다는 점이다. S1 인터페이스는 토큰 단위 디코딩 없이 동적 규칙과 옵션을 스코어링하므로, 자기회귀 S2 모델을 겨냥한 공격(텍스트 연속성 조작·명시적 오버라이드 명령)은 S1에 전이되지 않는다. 대신 S1-Evo는 컨텍스트 내 증거 경쟁(evidence competition)으로 타이핑된 출력 계약을 조작해 실행 분기를 탈취한다.

Wiki 관점에서 본 논문은 세 축을 연결한다. (1) [[dual-primitive-serving]]이 규정한 System One/Two 이원 원시 연산이 방어 관점에서도 이질적 위협 모델을 요구함을 보인다. (2) [[decision-model]] 계보(DecisionRank 증류 → Flide 서빙)에 적대 차원이 추가되어 결정 모델 라이프사이클이 구축→서빙→공방으로 확장됨을 시사한다. (3) [[efficiency-attack-surface-identity]]의 확장으로서 S1의 효율 구조(고정 출력 클래스·계약 기반 스코어링)가 그 자체로 공격 최적화의 표면이 됨을 입증한다. [[routing-adversarial-hijacking]]과 [[selection-metric-manipulation]]의 발견이 결정 모델 계층으로 특화되는 사례이며, [[compilation-as-offline-commitment]]의 배포 전 고정 계약이 공격자의 사전 최적화를 가능하게 하는 이중성도 드러난다.

## 🔗 관련 논문

- DecisionRank: On-Policy Distillation for Decision-Model Rerankers
- Flide: Accelerating Decision Inference with Exact State Forking

## 🏷️ 엔티티

- [[entities/decision-model.md|decision-model]]
- [[entities/dual-primitive-serving.md|dual-primitive-serving]]
- [[entities/decision-model-serving.md|decision-model-serving]]
- [[entities/dual-process-agent.md|dual-process-agent]]
- [[entities/selection-metric-manipulation.md|selection-metric-manipulation]]
- [[entities/efficiency-attack-surface-identity.md|efficiency-attack-surface-identity]]
- [[entities/routing-adversarial-hijacking.md|routing-adversarial-hijacking]]
- [[entities/compilation-as-offline-commitment.md|compilation-as-offline-commitment]]
- [[entities/self-evolving-framework-taxonomy.md|self-evolving-framework-taxonomy]]
- [[entities/adversarial-problem-generation.md|adversarial-problem-generation]]
- [[entities/exact-state-forking.md|exact-state-forking]]
- [[entities/s1-s2-attack-surface-divergence.md|s1-s2-attack-surface-divergence]]
- [[entities/evidence-competition-attack.md|evidence-competition-attack]]

## 📐 개념

- [[concepts/s1-s2-attack-surface-divergence.md|s1-s2-attack-surface-divergence]]
- [[concepts/evidence-competition-attack.md|evidence-competition-attack]]
- [[concepts/decision-contract-exploitation.md|decision-contract-exploitation]]

---
_LLM 분석으로 생성됨_
