# Large Language Models as Falsifiers for Cyber-Physical Systems

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-19
**링크**: http://arxiv.org/abs/2609.20752v1

## 💡 핵심 인사이트

LLM이 명세를 만족시키는 해결자를 넘어 명세를 위반시키는 반증자로 기능할 수 있음을 보여, 형식적 안전 보장의 쌍대인 적대적 반례 탐색을 LLM의 새로운 응용 영역으로 개방한다.

## 📖 분석

LLM-Falsifier는 CPS의 STL 명세 위반 반례를 탐색하는 반증(falsification) 작업을, 반복적 프롬프팅으로 결합된 LLM 격자 최적화기로 수행하는 프레임워크다. 전통적 블랙박스 탐색 알고리즘을 LLM 기반 탐색으로 대체한다.

**형식 검증의 쌍대**: 기존 [[formal-verification]]이 검증(verification, 명세 만족 증명) 측을 다뤘다면, 본 논문은 쌍대인 반증 측을 LLM에 위임한다. 검증이 '안전함을 증명'이라면 반증은 '불안전함을 찾는' 적대적 탐색이며, [[statistical-certification]]이 확률적 보장(위반 확률 상한)을 제공하는 것과 달리 결정론적 반례를 산출한다.

**삼분법의 제4 역할**: [[solver-poser-decoupling]]이 해결자-출제자에 검증자를 추가해 삼분법을 완성했다면, 반증자(falsifier)는 제4 역할로 확장된다. 반증자는 시스템의 실패 모드를 능동적으로 찾는 주체로, 판단자([[llm-as-judge]])나 생성자([[verifier-backed-generation]])와 다른 기능적 위치를 점유한다.

**적대적 생성과의 구별**: [[adversarial-problem-generation]]이 평가용 난제를 생성하는 것과 달리, 반증은 기존 시스템의 명세 위반을 탐색한다. 전자는 새로운 테스트를 만들어 문제 공간을 넓히고, 후자는 기존 시스템의 실패 공간을 조사한다.

**안전성 검증 계층**: 이 접근은 배포 전 반례 탐색을 자동화하여 [[auditability-as-scaling-requirement]]에 대응하는 능동적 안전 검증 계층을 제공한다. 반증 성공은 안전 보장의 부정적 증거가 되며, 반증 실패는 그 자체로 안전에 대한 긍정적 신호가 아니다(탐색 실패 ≠ 안전 보장).

## 🔗 관련 논문

- Verifier-Backed Hard Problem Generation for Mathematical Reasoning
- Corrupt Plans, Clean Traces: Evading Chain-of-Thought Monitoring
- Monitoring and Discovering Reward Hacking with Internal Representation

## 🏷️ 엔티티

- [[entities/formal-falsification.md|formal-falsification]]
- [[entities/llm-falsifier.md|llm-falsifier]]
- [[entities/stl-robustness-optimization.md|stl-robustness-optimization]]
- [[entities/formal-verification.md|formal-verification]]
- [[entities/solver-poser-decoupling.md|solver-poser-decoupling]]
- [[entities/adversarial-problem-generation.md|adversarial-problem-generation]]
- [[entities/statistical-certification.md|statistical-certification]]
- [[entities/verification-as-system-external-relation.md|verification-as-system-external-relation]]

## 📐 개념

- [[concepts/formal-falsification.md|formal-falsification]]
- [[concepts/llm-falsifier.md|llm-falsifier]]
- [[concepts/stl-robustness-optimization.md|stl-robustness-optimization]]
- [[concepts/iterative-prompting-optimization.md|iterative-prompting-optimization]]
- [[concepts/counterexample-search.md|counterexample-search]]
- [[concepts/falsifier-as-fourth-role.md|falsifier-as-fourth-role]]

---
_LLM 분석으로 생성됨_
