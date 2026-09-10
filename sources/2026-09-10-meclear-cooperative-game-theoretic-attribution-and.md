# MeClear: Cooperative Game-Theoretic Attribution and Risk-Aware Memory Clearance for Long-Horizon LLM Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-10
**링크**: http://arxiv.org/abs/2609.09115v1

## 💡 핵심 인사이트

메모리 검색의 semantic compatibility 최적화는 downstream utility와 무관하며, 협력적 게임이론 귀속으로 기억별 음의 기여도를 식별하면 망각이 회복 불가능한 손실이 아닌 위험을 정량화할 수 있는 검증 가능한 최적화가 된다.

## 📖 분석

## MeClear: 협력적 게임이론 귀속과 위험 인지 메모리 정리

Long-horizon LLM 에이전트의 외부 메모리에서 downstream utility가 음수인 기억을 식별·제거하는 task-conditioned clearance 프레임워크. 협력적 게임이론 attribution으로 각 기억의 태스크 기여도를 산정하고, risk-aware하게 정리한다.

### 기존 Wiki와의 관계

**1. [[value-differential-memory-management]]의 게임이론적 구현**: 기억 가치를 차등 평가하라는 추상적 패러다임에 구체적 메커니즘을 제공한다. 가치 평가를 협력적 게임이론 귀속으로 형식화하여, 기억의 가치가 태스크 조건부이며 음수일 수 있음을 조작적으로 정의한다.

**2. [[deletion-non-monotonicity]]의 체계적 해법**: '삭제할수록 점수가 오르는 역설'의 원인을 semantic-compatible하지만 utility-음수인 기억의 컨텍스트 오염으로 진단한다. 귀속 기반 선별은 역선택을 검증 가능한 최적화로 전환한다.

**3. [[utility-ontological-mislocation]]의 실증**: 검색이 최적화하는 semantic compatibility와 downstream utility의 분리를 보여, 유용성이 기억-질의 쌍의 정적 속성이 아닌 추론 체인 전체에 분산된 인과적 속성임을 뒷받침한다.

**4. [[adaptive-forgetting-as-function]]·[[forgetting-as-agent-decision]]의 통합**: 기능적 망각에 '누가·무엇을·얼마나 위험하게'라는 귀속 계층과 위험 제약을 추가한다.

**5. [[credit-assignment-granularity]]의 대상 확장**: 크레딧 할당 대상을 행동·토큰에서 외부 기억 단위로 확장한다.

'Cooperative'가 협력적 게임이론을 지칭한다는 점에서 [[cooperative-forgetting]](사회적 딜레마)과 어원이 다르지만, 두 개념 모두 망각을 전략적 선택으로 취급한다는 점에서 수렴한다.

## 🔗 관련 논문

- Does Your Agent's Memory Survive a Model Upgrade? A Controlled Stu
- User Feedback Provides a Unique Signal that LLMs Can not Det

## 🏷️ 엔티티

- [[entities/memory-management.md|memory-management]]
- [[entities/value-differential-memory-management.md|value-differential-memory-management]]
- [[entities/deletion-non-monotonicity.md|deletion-non-monotonicity]]
- [[entities/utility-ontological-mislocation.md|utility-ontological-mislocation]]
- [[entities/adaptive-forgetting-as-function.md|adaptive-forgetting-as-function]]
- [[entities/forgetting-as-agent-decision.md|forgetting-as-agent-decision]]
- [[entities/credit-assignment-granularity.md|credit-assignment-granularity]]
- [[entities/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[entities/cooperative-memory-attribution.md|cooperative-memory-attribution]]

## 📐 개념

- [[concepts/task-conditioned-memory-clearance.md|task-conditioned-memory-clearance]]
- [[concepts/risk-aware-forgetting.md|risk-aware-forgetting]]
- [[concepts/semantic-utility-divergence.md|semantic-utility-divergence]]
- [[concepts/negative-downstream-utility.md|negative-downstream-utility]]

---
_LLM 분석으로 생성됨_
