# Trust-Aware Adaptive Disclosure for Inference Privacy Preservation in Multi-Agent Networks

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-08
**링크**: http://arxiv.org/abs/2609.05340v1

## 💡 핵심 인사이트

신뢰 수준을 메시지 공개의 런타임 제어 변수로 삼으면, 합의에 필요한 조율과 잠재 목표의 추론 공격 방어를 동일한 통신 채널에서 동시에 최적화할 수 있다.

## 📖 분석

## 핵심 기여

의료 관리·스마트 그리드 등 정보 중요 도메인의 네트워크드 다중 에이전트 시스템에서, 각 에이전트의 잠재 목표를 통신 관찰 적대자로부터 보호하면서 합의(consensus)를 달성하는 프레임워크를 제시한다. Trust-Aware Privacy Control은 신뢰 수준에 따라 메시지 공개 범위를 적응적으로 조절한다.

## Wiki 맥락

[[latent-inter-agent-communication]]이 '얼마나 공유해야 능력이 향상되는가'를 다뤘다면, 본 논문은 '얼마나 숨겨야 목표가 보호되는가'를 다루어 통신 공개 제어의 양면을 완성한다. [[zero-knowledge-negotiation]]이 암호학적 증명으로 완전 비공개 합의를 달성하는 극단 경로라면, 본 논문은 신뢰에 비례한 점진적 공개라는 연속체 상의 중간 지점을 제공한다. [[information-preservation-boundary]]의 '각 에이전트가 독립 유지해야 할 정보 범위'를 잠재 목표로 구체화하고, 고정 설계 원칙을 신뢰의 함수로 동적 조정 가능한 대상으로 재정의한다. [[differential-privacy]]의 정적 통계적 난독화와 대비되는, 상호작용 이력에 따라 갱신되는 동적 신뢰 기반 보장이다. [[communication-increase-paradox]]에 '통신량 증가가 목표 추론 공격 표면을 확대한다'는 보안 축을 추가한다.

## 새 개념 제안

- **goal-inference-attack**: 통신 관찰로부터 잠재 목표를 역추론하는 공격 클래스
- **trust-aware-adaptive-disclosure**: 신뢰를 공개 수준의 제어 변수로 삼는 적응 메커니즘
- **privacy-coordination-tension**: 합의 통신 필요량과 목표 은닉 요구 간의 구조적 긴장

## 🔗 관련 논문

- Learning to Communicate: Toward End-to-End Optimization of M
- Differential Privacy in Generative AI Agents: Analysis and O

## 🏷️ 엔티티

- [[entities/multi-agent-system.md|multi-agent-system]]
- [[entities/latent-inter-agent-communication.md|latent-inter-agent-communication]]
- [[entities/differential-privacy.md|differential-privacy]]
- [[entities/zero-knowledge-negotiation.md|zero-knowledge-negotiation]]
- [[entities/information-preservation-boundary.md|information-preservation-boundary]]
- [[entities/trust-domain-scale-stratification.md|trust-domain-scale-stratification]]
- [[entities/communication-increase-paradox.md|communication-increase-paradox]]
- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/goal-inference-attack.md|goal-inference-attack]]
- [[entities/trust-aware-adaptive-disclosure.md|trust-aware-adaptive-disclosure]]
- [[entities/privacy-coordination-tension.md|privacy-coordination-tension]]

## 📐 개념

- [[concepts/inference-privacy.md|inference-privacy]]
- [[concepts/trust-conditioned-information-flow.md|trust-conditioned-information-flow]]
- [[concepts/latent-goal-confidentiality.md|latent-goal-confidentiality]]
- [[concepts/consensus-under-adversarial-observation.md|consensus-under-adversarial-observation]]

---
_LLM 분석으로 생성됨_
