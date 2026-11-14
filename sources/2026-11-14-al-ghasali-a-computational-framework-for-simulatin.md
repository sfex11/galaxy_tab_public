# Al-Ghasali: A Computational Framework for Simulating Islamic Jurisprudential Rulings via Finite State Automata and Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-14
**링크**: http://arxiv.org/abs/2611.17235v1

## 💡 핵심 인사이트

폐쇄된 규칙 도메인의 자연어 형식화는 결정론적 유한 상태 오토마타로 완전 붕괴할 수 있으며, 형식화 제약의 수준이 도달 가능한 계산 클래스를 결정한다 — NL→형식 번역의 난이도는 도메인의 개방성에 조건부다.

## 📖 분석

# Al-Ghasali: FSA와 LLM을 통한 이슬람 법학(Fiqh) 판결 시뮬레이션 (2026-11-14)

al-Sabr wa al-Taqsim의 집합론적 형식화에서 추출된 최소 운영 규칙(Horn 절)을 기반으로, 폐쇄된 Fiqh 장(chapter)의 의미론이 결정론적 유한 상태 오토마타(FSA)로 완전 붕괴함을 증명한다. 형식화 제약 완화에 따른 계산 위계를 제시하며, LLM이 NL 판례 텍스트의 형식화를 담당하는 하이브리드 프레임워크다.

## 기존 Wiki와의 관계

[[natural-language-to-formal-language]] 논의에 법·종교 도메인 사례를 추가한다. from-natural-language-to-exact-cover가 NL→NP 조합 문제 환원을 보였다면, 본 논문은 NL→Horn 절→FSA의 2단계 컴파일 경로를 제시한다. 핵심은 '폐쇄성'이다 — 규칙 집합이 완결된 도메인에서는 형식화 대상이 결정론 기계로 수렴하며, 이는 [[stochastic-deterministic-boundary]]의 도메인 조건부 버전이다.

[[neuro-symbolic-division-of-labor]]의 법 도메인 실현: LLM은 파싱·형식화를, FSA는 판결의 결정론적 시뮬레이션·검증을 담당한다. [[external-layer-principle]]이 예측한 대로 판정 근거가 LLM 외부의 형식 체계에 귀속된다.

[[legal-domain-extraction]](ARGUS)과의 대비: ARGUS가 법률 문서를 서술적 사건 그래프로 추출했다면, 본 논문은 종교법을 실행 가능한 결정 의미론으로 컴파일한다. 법 형식화가 '표현(그래프)'과 '집행(오토마타)'의 상보적 양축으로 분화함을 보여준다.

[[formalization-plurality]]의 정교화: 형식화 제약 수준이 도달 가능한 계산 클래스를 결정하는 위계 제시는, 형식화 선택이 표현력-계산가능성 트레이드오프임을 입증한다.

## 🔗 관련 논문

- From Natural Language to Exact Cover: A Neuro-Symbolic Approach to Zebra Puzzle
- Syntax Is Easy, Semantics Is Hard: Evaluating LLMs for LTL Translation
- ARGUS: Role-Aware Event Knowledge Graphs for U.S. Employment-Discrimination
- Evaluating LLM-Generated World Models for Neuro-Symbolic Reasoning
- Diagnosing CFG Interpretation in LLMs

## 🏷️ 엔티티

- [[entities/al-ghasali.md|al-ghasali]]
- [[entities/natural-language-to-formal-language.md|natural-language-to-formal-language]]
- [[entities/neuro-symbolic-division-of-labor.md|neuro-symbolic-division-of-labor]]
- [[entities/from-natural-language-to-exact-cover.md|from-natural-language-to-exact-cover]]
- [[entities/legal-domain-extraction.md|legal-domain-extraction]]
- [[entities/formalization-plurality.md|formalization-plurality]]
- [[entities/stochastic-deterministic-boundary.md|stochastic-deterministic-boundary]]
- [[entities/external-layer-principle.md|external-layer-principle]]

## 📐 개념

- [[concepts/closed-domain-fsa-collapse.md|closed-domain-fsa-collapse]]
- [[concepts/formalization-computational-hierarchy.md|formalization-computational-hierarchy]]
- [[concepts/legal-rule-compilation.md|legal-rule-compilation]]

---
_LLM 분석으로 생성됨_
