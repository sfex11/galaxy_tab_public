# From Model Scaling to System Scaling: Scaling the Harness in Agentic AI

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-27
**링크**: http://arxiv.org/abs/2605.26112v1

## 💡 핵심 인사이트

모델 스케일링에 국한된 법침의 한계에 도달한 것이라는 하네스 스케일링은 제2의 스케일링 축을 제안한다. 모델이 아무리 커질 수 있더라도 하네스 설계에 따라 시스템 전체의 능력 천장이 결정된다는 구조적 주장을 제공한다.

## 📖 분석

# system-scaling

**카테고리**: 미분류
**생성일**: 2026-05-27

## 정의
에이전트 AI 연구에서 모델 스케일링에 집중되어 오�려왔던 스케일링 패러다임에서 벗어나 기반 모델을 래핑하는 구조화된 실행 계층(하네스)를 독자적인 설계·평가·최적화의 일차 대상으로 격상하는 패러다임 전환. 하네스를 기반 모델의 외부 인프라가가 아닌 '인프라 세부'로 취급하지 않고, 에이전트 시스템의 핵심 능력 천장을 결정하는 일차 설계 대상이다.

## 핵심 속성
하네스의 4가지 스케일링 속성:
1. **감사 가능성(Auditability)**: 시스템 내부에서 무엇이, 왜 배경에서 발생했는지 추적 가능한 구조
2. **지속성(Persistence)**: 롤백, 분기, 전환 간 상태의 의미론적 무결성을 보존
3. **모듈성(Modularity)**: 모놀식 하네스를 독립적으로 검증·교체 가능한 모듈로 분해
4. **검증 가능성(Verifiability)**: 단일 모델 능력이 아닌 하네스 효과만으로 인해를 숨기하는 것인지 검증 가능한 구조

## 관련 논문
- sources/2026-05-27-from-model-scaling-to-system-scaling-scaling-the-harness-in-agentic.md

### From Model Scaling to System Scaling: Scaling the Harness in Agentic AI (2026-05-27)


## 🏷️ 엔티티

- [[entities/system-scaling.md|system-scaling]]

## 📐 개념

- [[concepts/auditability-as-scaling-requirement.md|auditability-as-scaling-requirement]]
- [[concepts/persistence-as-scaling-property.md|persistence-as-scaling-property]]
- [[concepts/modularity-as-scaling-strategy.md|modularity-as-scaling-strategy]]
- [[concepts/verifiability-as-scaling-proof.md|verifiability-as-scaling-proof]]

---
_LLM 분석으로 생성됨_
