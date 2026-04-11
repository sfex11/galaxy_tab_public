# Joint Optimization of Reasoning and Dual-Memory for Self-Learning Diagnostic Agent

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-10
**링크**: http://arxiv.org/abs/2604.07269v1

## 💡 핵심 인사이트

인지과학의 이중 메모리 모델을 LLM 진단 에이전트에 통합하고 강화학습으로 메모리 활용과 추론을 동시 최적화함으로써, 경험 축적을 통한 지속적 진단 성능 향상이 가능함을 보여준다.

## 📖 분석

## Joint Optimization of Reasoning and Dual-Memory for Self-Learning Diagnostic Agent

임상 진단 AI 에이전트의 자기학습(self-learning) 프레임워크를 제안한 논문이다. 핵심 아이디어는 인간 의사의 인지 과정에서 영감을 받은 **이중 메모리(dual-memory) 모듈**을 LLM 기반 진단 에이전트에 통합하는 것이다.

### 핵심 구조: SEA (Self-learning diagnostic agEnt)

기존 LLM 진단 에이전트들은 각 케이스를 독립적으로 처리하여 경험 재사용과 지속적 적응이 불가능했다. SEA는 이를 해결하기 위해:

1. **이중 메모리 모듈**: 인지과학의 단기/장기 기억 구분에 기반하여, 개별 진단 경험(에피소드 메모리)과 일반화된 진단 패턴(시맨틱 메모리)을 분리 저장한다.
2. **강화학습 기반 추론 최적화**: 메모리 활용과 추론 과정을 동시에 최적화하는 RL 훈련 프레임워크를 설계했다.
3. **경험 재사용**: 과거 진단 사례에서 추출한 패턴을 새로운 케이스에 적용하여 지속적 성능 향상을 달성한다.

### 기존 연구와의 연결

이 논문은 [[adaptive-forgetting]], [[memory-management]] 개념과 직접적으로 연결된다. 특히 Novel Memory Forgetting Techniques 논문이 다룬 에이전트 메모리 관리 문제의 의료 도메인 적용으로 볼 수 있다. [[cognitive-architecture]] 관점에서는 Triadic Cognitive Architecture 논문과 유사하게 인지과학적 구조를 AI에 적용하지만, 진단이라는 구체적 태스크에 특화했다.

[[reinforcement-learning]]을 메모리 최적화에 활용하는 접근은 Android Coach의 온라인 에이전트 훈련, Batched Contextual Reinforcement의 효율적 RL 프레임워크와 방법론적 유사성이 있다. [[medical-ai]] 측면에서는 MARCUS의 의료 VLM 접근과 상호보완적이다.

## 🔗 관련 논문

- Novel Memory Forgetting Techniques for Autonomous AI Agents:
- The Triadic Cognitive Architecture: Bounding Autonomous Acti
- Coupled Control, Structured Memory, and Verifiable Action in
- Android Coach: Improve Online Agentic Training Effi
- Batched Contextual Reinforcement: A Task-Scaling Law for Eff
- MARCUS: An agentic, multimodal vision-language model for car
- MTI: A Behavior-Based Temperament Profiling System for AI Ag
- ChameleonEpisodicMemoryforLong

## 📐 개념

- [[concepts/dual-memory-architecture.md|dual-memory-architecture]]
- [[concepts/self-learning-agent.md|self-learning-agent]]
- [[concepts/clinical-reasoning.md|clinical-reasoning]]
- [[concepts/experience-reuse.md|experience-reuse]]

---
_LLM 분석으로 재생성됨_
