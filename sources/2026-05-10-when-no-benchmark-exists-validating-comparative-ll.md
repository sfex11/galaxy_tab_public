# When No Benchmark Exists: Validating Comparative LLM Safety Scoring Without Ground-Truth Labels

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-10
**링크**: http://arxiv.org/abs/2605.06652v1

## 💡 핵심 인사이트

LLM 안전성 평가의 타당성은 정답 레이블의 유무가 아닌 평가 계약(시나리오·기준·심사자·판정자·샘플링·재실행 예산)의 고정성과 일관성에 달려있다는 것을 형식화함으로써, 벤치마크가 존재하지 않는 실제 배포 환경에서도 안전성 비교 점수를 배포 증거로 사용할 수 있는 길을 열었다.

## 📖 분석

# Benchmarkless Comparative Safety Scoring

**카테고리**: AI Safety / Evaluation Methodology
**생성일**: 2026-05-10

## 정의

실제 배포 환경에서 관련 언어·산업·규제 체제에 대한 정답 레이블이 있는 벤치마크가 존재하지 않는 상황에서, 후보 LLM 간의 안전성을 비교 점수화하는 문제 설정. 점수는 고정된 시나리오 묶음(scenario pack), 평가 기준(rubric), 심사자(auditor), 판정자(judge), 샘플링 설정, 재실행 예산의 6가지 계약 조건 하에서만 유효하다.

## 핵심 기여

기존 [[statistical-certification|통계적 인증]]이 정답 레이블을 전제로 안전 확률 경계를 설정했다면, 본 논문은 레이블 없이 일관성 검사(consistency check)로 이를 대체하는 경로를 제공한다. 이는 [[ai-risk-regulation|AI 규제]]의 실무적 장벽 — 규제 대상 도메인에 벤치마크가 없다는 [[regulatory-vacuity|규제 공백]] — 에 대한 직접적 해결책이다.

## 계약적 평가 패러다임

[[evaluator-assumption|평가자의 가정]]을 암묵적 전제에서 명시적 계약 항목으로 전환한다는 점에서, [[llm-as-judge|LLM-as-Judge]]의 신뢰성 문제를 '판정자 고정'이라는 계약 조건으로 흡수한다. [[certification-invariance|인증 불변성]]에 대한 부분적 답을 제공하는데, 점수가 계약 변경에 불변하지 않음을 명시적으로 인정하면서도 고정 계약 하에서의 상대적 비교가 배포 증거로서 기능함을 보인다.

## 관련 문제와의 연결

[[safety-property-underdetermination|안전 속성 미결정]] 상황에서도 절대적 안전 증명 대신 상대적 일관성 기반 비교가 가능함을 보여주며, [[acceptable-risk-quantification|수용 가능한 위험 정량화]]를 확률적 절대 경계에서 계약적 상대 경계로 확장한다.

## 🔗 관련 논문

- 2026 05 07 safety and accuracy follow different scaling laws
- Bounding the Black Box: A Statistical Certification Framework for AI R
- Three Models of RLHF Annotation: Extension, Evidence, and Au

## 🏷️ 엔티티

- [[entities/ai-safety.md|ai-safety]]
- [[entities/ai-risk-regulation.md|ai-risk-regulation]]
- [[entities/statistical-certification.md|statistical-certification]]
- [[entities/llm-benchmark.md|llm-benchmark]]
- [[entities/evaluator-assumption.md|evaluator-assumption]]
- [[entities/llm-as-judge.md|llm-as-judge]]
- [[entities/certification-invariance.md|certification-invariance]]
- [[entities/safety-property-underdetermination.md|safety-property-underdetermination]]
- [[entities/acceptable-risk-quantification.md|acceptable-risk-quantification]]
- [[entities/benchmarkless-comparative-safety-scoring.md|benchmarkless-comparative-safety-scoring]]

## 📐 개념

- [[concepts/scenario-audit-contract.md|scenario-audit-contract]]
- [[concepts/deployment-evidence-contract.md|deployment-evidence-contract]]
- [[concepts/label-free-consistency-check.md|label-free-consistency-check]]
- [[concepts/contractual-validity-scope.md|contractual-validity-scope]]

---
_LLM 분석으로 생성됨_
