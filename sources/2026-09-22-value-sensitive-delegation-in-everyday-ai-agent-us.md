# Value-Sensitive Delegation in Everyday AI Agent Use: Evidence from OpenClaw

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-22
**링크**: http://arxiv.org/abs/2609.22067v1

## 💡 핵심 인사이트

에이전트 평가의 표적은 태스크 완성도가 아니라 사용자가 실제로 중시하는 가치(도달 범위 제한, 검토 가능성, 신뢰 가능한 운영)이며, 이 가치 지형은 야생 사용자 데이터의 체계적 분석으로 측정 가능하다.

## 📖 분석

본 논문은 Value Sensitive Design 프레임워크로 [[openclaw]] 실사용자 73,093건의 1인칭 레딧 게시물을 LLM 보조 분석하여, 태스크 완성도가 아닌 사용자가 중시하는 가치를 평가 대상으로 삼는다. 21개 가치가 6개 그룹(Autonomous·Dependable·Affordable Operation, Bounded Reach, Reviewability, Equitable Access)으로 조직화된다.

Wiki 관점의 기여는 세 층위다. 첫째, 평가-가치 간극: 평가 체계가 태스크 완성도를 측정하는 동안 사용자는 Bounded Reach·Reviewability 같은 가치를 우선하며, 이는 [[benchmark-specification-gap]]의 사용자 중심 확장으로 벤치마크 명세 자체가 사용자의 실제 관심사를 담지 못함을 진단한다. 둘째, 기술 개념의 가치 축 검증: Bounded Reach는 [[capability-safety-inseparability]]와 샌드박스 논의가 다룬 기술적 제한이 사용자의 1급 가치로 상향됨을, Reviewability는 [[dual-readership-interface]]와 [[auditability-as-scaling-requirement]]의 구조가 사용자 측 요구이기도 함을 실증한다. 셋째, 방법론: 야생 사용자 게시물의 구조화된 가치 추출은 SWE-chat·copying 계열의 [[in-the-wild-agent-dataset]] 관찰 패러다임을 가치 연구로 확장하며, [[user-feedback-signal]]이 LLM 판독 가능한 신호로 변환될 수 있음을 보여준다.

## 🔗 관련 논문

- A Systematic Security Evaluation of OpenClaw and Its Variants
- SWE-chat: Coding Agent Interactions From Real Users in the Wild
- Copying explains the collective behavior of AI agents in the wild

## 🏷️ 엔티티

- [[entities/openclaw.md|openclaw]]
- [[entities/benchmark-specification-gap.md|benchmark-specification-gap]]
- [[entities/capability-safety-inseparability.md|capability-safety-inseparability]]
- [[entities/dual-readership-interface.md|dual-readership-interface]]
- [[entities/auditability-as-scaling-requirement.md|auditability-as-scaling-requirement]]
- [[entities/in-the-wild-agent-dataset.md|in-the-wild-agent-dataset]]
- [[entities/user-feedback-signal.md|user-feedback-signal]]
- [[entities/human-oversight.md|human-oversight]]
- [[entities/personal-ai-agent.md|personal-ai-agent]]
- [[entities/trust-in-automation.md|trust-in-automation]]

## 📐 개념

- [[concepts/value-sensitive-agent-evaluation.md|value-sensitive-agent-evaluation]]
- [[concepts/user-value-taxonomy.md|user-value-taxonomy]]
- [[concepts/bounded-reach-value.md|bounded-reach-value]]
- [[concepts/reviewability-value.md|reviewability-value]]

---
_LLM 분석으로 생성됨_
