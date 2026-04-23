# Brief Is Better: Non-Monotonic Chain-of-Thought Budget Effects in Function-Calling Language Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-03
**링크**: http://arxiv.org/abs/2604.02155v1

## 💡 핵심 인사이트

함수 호출 에이전트에서 CoT 추론 길이와 성능은 비단조적 관계를 보이며, 짧고 간결한 추론이 긴 추론보다 오히려 더 높은 정확도를 달성한다.

## 📖 분석

## Brief Is Better: Non-Monotonic Chain-of-Thought Budget Effects in Function-Calling Language Agents

**arXiv**: http://arxiv.org/abs/2604.02155v1
**날짜**: 2026-04-03

### 핵심 요약

언어 에이전트가 행동 전에 얼마나 사고해야 하는가? Chain-of-Thought(CoT) 추론이 에이전트 성능을 향상시킨다는 가정이 널리 퍼져 있지만, 구조화된 도구 사용 환경에서 추론 길이와 정확도 간의 관계는 잘 이해되지 않았다. 본 연구는 Berkeley Function Calling Leaderboard v3 Multiple 벤치마크의 200개 태스크에 대해 6개 토큰 버짓(0~512)을 스위핑하며 CoT 버짓 효과를 체계적으로 분석한다.

### 주요 발견

가장 핵심적인 발견은 **비단조적(non-monotonic) 관계**다. 추론 토큰을 늘린다고 성능이 계속 좋아지는 것이 아니라, 짧고 간결한 추론이 오히려 더 나은 성능을 보인다. 이는 CoT가 길어질수록 "overthinking" 현상이 발생하여 함수 호출의 정확도가 저하될 수 있음을 시사한다.

### 기존 연구와의 연결

이 결과는 [[concepts/reasoning-chain.md|reasoning chain]] 및 [[concepts/reasoning-integrity.md|reasoning integrity]] 개념과 직접적으로 관련된다. 추론 체인의 길이가 반드시 품질을 보장하지 않는다는 점에서, Box Maze의 프로세스 제어 아키텍처([[concepts/process-control-architecture.md|process control architecture]])가 제안한 구조화된 추론 제어의 필요성을 뒷받침한다. 또한 [[concepts/tool-use.md|tool use]] 개념과 밀접하며, TraceSafe의 가드레일 연구와도 연결된다—도구 호출 시 과도한 추론이 오히려 안전성 문제를 야기할 수 있다. [[concepts/metacognition.md|metacognition]] 관점에서 Act Wisely 논문이 제안한 메타인지적 도구 사용과도 상보적이다: 언제 충분히 생각했는지 아는 것이 중요하다.

### 시사점

함수 호출 에이전트 설계 시 CoT 버짓을 무조건 늘리기보다 최적 구간을 찾는 것이 중요하며, 이는 추론 효율성과 비용 절감 모두에 실질적 함의를 갖는다.

## 🔗 관련 논문

- 2026 04 11 act wisely cultivating meta cognitive tool use in
- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 10 how much llm does a self revising agent actually n

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/reasoning-chain.md|reasoning-chain]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/metacognition.md|metacognition]]
- [[concepts/reasoning-integrity.md|reasoning-integrity]]
- [[concepts/process-control-architecture.md|process-control-architecture]]
- [[concepts/llm-benchmark.md|llm-benchmark]]

---
_LLM 분석으로 재생성됨_
