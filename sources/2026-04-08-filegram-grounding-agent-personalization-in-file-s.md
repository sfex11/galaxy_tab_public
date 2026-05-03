# FileGram: Grounding Agent Personalization in File-System Behavioral Traces

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-08
**링크**: http://arxiv.org/abs/2604.04901v1

## 💡 핵심 인사이트

파일 시스템 조작 로그를 개인화 신호로 재해석함으로써, 대화 이력 의존적이던 에이전트 개인화의 데이터 병목을 우회하는 새로운 패러다임을 제시한다.

## 📖 분석

## FileGram: 파일 시스템 행동 흔적 기반 에이전트 개인화

FileGram은 로컬 파일 시스템에서 동작하는 AI 에이전트의 개인화(personalization) 문제를 다루는 프레임워크다. 기존 개인화 연구가 대화 이력이나 사용자 프로필 같은 상호작용 중심(interaction-centric) 데이터에 의존한 반면, FileGram은 파일 시스템 조작(생성, 수정, 삭제, 이동 등)에서 발생하는 **행동 흔적(behavioral traces)**을 밀도 높은 개인화 신호로 활용한다는 점에서 차별화된다.

### 핵심 문제의식
로컬 파일 시스템에서 작동하는 코워킹(coworking) AI 에이전트가 빠르게 등장하고 있지만, 프라이버시 제약과 멀티모달 실세계 흔적의 수집 난이도로 인해 학습·평가용 데이터가 극도로 부족하다. FileGram은 이 데이터 병목을 파일 시스템 행동 로그라는 새로운 모달리티로 우회한다.

### 기존 Wiki와의 관계
- **[[concepts/personal-ai-agent.md|personal ai agent]]**: PSI(공유 상태 계층)와 HippoCamp가 개인 컴퓨팅 맥락에서 에이전트 일관성과 벤치마킹을 다뤘다면, FileGram은 개인화의 **데이터 소스** 자체를 파일 시스템으로 재정의한다.
- **[[concepts/memory-management.md|memory management]]**: 에이전트 메모리 망각 기법(Novel Memory Forgetting)이 무엇을 기억/잊을지를 다뤘다면, FileGram은 파일 조작 패턴이라는 암묵적 기억을 개인화에 연결한다.
- **[[concepts/context-bus.md|context bus]]** / **[[concepts/shared-state-architecture.md|shared state architecture]]**: PSI의 공유 상태 레이어가 에이전트 간 일관성을 위한 것이라면, FileGram의 파일 시스템 트레이스는 단일 사용자-에이전트 간 개인화를 위한 상태 소스다.
- **[[entities/llm-agent.md|llm agent]]**: 에이전트 평가(ClawBench, TraceSafe)와 보안(OpenClaw) 연구들이 에이전트 행동의 신뢰성·안전성을 다뤘다면, FileGram은 에이전트가 사용자에게 얼마나 맞춤화될 수 있는지를 측정하는 새로운 축을 제시한다.

### 시사점
파일 시스템 로그는 프라이버시 민감도가 높아 실제 배포 시 [[concepts/differential-privacy.md|differential privacy]] 기법과의 결합이 필수적일 것으로 보인다. 또한 행동 흔적 기반 접근은 웹 에이전트([[concepts/web-agent-evaluation.md|web agent evaluation]])나 코드 에이전트([[concepts/repository-level-code-understanding.md|repository level code understanding]]) 등 다른 도메인으로 확장 가능한 일반적 패러다임이다.

## 🔗 관련 논문

- 2026 04 11 psi shared state as the missing layer for coherent
- 2026 04 11 clawbench can ai agents complete everyday online t
- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 11 act wisely cultivating meta cognitive tool use in

## 📐 개념

- [[concepts/file-system-behavioral-trace.md|file-system-behavioral-trace]]
- [[concepts/agent-personalization.md|agent-personalization]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[concepts/behavioral-temperament.md|behavioral temperament]]

---
**관련**: [[concepts/syntax-behavior-semantics-disentanglement.md|syntax behavior semantics disentanglement]]

---
**관련**: [[concepts/dual-trace-encoding.md|dual trace encoding]]

---
**관련**: [[concepts/image-grounding.md|image grounding]]

---
**관련**: [[concepts/recommendation-system.md|recommendation system]]

---
**관련**: [[concepts/formal-semantic-grounding.md|formal semantic grounding]]

---
**관련**: [[entities/machine-behavior.md|machine behavior]]

---
**관련**: [[concepts/functional-behavior-validation.md|functional behavior validation]]

---
**관련**: [[concepts/persona-collapse.md|persona collapse]]

---
**관련**: [[concepts/behavioral-manifold-confinement.md|behavioral manifold confinement]]

---
**관련**: [[concepts/native-environmental-grounding.md|native environmental grounding]]

---
**관련**: [[concepts/algorithm-system-translation-gap.md|algorithm system translation gap]]

---
**관련**: [[concepts/persona-runtime-fidelity-gap.md|persona runtime fidelity gap]]

---
**관련**: [[concepts/semantic-system-state-disconnect.md|semantic system state disconnect]]
