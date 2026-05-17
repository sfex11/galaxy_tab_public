# Vision2Web: A Hierarchical Benchmark for Visual Website Development with Agent Verification

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-30
**링크**: http://arxiv.org/abs/2603.26648v1

## 💡 핵심 인사이트

웹 에이전트 평가를 '웹 사용'에서 '웹 생성'으로 확장하며, 정적→인터랙티브→풀스택의 계층적 난이도 설계로 코딩 에이전트의 실제 개발 능력을 체계적으로 분리 측정할 수 있는 벤치마크를 제시한다.

## 📖 분석

## Vision2Web: 시각적 웹사이트 개발을 위한 계층적 벤치마크

Vision2Web은 LLM 기반 코딩 에이전트의 웹사이트 개발 능력을 체계적으로 평가하기 위한 계층적 벤치마크이다. 기존 UI-to-code 벤치마크가 정적 페이지 생성에 국한되었던 한계를 넘어, **정적 UI-to-code 생성 → 인터랙티브 멀티페이지 프론트엔드 재현 → 장기 호라이즌 풀스택 웹 개발**의 3단계 난이도 계층을 제시한다. 실제 웹사이트에서 수집된 총 193개 태스크로 구성되며, 에이전트 기반 검증(agent verification) 방식을 도입하여 시각적 충실도뿐 아니라 기능적 정확성까지 평가한다.

이 벤치마크는 [[entities/llm-agent.md|llm agent]] 평가 연구의 새로운 축을 형성한다. 기존 웹 에이전트 벤치마크인 [[ClawBench]]가 웹 탐색 및 일상 온라인 태스크 완수 능력을 측정했다면, Vision2Web은 **웹사이트를 '사용'하는 것이 아닌 '생성'하는** 능력에 초점을 맞춘다. 코드 생성 품질 평가라는 점에서 [[concepts/code-generation.md|code generation]] 개념과도 연결되며, 에이전트가 장기 호라이즌 태스크를 수행하는 구조는 [[concepts/tool-use.md|tool use]] 및 멀티스텝 추론 능력과 밀접하다.

계층적 평가 설계는 단순 코드 생성을 넘어 에이전트의 계획 수립, 상태 관리, 반복적 디버깅 능력까지 측정할 수 있게 하며, 이는 [[concepts/llm-benchmark.md|llm benchmark]] 분야에서 태스크 복잡도에 따른 능력 분리 평가라는 방법론적 기여를 한다.

## 🔗 관련 논문

- 2026 04 11 clawbench can ai agents complete everyday online t
- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 11 figures as interfaces toward llm native artifacts
- 2026 04 09 paper circle an open source multi agent research d

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/code-generation.md|code-generation]]
- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/web-agent-evaluation.md|web-agent-evaluation]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[entities/formal-verification.md|formal verification]]

---
**관련**: [[concepts/step-level-verification-decoding.md|step level verification decoding]]

---
**관련**: [[concepts/paired-route-benchmark.md|paired route benchmark]]

---
**관련**: [[concepts/benchmark.md|benchmark]]

---
**관련**: [[concepts/executable-benchmark.md|executable benchmark]]

---
**관련**: [[concepts/hierarchical-planning.md|hierarchical planning]]

---
**관련**: [[entities/self-play-benchmark.md|self play benchmark]]

---
**관련**: [[entities/live-benchmark.md|live benchmark]]

---
**관련**: [[entities/hierarchical-planning.md|hierarchical planning]]

---
**관련**: [[concepts/dynamic-benchmark.md|dynamic benchmark]]

---
**관련**: [[concepts/self-play-benchmark.md|self play benchmark]]

---
**관련**: [[concepts/live-benchmark.md|live benchmark]]

---
**관련**: [[concepts/runtime-verification-layer.md|runtime verification layer]]

---
**관련**: [[entities/hierarchical-kv-memory.md|hierarchical kv memory]]

---
**관련**: [[concepts/execution-verification.md|execution verification]]

---
**관련**: [[concepts/hierarchical-kv-memory.md|hierarchical kv memory]]

---
**관련**: [[concepts/render-verification-gap.md|render verification gap]]

---
**관련**: [[concepts/geographic-plausibility-verification.md|geographic plausibility verification]]

---
**관련**: [[entities/hierarchical-representation.md|hierarchical representation]]

---
**관련**: [[concepts/problem-validity-verification.md|problem validity verification]]
