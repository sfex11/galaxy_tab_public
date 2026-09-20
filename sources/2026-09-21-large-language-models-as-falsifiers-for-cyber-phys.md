# Large Language Models as Falsifiers for Cyber-Physical Systems

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-21
**링크**: http://arxiv.org/abs/2609.20752v1

## 💡 핵심 인사이트

STL 견고성처럼 결정론적 오라클이 주어지면 LLM은 경사 없이 반복 프롬프팅만으로 검증의 쌍대인 반례 탐색 최적화를 수행할 수 있으며, 이는 최적화의 병목이 미분 가능성이 아니라 목표의 언어적 기술 가능성임을 시사한다.

## 📖 분석

# Large Language Models as Falsifiers for Cyber-Physical Systems (2026-09-21)

## 핵심 기여
LLM-Falsifier는 STL 명세의 위반 반례 탐색(falsification)을 견고성 최적화 문제로 형식화하고, CMA-ES 같은 블랙박스 검색 대신 반복 프롬프팅으로 견고성 함수를 최적화하는 LLM을 배치한다. LLM은 시스템 동역학을 모른 채 평가 이력만으로 후보를 제안하며, STL 견고성이라는 결정론적 스칼라 오라클이 수렴 신호를 제공한다.

## 기존 Wiki와의 관계
- [[formal-verification]]의 쌍대 축: 검증이 안전 증명이라면 falsification은 위반 탐색이며, LLM을 증명자가 아닌 반증자로 배치하는 역방향 활용이다.
- [[verification-as-system-external-relation]]의 CPS 확장: STL 견고성은 모델 출력과 독립적인 외부 신호로, 검증 가능성이 시스템-외부 관계라는 명제가 물리 도메인에서도 성립함을 보여준다.
- [[solver-poser-decoupling]] 이래 세분화된 역할 분리(출제자→검증자)에 반증자를 제4 역할로 추가한다([[falsifier-as-fourth-role]]).
- [[adversarial-problem-generation]]의 CPS 버전: 반례 생성은 적대적 문제 생성과 동형 구조다.
- [[iterative-prompting-optimization]]: 파인튜닝 없이 프롬프팅 루프만으로 최적화가 성립함을 입증하는 원천 사례다.

## 인사이트
경사 정보 없이 목표의 언어적 기술만으로 LLM이 최적화 동력이 될 수 있다는 발견은, 최적화의 병목이 미분 가능성이 아니라 목표 기술 가능성일 수 있음을 시사한다.

## 🔗 관련 논문

- sources/2026-09-19-large-language-models-as-falsifiers-for-cyber-phys.md
- sources/2026-05-10-verifier-backed-hard-problem-generation-for-mathem.md
- sources/2026-04-25-mathduels-evaluating-llms-as-problem-posers-and-so.md
- sources/2026-09-18-evidence-grounded-agentic-formulation-development-.md

## 🏷️ 엔티티

- [[entities/llm-falsifier.md|llm-falsifier]]
- [[entities/formal-falsification.md|formal-falsification]]
- [[entities/stl-robustness-optimization.md|stl-robustness-optimization]]
- [[entities/counterexample-search.md|counterexample-search]]
- [[entities/falsifier-as-fourth-role.md|falsifier-as-fourth-role]]
- [[entities/iterative-prompting-optimization.md|iterative-prompting-optimization]]
- [[entities/verification-as-system-external-relation.md|verification-as-system-external-relation]]
- [[entities/formal-verification.md|formal-verification]]

## 📐 개념

- [[concepts/stl-robustness-as-decision-oracle.md|stl-robustness-as-decision-oracle]]
- [[concepts/llm-as-blackbox-optimizer.md|llm-as-blackbox-optimizer]]
- [[concepts/verification-falsification-duality.md|verification-falsification-duality]]
- [[concepts/prompting-loop-as-search.md|prompting-loop-as-search]]

---
_LLM 분석으로 생성됨_
