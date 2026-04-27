# MathDuels: Evaluating LLMs as Problem Posers and Solvers

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-27
**링크**: http://arxiv.org/abs/2604.21916v1

## 💡 핵심 인사이트

정적 벤치마크의 천장 성능 문제는 더 어려운 문제를 만드는 것으로 해결될 수 없으며, 모델을 평가 대상에서 평가 설계자(문제 출제자)로 전환시키는 셀프플레이 구조만이 평가의 근본적 한계를 구조적으로 해결한다.

## 📖 분석

# MathDuels: Evaluating LLMs as Problem Posers and Solvers

## 기존 Wiki와의 관계

본 논문의 arXiv v1 공식 발행(2026-04-27)은 기존 Wiki에 04-25~26에 이미 축적된 MathDuels 프레임워크의 내용을 확정한다. 기존에 '3단계 적대적 문제 생성 파이프라인(기초→난이도 상향→적대적 프롬프팅)'으로 요약된 구조가 공식적으로 검증되었으며, 특히 세 번째 단계의 'adversarial prompting'이 기존 Wiki의 `adversarial-prompting` 개념(Box Maze 등에서 주로 안전 우회 맥락으로 사용되던)을 **평가 생성** 맥락으로 확장하는 교차점을 제공한다.

## 새로운 관점

기존 Wiki가 MathDuels를 주로 '천장 성능 문제 해결'으로 위치지었다면, 본 v1은 **근본적 평가 패러다임 전환**으로서의 위상을 강화한다: 고정 문제 집합에 대한 모델 순위가 아닌, 모델 간 상호 생성-해결 역학 자체를 평가 대상으로 삼는다는 점에서 `evaluator-assumption`의 '사전 정의된 문제 공간' 가정을 구조적으로 부정한다. 또한 `bidirectional-competency-asymmetry`(출제 능력과 해결 능력의 비대칭성)이 모델 간 차별화의 핵심 지표로 작동함을 확인한다.

## 다른 논문과의 연결점

- **RoboGrid**(`robogrid`): 구문·행동·의미의 분리 스트레스 테스트가 MathDuels의 '출제-해결 분리'와 구조적으로 유사하며, 두 논문 모두 단일 축 평가의 모호성을 해결하기 위해 평가 차원 자체를 분해한다.
- **SWE-chat**(`swe-chat`): 야생 환경에서의 에이전트 평가가 정적 벤치마크의 한계를 보여준다면, MathDuels는 이를 **평가 생성 구조** 차원에서 해결하는 상보적 경로를 제시한다.
- **Bounding the Black Box**(`statistical-certification`): 통계적 경계로 모델 능력 차이를 정량화하려는 시도와 MathDuels의 모델 간 상호 구별 가능성(discriminability) 목표가 방법론적 수준에서 수렴한다.

## 🔗 관련 논문

- 2026 04 24 diagnosing cfg interpretation in llms
- 2026 04 24 swe chat coding agent interactions from real users
- 2026 04 25 bounding the black box a statistical certification
- 2026 04 26 revisiting non verbatim memorization in large lang

## 🏷️ 엔티티

- [[entities/mathduels.md|mathduels]]
- [[entities/adversarial-problem-generation.md|adversarial-problem-generation]]
- [[entities/ceiling-performance-problem.md|ceiling-performance-problem]]
- [[entities/self-play-benchmark.md|self-play-benchmark]]
- [[entities/dual-role-evaluation.md|dual-role-evaluation]]
- [[entities/llm-benchmark.md|llm-benchmark]]
- [[entities/evaluator-assumption.md|evaluator-assumption]]
- [[entities/solver-poser-decoupling.md|solver-poser-decoupling]]
- [[entities/bidirectional-competency-asymmetry.md|bidirectional-competency-asymmetry]]
- [[entities/dynamic-evaluation-landscape.md|dynamic-evaluation-landscape]]

## 📐 개념

- [[concepts/adversarial-problem-generation.md|adversarial-problem-generation]]
- [[concepts/self-play-benchmark.md|self-play-benchmark]]
- [[concepts/dual-role-evaluation.md|dual-role-evaluation]]
- [[concepts/ceiling-performance-problem.md|ceiling-performance-problem]]
- [[concepts/solver-poser-decoupling.md|solver-poser-decoupling]]
- [[concepts/bidirectional-competency-asymmetry.md|bidirectional-competency-asymmetry]]
- [[concepts/dynamic-evaluation-landscape.md|dynamic-evaluation-landscape]]

---
_LLM 분석으로 생성됨_
