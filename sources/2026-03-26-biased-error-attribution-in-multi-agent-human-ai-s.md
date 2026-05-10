# Biased Error Attribution in Multi-Agent Human-AI Systems Under Delayed Feedback

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-26
**링크**: http://arxiv.org/abs/2603.23419v1

## 💡 핵심 인사이트

다중 AI 에이전트 시스템에서 지연된 피드백은 인간 감독자의 오류 귀인을 체계적으로 왜곡하며, 이는 다중 에이전트 시스템의 투명성 설계가 단순한 성능 문제가 아닌 인지 편향 완화 관점에서 접근되어야 함을 시사한다.

## 📖 분석

## Biased Error Attribution in Multi-Agent Human-AI Systems Under Delayed Feedback

본 논문은 다중 AI 에이전트 환경에서 지연된 피드백(delayed feedback) 조건 하에 인간의 오류 귀인(error attribution)이 어떻게 인지 편향(cognitive bias)에 의해 왜곡되는지를 연구한다. 기존 연구가 단일 에이전트와의 즉각적 결과 상황에 집중했던 것과 달리, 본 연구는 **다단계 의사결정(multi-step decision-making)**에서 각 단계의 결정이 후속 상태에 영향을 미치는 순차적 환경을 다룬다.

### 핵심 기여

1. **지연된 결과와 편향의 관계**: 결과가 즉시 드러나지 않는 환경에서 인간은 특정 AI 에이전트에 체계적으로 편향된 오류 귀인을 수행함을 실증적으로 보여준다.
2. **다중 에이전트 맥락의 복잡성**: 여러 AI 에이전트가 협력하는 시스템에서 인간 감독자가 어떤 에이전트의 실수인지 판단할 때 발생하는 귀인 오류 패턴을 분석한다.
3. **인간-AI 협업 설계 시사점**: 다중 에이전트 시스템의 투명성(transparency)과 설명 가능성(explainability) 설계에 대한 실질적 가이드라인을 제시한다.

### Wiki 연결점

본 연구는 [[concepts/multi-agent-system.md|multi agent system]] 개념과 직접적으로 관련되며, 특히 다중 에이전트 간 책임 소재를 인간이 판단하는 문제를 다룬다는 점에서 [[concepts/theory-of-mind.md|theory of mind]] 및 [[concepts/cognitive-modeling.md|cognitive modeling]] 개념과도 밀접하다. 또한 [[concepts/ai-safety.md|ai safety]] 관점에서 인간 감독(human oversight) 하의 편향 문제를 다루므로, TraceSafe 등 LLM 가드레일 연구와 보완적 관계에 있다. LLM Agent의 신뢰성과 거버넌스를 다룬 'Who Governs the Machine' 논문과도 인간-AI 신뢰 측면에서 연결된다.

## 🔗 관련 논문

- 2026 04 09 social dynamics as critical vulnerabilities that u
- 2026 04 09 who governs the machine a machine identity governa
- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 09 claw eval toward trustworthy evaluation of autonom

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/multi-agent-system.md|multi-agent-system]]

## 📐 개념

- [[concepts/cognitive-modeling.md|cognitive-modeling]]
- [[concepts/theory-of-mind.md|theory-of-mind]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/multi-agent-system.md|multi-agent-system]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[concepts/zero-error-capacity.md|zero error capacity]]

---
**관련**: [[concepts/compounding-error.md|compounding error]]

---
**관련**: [[concepts/ai-feedback-loop.md|ai feedback loop]]

---
**관련**: [[entities/word-error-rate.md|word error rate]]

---
**관련**: [[concepts/attribution-scarcity.md|attribution scarcity]]

---
**관련**: [[concepts/error-attribution-problem.md|error attribution problem]]

---
**관련**: [[concepts/word-error-rate.md|word error rate]]

---
**관련**: [[concepts/bayesian-update-cumulative-error.md|bayesian update cumulative error]]
