# Re-Search: Dissecting LLM Ideation Through a Two-Player Questioning Game

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-12
**링크**: http://arxiv.org/abs/2611.14487v1

## 💡 핵심 인사이트

아이디어화 능력은 최종 아이디어의 품질이 아니라, 유한 질의 예산 하에서 상대의 지식 상태를 모델링하며 탐색 공간을 좁혀가는 동역학으로 측정해야 한다.

## 📖 분석

## Re-Search: Dissecting LLM Ideation Through a Two-Player Questioning Game

연구 아이디어화(ideation)를 이십 문제(Twenty Questions) 형식으로 조작화한 평가 프레임워크다. 200개 ICML 논문에서 발표된 연구 문제만을 주고, 모델이 yes/no 질문을 반복하여 그 논문의 핵심 아이디어를 '재발견'해야 한다. 기존 아이디어 평가가 최종 산출물의 품질만 측정해 탐색 과정을 가렸다면, Re-Search는 아이디어 공간에서의 탐색 궤적 자체를 관찰 가능하게 만든다.

### Wiki 기존 개념과의 연결

**question-generation-as-belief-modeling**과 **prior-weighted-bisection**의 평가 도메인 실현이다. 질문 생성을 상대(논문 저자)의 신념·지식 상태에 대한 모델링으로 본 위키 논의에 대해, Re-Search는 '논문 아이디어'라는 고정 타겟의 재발견 게임을 통해 그 능력을 통제 조건에서 측정한다. 특히 사전분포 가중 이분 원리가 실제로 작동하는지 — 모델이 Zipf적 논문 주제 분포를 반영해 질문하는가 — 를 검증 가능한 채널로 만든다.

**exact-entropy-question-budget**의 최소 질의 상한이 최적 차수 천장처럼 작동하며, 모델 실성능과의 격차가 정보 이론적 병목([[capacity-achievability-dichotomy]])의 아이디어화 도메인 사례가 된다. 이는 인터랙티브 검색 게임을 통한 능력 진단이라는 점에서 ideasambig와 상보적이다: IdeaAMBIG이 아이디어→명세의 간극을 측정한다면 Re-Search는 문제→아이디어의 탐색 간극을 측정한다.

**bidirectional-competency-asymmetry**의 새 축도 제공한다 — MathDuels가 출제-해결 역량 비대칭을 다뤘다면, Re-Search는 질문-응답 구도에서 질문자(탐색자)의 병목을 격리한다.

### 방법론적 의의

반복적 개선을 평가에 내장하여, 아이디어 품질을 정적 특성이 아닌 탐색 동역학(수렴 속도, 질문 효율, 조기 수렴 여부)으로 재정의한다. 이는 [[dynamic-evaluation-landscape]]와 alternatives-decision-trajectory 계열의 '결정 공간 관찰' 패러다임이 연구 아이디어 도메인으로 확장된 사례다.

## 🔗 관련 논문

- Quantifying Overclaiming Propensity in Frontier LLM Agents
- Playing log(N)-Questions over Wikipedia Abstracts: Communication Effic
- MathDuels: Evaluating LLMs as Problem Posers and Solvers
- Verifier-Backed Hard Problem Generation for Mathematical Reasoning

## 🏷️ 엔티티

- [[entities/question-generation-as-belief-modeling.md|question-generation-as-belief-modeling]]
- [[entities/prior-weighted-bisection.md|prior-weighted-bisection]]
- [[entities/exact-entropy-question-budget.md|exact-entropy-question-budget]]
- [[entities/bidirectional-competency-asymmetry.md|bidirectional-competency-asymmetry]]
- [[entities/dynamic-evaluation-landscape.md|dynamic-evaluation-landscape]]
- [[entities/ideaambig.md|ideaambig]]

## 📐 개념

- [[concepts/탐색-궤적-조작화.md|탐색 궤적 조작화]]
- [[concepts/재발견-게임-평가.md|재발견 게임 평가]]
- [[concepts/아이디어-공간-탐색-동역학.md|아이디어 공간 탐색 동역학]]
- [[concepts/질문-기반-아이디어-진단.md|질문 기반 아이디어 진단]]
- [[concepts/정보-이론적-질의-예산.md|정보 이론적 질의 예산]]

---
_LLM 분석으로 생성됨_
