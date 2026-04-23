# Detecting and Correcting Reference Hallucinations in Commercial LLMs and Deep Research Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-07
**링크**: http://arxiv.org/abs/2604.03173v1

## 💡 핵심 인사이트

상용 LLM과 딥 리서치 에이전트가 생성하는 인용 URL의 3~13%가 실제로 존재한 적 없는 환각이며, 이는 RAG 없이 모델이 자체 생성하는 출처의 근본적 신뢰성 한계를 최초로 대규모 정량화한 결과이다.

## 📖 분석

## Detecting and Correcting Reference Hallucinations in Commercial LLMs and Deep Research Agents

대규모 언어모델(LLM)과 딥 리서치 에이전트가 생성하는 인용 URL의 신뢰성을 체계적으로 측정한 최초의 대규모 연구이다. 10개 모델/에이전트를 대상으로 DRBench(53,090개 URL)와 ExpertQA(168,021개 URL, 32개 학술 분야)를 활용하여 6가지 연구 질문을 검증했다.

핵심 발견으로, 인용 URL의 3~13%가 **환각(hallucination)**된 것으로 나타났다. 이 URL들은 Wayback Machine에도 기록이 없어 실제로 존재한 적이 없을 가능성이 높다. 추가로 5~18%는 접근 불가능한 상태였다. 이는 LLM이 사실적 주장을 뒷받침하기 위해 그럴듯하지만 허구의 출처를 생성하는 심각한 신뢰성 문제를 드러낸다.

이 연구는 기존 LLM 벤치마크 연구들이 모델의 추론 능력이나 태스크 수행 정확도에 집중한 것과 달리, **출력의 근거(grounding) 품질**이라는 새로운 평가 축을 제시한다. 특히 RAG(Retrieval-Augmented Generation) 파이프라인이 환각을 줄이는 해법으로 주목받는 상황에서, 검색 없이 모델이 자체 생성하는 인용의 취약성을 정량화한 점이 중요하다.

딥 리서치 에이전트의 인용 환각 문제는 [[concepts/ai-safety.md|ai safety]] 및 [[concepts/ai-governance.md|ai governance]] 관점에서도 중대한 함의를 가진다. 학술·법률·의료 등 고위험 도메인에서 허위 인용은 잘못된 의사결정으로 이어질 수 있기 때문이다. 또한 에이전트 신뢰성 감사([[concepts/agent-reliability-auditing.md|agent reliability auditing]])의 범위를 행동 정확성에서 출처 정확성으로 확장해야 함을 시사한다.

## 🔗 관련 논문

- 2026 04 10 a systematic study of retrieval pipeline design fo
- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 09 who governs the machine a machine identity governa
- 2026 03 27 march multi agent reinforced self check for llm ha
- 2026 03 25 evaluating the reliability and fidelity of automat

## 🏷️ 엔티티

- [[entities/llm.md|LLM]]

## 📐 개념

- [[concepts/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/ai-governance.md|ai-governance]]
- [[concepts/agent-reliability-auditing.md|agent-reliability-auditing]]
- [[concepts/reasoning-integrity.md|reasoning-integrity]]
- [[concepts/citation-hallucination.md|citation-hallucination]]

---
_LLM 분석으로 재생성됨_
