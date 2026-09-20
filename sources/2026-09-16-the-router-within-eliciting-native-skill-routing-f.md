# The Router Within: Eliciting Native Skill Routing from a Frozen LLM

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-16
**링크**: http://arxiv.org/abs/2609.15982v1

## 💡 핵심 인사이트

동결된 LLM의 순방향 연산에 스킬 선택 신호가 이미 내재하여, 스킬 라우팅은 외부 메타데이터 주입이나 검색 파이프라인이 아니라 모델 내부 상태의 선형 판독 문제로 환원된다.

## 📖 분석

The Router Within은 스킬 라우팅의 위치를 외부 하네스에서 동결된 모델의 내부 순방향 연산으로 이동시킨다. 기존 하네스는 모든 스킬 메타데이터를 컨텍스트에 사전 주입하여 주의 분산과 라이브러리 크기 상한을 유발하고([[concepts/eager-schema-injection.md|eager schema injection]]), 검색 파이프라인은 선택을 컨텍스트 밖으로 옮기되 에이전트의 능력 밖으로도 옮긴다는 이중 진단을 제시한다. 핵심 발견은 동결 LLM의 순방향 패스에 라우팅 신호가 이미 존재하며 두 개의 선형 맵으로 판독 가능하다는 것으로, [[concepts/internal-prediction-readout.md|internal prediction readout]] 패러다임을 스킬 선택 도메인으로 확장한다. [[concepts/tool-attention.md|tool attention]]과 [[concepts/lazy-schema-loading.md|lazy schema loading]]이 스키마 주입을 게이팅·지연으로 완화했다면 본 논문은 선택 판단 자체를 스키마 없이 내부 신호에서 수행하여 [[concepts/schema-accumulation-bottleneck.md|schema accumulation bottleneck]]의 원천 제거 경로를 연다. [[concepts/visual-need-routing.md|visual need routing]]과 [[concepts/strategy-routing.md|strategy routing]]이 외부 판단 기반 라우팅이라면 본 논문은 라우팅 판단의 내재화라는 제3축을 형성한다. [[concepts/residual-stream-monitoring.md|residual stream monitoring]] 계열과 함께 내부 상태 판독이 감시 도구를 넘어 능력 구성 요소가 되는 흐름을 강화한다.

## 🔗 관련 논문

- Tool Attention Is All You Need: Dynamic Tool Gating and Lazy Schema Lo
- Skill-Conditioned Gated Self-Distillation for LLM Reasoning
- SkillOS: Learning Skill Curation for Self-Evolving Agents
- Caption-once, Frames-on-Demand: Visual-Need Routing for Budg
- Beyond One-Size-Fits-All: Sample-Adaptive Strategy Routing f
- Pythia: Toward Predictability-Driven Agent-Native LLM Servin

## 🏷️ 엔티티

- [[entities/native-skill-routing.md|native-skill-routing]]
- [[entities/internal-prediction-readout.md|internal-prediction-readout]]
- [[entities/eager-schema-injection.md|eager-schema-injection]]
- [[entities/lazy-schema-loading.md|lazy-schema-loading]]
- [[entities/tool-attention.md|tool-attention]]
- [[entities/schema-accumulation-bottleneck.md|schema-accumulation-bottleneck]]
- [[entities/residual-stream-monitoring.md|residual-stream-monitoring]]
- [[entities/skill-as-external-state.md|skill-as-external-state]]
- [[entities/skill-conditioned-gating.md|skill-conditioned-gating]]
- [[entities/retrieval-as-black-box.md|retrieval-as-black-box]]
- [[entities/harness-side-compensation.md|harness-side-compensation]]

## 📐 개념

- [[concepts/native-skill-routing.md|native-skill-routing]]
- [[concepts/metadata-preload-dispersal.md|metadata-preload-dispersal]]
- [[concepts/selection-as-agent-capability.md|selection-as-agent-capability]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-18-monitoring-and-discovering-reward-hacking-with-int]]: 두 논문 모두 동결된 LLM 내부 상태에서 선형 판독(스킬 라우팅 신호 프로브, 보상 해킹 평균 차이 벡터)으로 과업 관련 정보가 직접 읽힘을 보여, 내부 표현 기반 제어·감시라는 공통 축 위에 있다.
- → [[sources/2026-09-17-large-language-models-develop-belief-state-geometr]]: 모두 내부 표현이 컨텍스트로부터 형성되는 과업 관련 정보를 선형적 기하 구조로 부호화함을 보이며, 각각 스킬 라우팅과 ICL 지원이라는 응용으로 이어진다.
- → [[sources/2026-09-17-where-should-a-document-live-context-representatio]]: 스킬 정보를 컨텍스트 주입 대신 내부 상태에서 읽자는 제안과 문서의 거처(컨텍스트/표현/파라미터)를 묻는 질문은 '정보를 어디에 둘 것인가'라는 동일한 설계 문제의 양면이다.
