# When LLMs Stop Following Steps: A Diagnostic Study of Procedural Execution in Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-05
**링크**: http://arxiv.org/abs/2605.00817v1

## 💡 핵심 인사이트

최종 답변 정확도는 모델이 지정된 절차를 충실히 따랐는지에 대한 정보를 전혀 제공하지 않으며, 모델은 명시적 알고리즘을 자체적 단축 경로로 대체하면서도 정답을 산출할 수 있어 절차적 충실도와 출력 정확도는 본질적으로 분리 가능한 두 차원이다.

## 📖 분석

## 정의
LLM이 프롬프트에 명시된 절차적 알고리즘을 충실히 수행하는지를 진단하는 연구로, 최종 답변 정확도와 절차 수행 충실도가 분리될 수 있음을 체계적으로 실증한다. 단순 산술 연산으로 구성된 단계별 알고리즘을 제시하고 두 개의 수치 입력을 주어 최종 계산값을 반환하도록 하되, 알고리즘 길이를 증가시켜 복잡도를 제어하는 진단 벤치마크를 제안한다.

## 기존 Wiki와의 관계
이 논문은 [[concepts/reasoning-integrity.md|reasoning integrity]]를 '논리적 타당성'에서 '절차적 충실도'로 확장하는 구체적 실증을 제공한다. 기존에 [[concepts/unrecoverable-reasoning-error.md|unrecoverable reasoning error]]가 '한 번 잘못된 단계를 밟으면 복구 불가능'함을 기술했다면, 본 논문은 이를 절차적 실행 맥락에서 정량화 가능한 현상으로 구체화한다.

[[concepts/meaning-insensitive-metric.md|meaning insensitive metric]]의 새로운 사례를 제공한다 — 최종 답변 정확도는 절차 수행의 충실도를 측정하지 못하며, 모델이 알고리즘을 무시하고 자체적 단축 경로로 정답에 도달하는 현상을 포착하지 못한다. 이는 [[concepts/evaluator-assumption.md|evaluator assumption]]이 '정답 일치 = 절차 준수'를 암묵적으로 가정하는 구조적 문제의 또 다른 현현이다.

[[concepts/benchmark.md|benchmark]] 엔티티에 대하여, 정적 태스크에서의 천장 성능 문제([[concepts/ceiling-performance-problem.md|ceiling performance problem]])뿐 아니라 '측정 대상의 오귀정' 문제 — 즉, 우리가 무엇을 측정하고 있는지에 대한 메타적 오류 — 를 진단하는 벤치마크로서의 역할을 부여한다.

## 연결점
[[concepts/process-control-architecture.md|process control architecture]](Box Maze)가 추론 프로세스의 무결성을 아키텍처 수준에서 강제하려 한다면, 본 논문은 그 강제의 대상이 되는 '절차적 준수'라는 속성이 현재 어느 정도로 결여되어 있는지를 기준선으로 제공한다. [[concepts/shortcut-learning.md|shortcut learning]]과도 연결되는데, 모델이 명시적 알고리즘을 '단축 경로'로 대체하는 행위가 절차적 불충실의 미시적 메커니즘으로 해석될 수 있다.

## 🔗 관련 논문

- sources/2026-04-22-box-maze-a-process-control-architecture-for-reliab.md
- sources/2026-04-30-from-syntax-to-emotion-a-mechanistic-analysis-of-e.md
- sources/2026-04-25-mathduels-evaluating-llms-as-problem-posers-and-so.md
- sources/2026-04-24-diagnosing-cfg-interpretation-in-llms.md

## 🏷️ 엔티티

- [[entities/reasoning-integrity.md|reasoning-integrity]]
- [[entities/unrecoverable-reasoning-error.md|unrecoverable-reasoning-error]]
- [[entities/meaning-insensitive-metric.md|meaning-insensitive-metric]]
- [[entities/evaluator-assumption.md|evaluator-assumption]]
- [[entities/benchmark.md|benchmark]]
- [[entities/ceiling-performance-problem.md|ceiling-performance-problem]]
- [[entities/process-control-architecture.md|process-control-architecture]]
- [[entities/shortcut-learning.md|shortcut-learning]]

## 📐 개념

- [[concepts/procedural-faithfulness.md|procedural-faithfulness]]
- [[concepts/procedure-accuracy-decoupling.md|procedure-accuracy-decoupling]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-05-05-to-call-or-not-to-call-a-framework-to-assess-and-o]]: 두 논문 모두 LLM이 지정된 동작 규격을 따르지 않는 현상을 분석하며, 하나는 도구 호출 결정 경계에서, 다른 하나는 절차적 실행 충실도에서 이 문제를 다룬다.
- → [[sources/2026-05-06-scprm-a-schema-aware-cumulative-process-reward-mod]]: 두 논문 모두 최종 출력이 아닌 중간 단계의 품질을 평가해야 한다는 공통 인식을 공유하며, 하나는 프로세스 보상 모델로, 다른 하나는 절차적 충실도 진단으로 이를 접근한다.
- → [[sources/2026-05-07-mcjudgebench-a-benchmark-for-constraint-level-judg]]: 두 논문 모두 LLM 평가 방법론의 한계를 지적하며, 하나는 응답 수준이 아닌 제약 조건 수준 판단의 필요성을, 다른 하나는 최종 정확도가 아닌 절차적 충실도의 독립적 측정 필요성을 주장한다.

---
**관련**: [[concepts/procedural-independence.md|procedural independence]]
