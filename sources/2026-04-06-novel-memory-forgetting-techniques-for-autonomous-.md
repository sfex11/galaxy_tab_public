# Novel Memory Forgetting Techniques for Autonomous AI Agents: Balancing Relevance and Efficiency

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-06
**링크**: http://arxiv.org/abs/2604.02280v1

## 💡 핵심 인사이트

AI 에이전트의 메모리 관리에서 '무엇을 기억할 것인가'만큼 '무엇을 잊을 것인가'가 중요하며, 적응적 망각 메커니즘이 장기 대화 에이전트의 성능 유지에 핵심적이다.

## 📖 분석

## Novel Memory Forgetting Techniques for Autonomous AI Agents

자율 AI 에이전트의 장기 대화에서 메모리가 무한히 축적되면 시간적 감쇠(temporal decay)와 허위 기억 전파(false memory propagation)가 발생한다. LOCOMO 벤치마크에서 단계별 성능이 0.455에서 0.05로 급락하고, MultiWOZ에서는 지속적 메모리 유지 시 78.2% 정확도에 6.8% 허위 기억률을 보인다.

본 논문은 **적응적 예산 기반 망각 프레임워크(adaptive budgeted forgetting framework)**를 제안한다. 관련성 기반 스코어링(relevance-guided scoring)과 제한된 최적화(bounded optimization)를 통해 메모리를 조절하며, 불필요한 기억을 능동적으로 제거하여 에이전트의 추론 일관성과 효율성을 동시에 확보한다.

이 연구는 기존 메모리 관리 연구와 차별화되는 지점이 있다. [[shared-state-architecture]]의 공유 상태 아키텍처가 여러 에이전트 간 메모리 일관성에 초점을 맞추는 반면, 본 연구는 단일 에이전트 내에서의 메모리 생애주기 관리에 집중한다. [[ChameleonEpisodicMemoryforLong]] 등 에피소딕 메모리 연구가 기억의 저장과 검색에 초점을 두었다면, 본 논문은 **무엇을 잊을 것인가**라는 보완적 문제를 다룬다.

또한 [[llm-agent]] 엔티티의 핵심 과제인 장기 자율성(long-horizon autonomy)과 직결되며, [[cognitive-architecture]]의 인지 아키텍처 설계에서 망각 메커니즘이 필수 구성요소임을 실증적으로 보여준다. [[metacognition]] 개념과도 연결되는데, 에이전트가 자신의 메모리 상태를 모니터링하고 능동적으로 조절한다는 점에서 메타인지적 자기 조절의 한 형태로 볼 수 있다.

## 🔗 관련 논문

- PSI: Shared State as the Missing Layer for Coherent AI-Gener
- The Triadic Cognitive Architecture: Bounding Autonomous Acti
- Act Wisely: Cultivating Meta-Cognitive Tool Use in Agentic M
- Joint Optimization of Reasoning and Dual Memory fo

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/metacognition.md|metacognition]]
- [[concepts/shared-state-architecture.md|shared-state-architecture]]
- [[concepts/cognitive-architecture.md|cognitive-architecture]]

---
_LLM 분석으로 재생성됨_
