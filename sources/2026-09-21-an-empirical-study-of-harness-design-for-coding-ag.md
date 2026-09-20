# An Empirical Study of Harness Design for Coding Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-21
**링크**: http://arxiv.org/abs/2609.20804v1

## 💡 핵심 인사이트

하네스를 고정 실행 루프 위의 교체 가능 구성요소(계획·행동 공간·컨텍스트 관리)로 분해하고 4개 모델에 걸쳐 절제 실험함으로써, 코딩 에이전트 하네스 연구를 단일 시스템의 블랙박스 평가에서 구성요소별 기여도의 인과적 측정으로 전환한다.

## 📖 분석

## 핵심 기여

자율 코딩 에이전트의 롱호라이즌 성능이 모델 능력을 번역하는 계층인 하네스에 의해 좌우됨에도, 기존 연구는 하네스를 단일 시스템으로 평가하여 개별 구성요소의 효과를 파악하지 못했다. 본 논문은 실행 루프를 고정한 채 계획(planning), 행동 공간(action space), 컨텍스트 관리(context management)의 3개 구성요소만 변이하는 경량 하네스로 구성요소 수준 비교를 실현하고, 4개 모델에 걸쳐 동일 변이를 반복하는 절제 실험으로 구성요소별 기여도를 인과적으로 분리한다.

## 기존 Wiki와의 관계

- [[harness-engineering]]: 관측성 기반 자동 진화([[observability-driven-evolution]])가 하네스를 블랙박스 최적화 대상으로 다뤘다면, 본 논문은 그 탐색 공간을 3축으로 명시화하여 자동 진화 연구가 다뤄야 할 설계 축의 정의에 근거를 부여한다.
- [[fixed-loop-component-ablation]]: 본 논문의 방법론적 핵심이다. 루프 고정 + 구성요소 변이 설계는 [[harness-as-hidden-variable]]의 혼동 효과를 통제하는 실험적 해법으로, 하네스 효과를 처음으로 구성요소 단위로 귀속 가능하게 한다.
- [[component-independence-assumption]]: 구성요소 독립성을 가정이 아닌 측정 대상으로 전환한다. 변이 효과의 조건별 차이는 구성요소 간 상호작용을 관찰 가능하게 한다.
- [[harness-design-combinatorics]]: 3축 조합 공간을 실증적으로 탐색하는 첫 사례로, 어떤 구성요소 조합도 지배적이지 않다는 조합적 폭발 진단의 검증 무대를 제공한다.
- [[system-scaling]]: 4개 모델 반복 설계로 하네스 원칙이 모델 규모와 독립적인지(이식 가능한 원칙) 아니면 규모 조건부인지(구성별 최적화 필요)를 판별하는 토대를 마련한다.

## 연결점

[[agentic-harness-engineering]]의 자동 진화, [[clawgym]]의 진단적 평가, [[swe-chat]]의 실사용 세션 분석과 함께 하네스 연구의 측정→설계→검증 루프를 완성한다. 모델 능력이 동일해도 하네스 구성이 성능을 결정할 수 있다는 이 연구의 전제는 [[model-harness-decomposability]]의 실증적 기초가 된다.

## 🔗 관련 논문

- Agentic Harness Engineering: Observability-Driven Automatic Evolution
- ClawGym: A Scalable Framework for Building Effective Claw Agents
- SWE-chat: Coding Agent Interactions From Real Users in the Wild
- From Model Scaling to System Scaling: Scaling the Harness

## 🏷️ 엔티티

- [[entities/harness-engineering.md|harness-engineering]]
- [[entities/llm-agent.md|llm-agent]]
- [[entities/system-scaling.md|system-scaling]]

## 📐 개념

- [[concepts/fixed-loop-component-ablation.md|fixed-loop-component-ablation]]
- [[concepts/component-independence-assumption.md|component-independence-assumption]]
- [[concepts/harness-design-combinatorics.md|harness-design-combinatorics]]
- [[concepts/harness-as-hidden-variable.md|harness-as-hidden-variable]]
- [[concepts/model-harness-decomposability.md|model-harness-decomposability]]
- [[concepts/harness-task-matching-bottleneck.md|harness-task-matching-bottleneck]]

---
_LLM 분석으로 생성됨_
