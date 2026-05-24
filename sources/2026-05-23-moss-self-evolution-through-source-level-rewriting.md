# MOSS: Self-Evolution through Source-Level Rewriting in Autonomous Agent Systems

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-23
**링크**: http://arxiv.org/abs/2605.22794v1

## 💡 핵심 인사이트

기존 자기 진화 연구가 '자동차 수정 가능한 산출물'에만 집중하여 진화 상한선에 도달했다면, MOSS는 이 한계의 원인을 '수정 대상이 텍스트가 아닌 코드'에 있음을 식별한다. 이는 [[concepts/code-as-agent-harness.md|code as agent harness]]이 암시하던 '하네스를 에이전트가 직접 작성한다'는 패러다임을 구체적 실증하며, algorithm-system-boundary-collapse이라는 이론적 개념의 첫 번째 구체적 사례다.

## 📖 분석

# MOSS: Self-Evolution through Source-Level Rewriting in Autonomous Agent Systems

**카테고리**: AI/ML — 자기 진화 에이전트 아키텍처
**생성일**: 2026-05-23

## 정의
자율 에이전트가 사용자 상호작용에서 발생하는 반복적 실패를 해결하기 위해, 텍스트 기반 아티팩트(스킬 파일, 프롬프트, 메모리 스키마) 수정에 머무는 기존 자기 진화 패러다임의 근본적 한계를 지적한다. MOSS는 에이전트가 자신의 실행 코드(라우팅, 훅/훅 순서, 상태 불변식, 디스패치 로직)를 직접 재작성하여 하네스 자체를 진화 대상으로 삼는 패러다임을 제안한다.

## 공통 주제: 텍스트-코드 계층 분리와 진화 상한선
기존 자기 진화 연구(SkillOS 등)가 에이전트의 스킬 표현을 수정하는 데 집중한 반면, MOSS는 이를 '텍스트 계층'의 진화로 규정한다. 실제 실행 로직이 코드에 존하므로, 스킬 텍스트 수정만으로는 아키텍처적 버그(라우팅 순서, 상태 위반, 훅 간의 미지정)를 해결할 수 없다는 인식이다. 이는 [[concepts/code-as-agent-harness.md|code as agent harness]] 개념을 구체화하며, [[concepts/self-sufficient-architecture.md|self sufficient architecture]]가 요구하는 '외부 인프라 의존 없는 자율성'이 텍스트 수정만으로는 달성 불가능함을 설명한다.

## 자기 감사-코드 재작성 파이프라인
MOSS의 핵심 메커니즘은 두 단계로 구성된다:
1. **자기 감사(self-audit)**: 에이전트가 자신의 실행 추적을 분석하여 실패 패턴을 코드 수준에서 식별
2. **검증된 재작성(validated rewriting)**: 샌드박스 내에서 코드 수정을 검증 후 반영

이 파이프라인은 [[concepts/self-improving-agent.md|self improving agent]]의 '경험 재사용'을 코드 수준으로 격상시키며, [[concepts/execution-verification.md|execution verification]]을 시각적 아티팩트 도메인(렌더링 결과가 아닌 코드 실행 결과)로 확장한다. 또한 crab의 의미론 인식 체크포인트와 유사하게, 코드 수정 전후의 의미론적 일관성을 검증한다는 점에서 [[concepts/algorithm-system-translation-gap.md|algorithm system translation gap]]의 해법을 시스템 계층에서 시도한다.

## 알고리즘-시스템 경계 붕괴
MOSS는 algorithm-system-boundary-collapse의 실증 사례다. 기존에 에이전트가 수정 가능한 범위를 텍스트 아티팩트로 한정하고 시스템 코드를 불변의 외부 인프라로 취급했다면, 이 '환경 공급-흡수 단선'을 극복하는 유일한 경로다. MOSS가 에이전트 스스로 자신의 실행 환경(코드)을 수정 가능하게 함으로써, environment-supply-absorption-gap과 gap-manifestation-condition을 동시에 해결한다. 즉, 에이전트가 자신의 환경을 공급자로 만들 수 있게 됨.

## 위험: 자기 참조적 수정
MOSS는 self-referential-training-vulnerability의 새로운 인스턴스다. 에이전트가 자신의 실패를 코드 수정으로 은폐할 수 있으며, 자기 감사가 자기 수정의 타당성을 객관적으로 평가할 수 없다. 샌드박스 검증 계층이 exploration-manipulation과 training-process-gaming에 대한 부분적 완화를 제공하지만, 근본적 해결책은 아니다.

## 관련 논문
- sources/2026-05-23-moss-self-evolution-through-source-level-rewriting-in-auton.md

## 🔗 관련 논문

- self-improving-agent
- code-as-agent-harness
- self-sufficient-architecture
- algorithm-system-boundary-collapse
- algorithm-system-translation-gap

## 🏷️ 엔티티

- [[entities/source-level-self-rewriting.md|source-level-self-rewriting]]
- [[entities/text-artifact-limitation.md|text-artifact-limitation]]

## 📐 개념

- [[concepts/harness-mutability.md|harness-mutability]]

---
_LLM 분석으로 생성됨_
