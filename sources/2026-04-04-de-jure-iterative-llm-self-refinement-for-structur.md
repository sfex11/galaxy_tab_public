# De Jure: Iterative LLM Self-Refinement for Structured Extraction of Regulatory Rules

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-04
**링크**: http://arxiv.org/abs/2604.02276v1

## 💡 핵심 인사이트

인간 어노테이션 없이 LLM의 반복적 자기 정제만으로 복잡한 계층적 법률 텍스트를 구조화된 규칙으로 변환할 수 있으며, 이는 도메인 비의존적 규제 준수 자동화의 실용적 경로를 제시한다.

## 📖 분석

## De Jure: 규제 문서에서 구조화된 규칙 자동 추출을 위한 반복적 LLM 자기 정제

De Jure는 법률·규제 문서에서 기계 판독 가능한 구조화 규칙을 자동 추출하는 완전 자동화 파이프라인이다. 인간 어노테이션, 도메인 특화 프롬프팅, 골드 데이터 없이 작동하며, 네 단계 순차 처리(정규화 → 추출 → 정제 → 검증)를 통해 계층적 법률 텍스트를 구조화한다.

### 핵심 메커니즘

파이프라인의 가장 차별적 요소는 **반복적 자기 정제(iterative self-refinement)** 단계로, LLM이 자체 출력을 평가하고 오류를 수정하는 피드백 루프를 형성한다. 이는 [[concepts/reasoning-integrity.md|reasoning integrity]]와 직결되는 접근으로, 단일 패스 추출의 한계를 극복한다. 또한 도메인 비의존적(domain-agnostic) 설계를 채택하여 금융, 의료, 환경 등 다양한 규제 영역에 범용 적용이 가능하다.

### Wiki 연결점

**프로세스 제어 아키텍처와의 유사성**: Box Maze가 LLM 추론의 신뢰성을 위해 다단계 프로세스 제어를 도입한 것처럼, De Jure도 순차적 단계 분리와 자기 검증 메커니즘으로 추출 품질을 보장한다. **구조적 매핑**: 비정형 텍스트에서 정형 규칙을 추출하는 과정은 [[concepts/structural-mapping.md|structural mapping]] 연구와 방법론적 교차점을 가진다. **요구사항 공학**: ReqFusion이 다중 LLM 제공자를 활용해 소프트웨어 요구사항을 자동 분석한 것과 유사하게, De Jure는 규제 요구사항의 자동 구조화에 초점을 둔다.

### 시사점

LLM 기반 규제 준수(compliance) 자동화는 AI 거버넌스 논의에서 점점 중요해지고 있으며, De Jure의 어노테이션 프리 접근은 실무 배포 장벽을 크게 낮춘다.

## 🔗 관련 논문

- Box Maze: A Process-Control Architecture for Reliable LLM Re
- Enhancing Structural Mapping with LLM-derived Abstractions f
- ReqFusion: A Multi-Provider Framework for Automated PEGS Ana
- Evaluating the Reliability and Fidelity of Automated Judgmen

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/reasoning-integrity.md|reasoning-integrity]]
- [[concepts/structural-mapping.md|structural-mapping]]
- [[concepts/requirements-engineering.md|requirements-engineering]]
- [[concepts/process-control-architecture.md|process-control-architecture]]
- [[concepts/prompt-engineering.md|prompt-engineering]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[entities/event-extraction.md|event extraction]]

---
**관련**: [[concepts/experience-dynamics-extraction-gap.md|experience dynamics extraction gap]]

---
**관련**: [[concepts/regulatory-vacuity.md|regulatory vacuity]]

---
**관련**: [[concepts/event-extraction.md|event extraction]]
