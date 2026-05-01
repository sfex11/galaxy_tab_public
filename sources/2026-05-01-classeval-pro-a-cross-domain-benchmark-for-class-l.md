# ClassEval-Pro: A Cross-Domain Benchmark for Class-Level Code Generation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-01
**링크**: http://arxiv.org/abs/2604.26923v1

## 💡 핵심 인사이트

함수 수준 코드 합성과 저장소 수준 코드 수정 사이에 '완전하고 내부적으로 구조화된 클래스를 명세로부터 구성하는 능력'이라는 독립적 평가 축이 존재하며, 이를 간과한 평가 설계는 모델의 실제 구성적 코드 능력을 체계적으로 과대평가한다.

## 📖 분석

# ClassEval-Pro: 함수-저장소 사각지대에 대한 벤치마크 제안

ClassEval-Pro는 LLM 코드 생성 평가에서 함수 수준(function-level)과 저장소 수준(repository-level) 사이에 존재하는 **구성적 코드 창작(compositional code creation)**의 사각지대를 구체화하는 크로스 도메인 벤치마크다. 기존 평가가 고립된 함수에 국한되거나 수동 큐레이션된 클래스 수준 태스크에 의존하여 확장성과 데이터 오염 저항성에서 한계를 보인다는 점을 문제 삼는다.

이 논문은 [[benchmark]] 엔티티가 지적해온 **평가자의 가정([[evaluator-assumption]])** 문제를 코드 생성 도메인에서 구체적으로 실증한다: 평가가 '함수 단위 능력'과 '저장소 단위 수정 능력'만을 측정하도록 가정을 설정해두면, 그 사이에 위치한 구성적 능력은 보이지 않게 된다. [[restestbench]]가 REST API 테스트에서 [[coverage-functionality-gap]]을 문제 삼은 것과 구조적으로 동일한 패턴이다.

또한 [[ceiling-performance-problem]]에 대한 해법 경로를 제시한다 — 크로스 도메인 설계와 데이터 오염 저항성을 통해 정적 벤치마크가 직면한 포화 문제를 구조적으로 완화한다. [[swe-chat]]이 야생 환경에서의 코딩 에이전트 상호작용을 포착한 것과 보완적 위치에 있으며, ClassEval-Pro는 통제된 환경에서 클래스 수준 구성 능력을 정밀하게 분리 측정한다.

[[repository-level-code-understanding]]의 하위 호환 문제를 역으로 조명한다: 저장소 이해가 클래스 구성 능력을 함의하지 않을 수 있으며, 두 능력은 독립적인 평가 축으로 분리되어야 한다는 점을 시사한다.

## 🔗 관련 논문

- 2026-04-30-restestbench-a-benchmark-for-evaluating-the-effect.md
- 2026-04-24-swe-chat-coding-agent-interactions-from-real-users.md
- 2026-04-29-defective-task-descriptions-in-llm-based-code-gene
- 2026-04-29-leveraging-llms-for-multi-file-dsl-code-generation

## 🏷️ 엔티티

- [[entities/classeval-pro.md|classeval-pro]]
- [[entities/class-level-code-generation.md|class-level-code-generation]]
- [[entities/compositional-code-creation.md|compositional-code-creation]]

## 📐 개념

- [[concepts/data-contamination-resistance.md|data-contamination-resistance]]
- [[concepts/cross-domain-code-evaluation.md|cross-domain-code-evaluation]]
- [[concepts/function-repository-evaluation-spectrum-gap.md|function-repository-evaluation-spectrum-gap]]

---
_LLM 분석으로 생성됨_
