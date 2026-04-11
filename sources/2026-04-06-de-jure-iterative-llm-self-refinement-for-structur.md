# De Jure: Iterative LLM Self-Refinement for Structured Extraction of Regulatory Rules

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-06
**링크**: http://arxiv.org/abs/2604.02276v1

## 💡 핵심 인사이트

LLM의 반복적 자기 정제(iterative self-refinement)만으로 외부 어노테이션 없이 법률 텍스트에서 구조화된 규칙을 추출할 수 있으며, 이는 AI 규제 준수 자동화의 핵심 빌딩 블록이 된다.

## 📖 분석

## De Jure: Iterative LLM Self-Refinement for Structured Extraction of Regulatory Rules

**De Jure**는 규제 문서(regulatory documents)에서 구조화된 규칙을 자동으로 추출하는 완전 자동화 파이프라인이다. 인간 어노테이션, 도메인 특화 프롬프팅, 골드 데이터 없이 작동하며, 4단계 순차 처리(정규화 → 규칙 추출 → 자기 정제 → 구조화)를 통해 법적 텍스트를 머신 리더블 규칙으로 변환한다.

### 핵심 기여

- **LLM 자기 정제(Self-Refinement)**: 추출된 규칙을 LLM이 반복적으로 검증·수정하는 iterative refinement 루프를 도입하여, 외부 검증자 없이도 추출 품질을 향상시킨다. 이는 [[reasoning-integrity]] 연구에서 다루는 LLM 출력 신뢰성 문제와 직접 연결된다.
- **도메인 비의존적 설계**: 특정 법률 도메인에 종속되지 않아, 다양한 규제 영역에 범용 적용 가능하다. 이는 [[retrieval-augmented-generation]]이나 [[knowledge-injection]] 접근법과 달리 외부 지식 소스에 의존하지 않는 차별점이다.
- **계층적 법률 텍스트 처리**: 규제 문서의 계층 구조(조항, 항, 호)를 보존하며 추출하는 정규화 단계는 [[hierarchical-representation]] 개념과 맥을 같이한다.

### 기존 연구와의 연결

Box Maze의 [[process-control-architecture]]가 LLM 추론의 신뢰성을 제어 흐름으로 보장하려 했다면, De Jure는 자기 정제 루프를 통해 구조화된 출력의 정확성을 담보한다. 또한 [[ai-governance]] 관점에서, 규제 규칙의 자동 추출은 AI 시스템의 법적 준수(compliance) 자동화를 위한 기반 기술로 볼 수 있다. TraceSafe의 [[ai-safety]] 가드레일 평가와도 상보적 관계에 있다—De Jure가 규칙을 추출하면, 가드레일 시스템이 이를 실행한다.

## 🔗 관련 논문

- Box Maze: A Process-Control Architecture for Reliable LLM Re
- TraceSafe: A Systematic Assessment of LLM Guardrails on Mult
- Evaluating the Reliability and Fidelity of Automated Judgmen
- SPA: A Simple but Tough-to-Beat Baseline for Kno

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/reasoning-integrity.md|reasoning-integrity]]
- [[concepts/hierarchical-representation.md|hierarchical-representation]]
- [[concepts/ai-governance.md|ai-governance]]
- [[concepts/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[concepts/knowledge-injection.md|knowledge-injection]]
- [[concepts/process-control-architecture.md|process-control-architecture]]

---
_LLM 분석으로 재생성됨_
