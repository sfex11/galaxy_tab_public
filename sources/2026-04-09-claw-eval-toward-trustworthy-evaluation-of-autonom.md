# Claw-Eval: Toward Trustworthy Evaluation of Autonomous Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-09
**링크**: http://arxiv.org/abs/2604.06132v1

## 💡 핵심 인사이트

에이전트 평가를 최종 결과 중심에서 trajectory 전체의 안전성·강건성·다모달 상호작용까지 포괄하는 엔드투엔드 프레임워크로 확장함으로써, 실환경 배포 전 신뢰성 검증의 새로운 표준을 제시한다.

## 📖 분석

## Claw-Eval: Toward Trustworthy Evaluation of Autonomous Agents

**arXiv**: http://arxiv.org/abs/2604.06132v1
**날짜**: 2026-04-09

Claw-Eval은 자율 에이전트의 신뢰성 있는 평가를 위한 엔드투엔드 평가 스위트로, 기존 에이전트 벤치마크의 세 가지 핵심 한계를 해결한다. 첫째, 최종 출력만 확인하는 **trajectory-opaque grading** 문제를 해결하여 에이전트의 중간 경로까지 평가한다. 둘째, 안전성과 강건성 평가의 **underspecification** 문제를 다루며, 셋째 좁은 모달리티 커버리지와 상호작용 패러다임의 한계를 극복한다. 300개의 인간 검증 태스크로 구성되어 있으며, 실제 소프트웨어 환경에서 다단계 워크플로우를 수행하는 LLM 에이전트를 종합적으로 평가한다.

이 연구는 [[entities/llm-agent|LLM Agent]] 생태계의 평가 방법론을 체계화하는 데 기여하며, [[entities/openclaw|OpenClaw]] 프로젝트와 직접적인 관련이 있다. 기존의 [[concepts/closed-loop-evaluation|closed-loop evaluation]] 접근과 달리, trajectory 수준의 세밀한 평가를 도입한 점이 차별화된다. [[concepts/ai-safety|AI Safety]] 관점에서 에이전트의 안전성 평가를 명시적으로 포함하며, [[concepts/web-agent-evaluation|web-agent-evaluation]]과 [[concepts/tool-use|tool-use]] 평가를 통합적으로 다룬다. TraceSafe가 가드레일 수준의 안전성을 평가했다면, Claw-Eval은 전체 에이전트 파이프라인의 신뢰성을 포괄적으로 평가하는 프레임워크를 제시한다.

## 🔗 관련 논문

- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 11 clawbench can ai agents complete everyday online t
- 2026 04 11 act wisely cultivating meta cognitive tool use in
- 2026 04 09 who governs the machine a machine identity governa
- 2026 04 10 how much llm does a self revising agent actually n

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/openclaw.md|openclaw]]

## 📐 개념

- [[concepts/closed-loop-evaluation.md|closed-loop-evaluation]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/web-agent-evaluation.md|web-agent-evaluation]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/agent-reliability-auditing.md|agent-reliability-auditing]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[concepts/disembodied-vs-embodied-safety-evaluation.md|disembodied vs embodied safety evaluation]]

---
**관련**: [[concepts/evaluation-planning-irreducibility.md|evaluation planning irreducibility]]

---
**관련**: [[concepts/dual-evaluation-distortion.md|dual evaluation distortion]]

---
**관련**: [[concepts/trajectory-opacity.md|trajectory opacity]]

---
**관련**: [[concepts/clinical-readability-evaluation.md|clinical readability evaluation]]

---
**관련**: [[concepts/trajectory-prediction.md|trajectory prediction]]
