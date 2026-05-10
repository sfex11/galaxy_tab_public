# Recursive Agent Optimization

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-10
**링크**: http://arxiv.org/abs/2605.06639v1

## 💡 핵심 인사이트

추론 시점 스케일링(재귀적 자기 위임)은 훈련 없이도 작동하지만, 그 구조를 최적으로 활용하는 것은 별개의 학습 가능한 능력이며, 이를 RL로 명시적으로 훈련해야 비로 분할-정복의 이점이 실현된다.

## 📖 분석

# Recursive Agent Optimization (RAO)

**카테고리**: AI/ML — 강화학습 기반 에이전트 훈련
**생성일**: 2026-05-10

## 정의

RAO는 에이전트가 자기 자신의 새 인스턴스를 재귀적으로 생성하여 하위 태스크를 위임하는 **재귀적 에이전트(recursive agent)**를 훈련하기 위한 강화학습 접근법이다. 분할-정복(divide-and-conquer)을 통해 더 긴 컨텍스트와 더 어려운 문제로 자연스럽게 일반화하는 추론 시점 스케일링 알고리즘을 구현하며, 단순히 재귀적 추론 구조를 사용하는 것 이상으로 모델이 이 구조를 최적으로 활용하도록 **명시적 훈련**을 제공한다.

## 기존 Wiki와의 관계

RAO는 기존에 이론적으로만 존재하던 두 개념을 최초로 실증적 훈련 프레임워크로 구체화한다:

1. **내생적 계산 확장([[concepts/endogenous-computation-expansion|endogenous-computation-expansion]])**: 외부 도구나 환경 구성에 의존하지 않고 에이전트가 자신의 계산 구조를 내부적으로 복제하여 자원을 동적으로 확장하는 메커니즘이라는 개념을 RAO가 구현체로 제공한다.

2. **도구 사용의 내재화([[concepts/internalization-of-tool-use|internalization-of-tool-use]])**: 외부 API 호출 대신 자기 자신의 재귀적 복제본을 내부적 도구로 사용하는 패러다임을 RAO가 훈련 가능한 능력으로 입증한다.

## 적응적 추론과의 관계

[[entities/adaptive-inference|adaptive-inference]]의 이중성 축에서 RAO는 **상향식(Bottom-up) 확장**의 구체적 실현이다. 기존 적응적 추론(추측 디코딩 길이 조절, CADENCE 등)이 주로 계산 자원을 **축소**하는 하향식 접근이었다면, RAO는 문제 복잡도에 맞춰 자기 재귀적으로 자원을 **확장**하는 상향식 경로를 열어준다. 이는 [[concepts/duality-of-adaptive-inference|duality-of-adaptive-inference]] 개념의 하향식 편향을 교정하는 중요한 균형추가 된다.

## 연결점

- [[sources/2026-05-08-longseeker-elastic-context-orchestration-for-long-.md|LongSeeker]]가 탄력적 컨텍스트 오케스트레이션으로 긴 컨텍스트 문제를 해결한다면, RAO는 재귀적 분할로 구조적으로 컨텍스트를 관리한다.
- [[sources/2026-04-30-recursive-multi-agent-systems.md|Recursive Multi-Agent Systems]]가 재귀적 통신 채널을 다루었다면, RAO는 재귀적 **위임 계층(delegation hierarchy)**을 훈련 대상으로 삼는다.
- [[sources/2026-05-09-can-rl-teach-long-horizon-reasoning-to-llms-expres.md|Can RL Teach Long-Horizon Reasoning]]와 짝을 이루며, 롱호라이즌 추론에 대한 RL의 효능을 재귀적 구조라는 새 차원에서 검증한다.

## 🔗 관련 논문

- 2026 05 08 longseeker elastic context orchestration for long 
- 2026 05 09 can rl teach long horizon reasoning to llms expres
- 2026 04 30 recursive multi agent systems
- 2026 05 09 strata incentivizing agentic reinforcement learnin

## 🏷️ 엔티티

- [[entities/recursive-agent-optimization.md|recursive-agent-optimization]]
- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/reinforcement-learning.md|reinforcement-learning]]
- [[entities/llm-agent.md|llm-agent]]
- [[entities/recursive-multi-agent-scaling.md|recursive-multi-agent-scaling]]

## 📐 개념

- [[concepts/endogenous-computation-expansion.md|endogenous-computation-expansion]]
- [[concepts/internalization-of-tool-use.md|internalization-of-tool-use]]
- [[concepts/duality-of-adaptive-inference.md|duality-of-adaptive-inference]]
- [[concepts/exploration-absorption-decoupling.md|exploration-absorption-decoupling]]

---
_LLM 분석으로 생성됨_
