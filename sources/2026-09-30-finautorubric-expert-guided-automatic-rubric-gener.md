# FinAutoRubric: Expert-Guided Automatic Rubric Generation for Evaluating Financial Research Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-30
**링크**: http://arxiv.org/abs/2609.35744v1

## 💡 핵심 인사이트

평가 기준(루브릭)의 생성 자체를 전문가 가이던스가 지배하는 에이전트 파이프라인에 위임하면, 고정 벤치마크의 확장 비용 없이 기관별 전문 표준을 인코딩할 수 있다.

## 📖 분석

FinAutoRubric은 금융 리서치 에이전트 평가에서 고정 루브릭의 두 병목 — 확장 비용과 기관별 표준 인코딩 불가 — 를 '전문가 가이던스 vs 에이전트 실행'의 계층 분리로 해소한다. 전문가는 재사용 가능한 평가 가이던스를 한 번 명시하고, 에이전트와 코드가 질의별 루브릭 생성·검토·검증을 수행하며, 정보 시점(cutoff) 기준 값 고정으로 금융 사실의 시간 의존성을 처리한다. 핵심 설계는 가이던스의 이중 작용이다: 전문가 지식이 프롬프트(생성 시점 구속)와 루브릭(판정 시점 구속) 양면에서 모든 에이전트를 지배한다.

이 논문은 [[automatic-benchmark-generation]] 계열의 생성 대상을 평가 데이터(2026-09-26 EHR Living Benchmark의 질의-근거 쌍)에서 평가 기준(루브릭) 자체로 확장한다. 생성 파이프라인이 전문가 가이던스에 접지되므로, 자동 생성의 순환적 타당성 위험이 완화되는 구체적 조건을 금융 도메인에서 제시한다. [[llm-as-judge]]와 [[judge-instrument-reliability]] 논의에 '판단 행위의 사전 구속'이라는 새 교정 축을 제공하며, [[signal-evaluation-decoupling]]의 신호-평가 분리 원리가 '재사용 가이던스 계층 vs 질의별 루브릭 인스턴스'의 분리로 재현됨을 보여준다. [[rubric-to-reward-reducibility]] 관점에서 루브릭이 정적 산출물에서 동적 생성물로 이동하면, 루브릭 품질 검증이 환원 사슬의 새 상위 계층이 된다. [[benchmark-domain-specialization]]은 수직 도메인에서 기관 단위로 더 세분화된다.

## 🔗 관련 논문

- A Living Benchmark for Information Retrieval from Electronic Health Records (2026-09-26)
- Verifier-Backed Hard Problem Generation for Mathematical Reasoning (2026-05-10)
- RunAgent: Interpreting Natural-Language Plans with Constraint-Guided Execution (2026-05-05)

## 🏷️ 엔티티

- [[entities/financial-reasoning.md|financial-reasoning]]
- [[entities/automatic-benchmark-generation.md|automatic-benchmark-generation]]
- [[entities/llm-as-judge.md|llm-as-judge]]
- [[entities/judge-instrument-reliability.md|judge-instrument-reliability]]
- [[entities/rubric-to-reward-reducibility.md|rubric-to-reward-reducibility]]
- [[entities/signal-evaluation-decoupling.md|signal-evaluation-decoupling]]
- [[entities/benchmark-domain-specialization.md|benchmark-domain-specialization]]
- [[entities/expert-guided-rubric-synthesis.md|expert-guided-rubric-synthesis]]

## 📐 개념

- [[concepts/information-cutoff-anchoring.md|information-cutoff-anchoring]]
- [[concepts/dual-governance-prompt-and-rubric.md|dual-governance-prompt-and-rubric]]
- [[concepts/institution-specific-evaluation-standard.md|institution-specific-evaluation-standard]]

---
_LLM 분석으로 생성됨_
