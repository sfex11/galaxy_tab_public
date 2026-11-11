# Pyrite: Building and Benchmarking Protein-Ligand Pose Ranking Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-12
**링크**: http://arxiv.org/abs/2611.14511v1

## 💡 핵심 인사이트

약물 발견 포즈 순위 평가의 병목은 AI 능력이 아니라 전문 화학자조차 판별하지 못하는 평가 신호의 근본적 결핍이며, 쌍별 상대 비교가 이 신호 결핍 하에서 유일하게 정의 가능한 평가 형식이다.

## 📖 분석

# Pyrite: 단백질-리간드 포즈 순위 에이전트의 구축과 벤치마킹 (2026-11-12)

소분자 약물 발견에서 cofolding 모델은 다양한 결합 포즈 후보를 생성할 수 있으나, 그 순위를 신뢰성 있게 매기는 것은 미해결 과제다. Pyrite는 다양한 단백질-리간드 복합체에 걸친 1,500개 포즈 쌍의 쌍별(pairwise) 순위 벤치마크로, 포즈 순위 에이전트의 구축과 평가를 동시에 다룬다.

가장 중요한 발견은 평가 신호의 결핍이다 — 3D 시각화 도구와 물리 기반 점수를 갖춘 전문 화학자조차 거의 무작위 수준의 판별력을 보였다. 이는 [[signal-existence-premise]]가 전제하는 '좋은 신호의 존재'가 이 도메인에서 붕괴함을 실증한다. 문제는 신호의 정제·할당이 아니라 신호 자체의 부재이며, 다중 신호원(시각화+물리 점수)의 결합으로도 회복되지 않는다.

평가 구조는 [[comparison-oracle]]과 [[relative-verifiability]]의 과학 도메인 실현이다. 검증 가능성의 기준이 절대 정답 일치에서 포즈 간 상대 순위로 전이되며, 절대 정답 부재 환경에서 쌍별 비교만이 정의 가능한 평가 형식이라는 논리가 LLM 선호 정렬에서 구조화된 과학 과제로 확장된다. 동시에 [[benchmark-domain-specialization]] 트렌드에 약물 발견 도메인을 추가하여, 에이전트 평가의 수직 특화가 과학 응용으로 확장됨을 확정한다.

[[tacit-criteria-surfacing]] 관점에서 이 논문은 역방향 교훈을 제공한다 — 포즈 품질의 암묵적 기준은 전문가에게조차 신뢰 가능한 형식으로 외면화되지 않으므로, 기준 표면화 전략의 성립 조건(전문가 지식의 존재·접근 가능성)이 도메인별로 검증되어야 함을 보여준다. 포즈 순위 에이전트 연구는 [[research-capability-benchmark]]에 물리 구조 판단이라는 새 축을 열며, 실험적 결합 데이터라는 환경 근거([[environment-grounded-validity]])와의 접지가 후속 과제가 된다.

## 🔗 관련 논문

- A Zeroth-Order Paradigm for LLM Preference Alignment
- SWE-Serve: Benchmarking Agentic Engineering For Production Inference S
- A Living Benchmark for Information Retrieval from Electronic Health Re
- SAEScientist-Bench: Can AI Agents Conduct Autonomous SAE Interp

## 🏷️ 엔티티

- [[entities/pyrite-benchmark.md|pyrite-benchmark]]
- [[entities/benchmark-domain-specialization.md|benchmark-domain-specialization]]
- [[entities/research-capability-benchmark.md|research-capability-benchmark]]
- [[entities/tacit-criteria-surfacing.md|tacit-criteria-surfacing]]

## 📐 개념

- [[concepts/comparison-oracle.md|comparison-oracle]]
- [[concepts/signal-existence-premise.md|signal-existence-premise]]
- [[concepts/relative-verifiability.md|relative-verifiability]]
- [[concepts/environment-grounded-validity.md|environment-grounded-validity]]
- [[concepts/tacit-criteria-surfacing.md|tacit-criteria-surfacing]]

---
_LLM 분석으로 생성됨_
