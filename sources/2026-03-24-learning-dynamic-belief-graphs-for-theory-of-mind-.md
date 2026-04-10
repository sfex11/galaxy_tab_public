# Learning Dynamic Belief Graphs for Theory-of-mind Reasoning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-24
**링크**: http://arxiv.org/abs/2603.20170v1

## 💡 핵심 인사이트

LLM의 Theory of Mind 추론에서 믿음을 정적 상태가 아닌 동적 그래프 구조로 모델링함으로써, 시간에 따른 믿음의 진화와 상호의존성을 포착하여 고위험 환경에서의 에이전트 행동 예측을 크게 개선한다.

## 📖 분석

## Learning Dynamic Belief Graphs for Theory-of-mind Reasoning

본 논문은 LLM 기반 Theory of Mind(ToM) 추론을 위해 **동적 믿음 그래프(Dynamic Belief Graph)**를 학습하는 프레임워크를 제안한다. 기존 접근법이 믿음(belief)을 정적이고 독립적으로 처리하여 시간에 따라 비일관적인 멘탈 모델을 생성하는 한계를 극복하고자, 에이전트의 암묵적이고 진화하는 믿음을 그래프 구조로 명시적으로 모델링한다.

### 기존 Wiki와의 관계

**[[llm-agent]]**와 직접적으로 관련된다. LLM 에이전트가 다른 에이전트나 인간의 의도와 믿음을 추론하는 능력은 협력적 의사결정의 핵심이며, 본 논문은 이를 구조화된 그래프로 해결한다. **[[multi-agent-system]]**에서 에이전트 간 상호작용의 기반이 되는 상대방 모델링(opponent modeling) 문제와도 밀접하다.

**[[reasoning-chain]]** 개념과 연결되는데, 믿음 그래프의 동적 업데이트가 일종의 구조화된 추론 체인으로 작동한다. 또한 재난 대응, 응급의료 등 고위험 환경에서의 적용을 강조하므로 **[[ai-safety]]**의 인간-AI 협업 안전성 논의와도 접점이 있다.

### 핵심 기여

- 믿음을 정적 잠재 상태가 아닌 **시간에 따라 진화하는 그래프 구조**로 표현
- 불확실성 하에서 에이전트의 행동 예측 성능 향상
- Human-in-the-loop 자율 시스템에서의 ToM 추론 실용성 제시

## 🔗 관련 논문

- 2026 04 09 social dynamics as critical vulnerabilities that u
- 2026 04 09 who governs the machine a machine identity governa
- 2026 04 10 tracesafe a systematic assessment of llm guardrail

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/theory-of-mind.md|theory-of-mind]]
- [[concepts/reasoning-chain.md|reasoning-chain]]
- [[concepts/multi-agent-system.md|multi-agent-system]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/cognitive-modeling.md|cognitive-modeling]]

---
_LLM 분석으로 재생성됨_
