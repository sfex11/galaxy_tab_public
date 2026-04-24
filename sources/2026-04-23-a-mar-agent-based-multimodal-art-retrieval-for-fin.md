# A-MAR: Agent-based Multimodal Art Retrieval for Fine-Grained Artwork Understanding

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-23
**링크**: http://arxiv.org/abs/2604.19689v1

## 💡 핵심 인사이트

검색을 추론 계획에 명시적으로 조건화함으로써, MLLM의 암묵적 지식 의존이라는 인식론적 한계를 아키텍처 수준에서 해결하고 미술 작품 이해의 근거 가능성(traceability)을 확보한다.

## 📖 분석

# A-MAR: Agent-based Multimodal Art Retrieval

## 정의
미술 작품의 미세한(fine-grained) 이해를 위해 구조화된 추론 계획에 기반하여 검색을 명시적으로 조건화하는 에이전트 기반 멀티모달 미술 검색 프레임워크.

## 기존 Wiki와의 관계

### RAG 패러다임의 확장: 검색→생성에서 추론→검색→생성으로
기존 [[concepts/retrieval-augmented-generation.md|retrieval augmented generation]]은 검색 후 생성하는 선형 파이프라인을 전제하지만, A-MAR은 **추론 계획(reasoning plan)을 먼저 수립하고, 이 계획에 검색을 명시적으로 조건화**한다는 점에서 질적 차이가 있다. 이는 Wiki의 [[concepts/epistemic-fidelity.md|epistemic fidelity]](인식론적 충실도) 개념과 직결된다—암묵적 지식에 의존하는 MLLM의 한계를 "검색 충실도"가 아닌 "증거 기반 충실도"로 극복하려는 시도다.

### 추론 무결성과의 연결
[[concepts/reasoning-integrity.md|reasoning integrity]]와 [[concepts/process-control-architecture.md|process control architecture]]의 맥락에서, A-MAR의 구조화된 추론 계획은 사후 검증이 아닌 **아키텍처 수준에서 추론 경로를 구조화**하는 접근법이다. Box Maze가 프로세스 제어로 추론 무결성을 강제한다면, A-MAR은 검색 조건화로 추론의 근거(traceability)를 강제한다.

### 에이전트 아키텍처로서의 위치
[[entities/llm-agent.md|llm agent]]의 97편 합성 분석에서 "능력 확장" 축에 해당하며, 특히 미술이라는 문화적·역사적 맥락이 요구되는 도메인에서 [[concepts/evidence-fusion.md|evidence fusion]]과 [[concepts/visual-grounding.md|visual grounding]]을 결합하는 사례다.

## 핵심 구조
1. 쿼리 분해 → 구조화된 추론 계획 수립
2. 계획에 조건화된 멀티모달 검색
3. 검색된 증거에 기반한 명시적 근거 생성

이 구조는 [[concepts/structure-level-integrity-enforcement.md|structure level integrity enforcement]](구조 수준 무결성 강제)의 도메인 특화 적용이라고 볼 수 있다.

## 🔗 관련 논문

- 2026 04 22 mass rag multi agent synthesis retrieval augmented
- 2026 04 22 using large language models for embodied planning

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/multi-agent-system.md|multi-agent-system]]
- [[entities/vlm.md|vlm]]

## 📐 개념

- [[concepts/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[concepts/reasoning-chain.md|reasoning-chain]]
- [[concepts/evidence-fusion.md|evidence-fusion]]
- [[concepts/visual-grounding.md|visual-grounding]]
- [[concepts/epistemic-fidelity.md|epistemic-fidelity]]
- [[concepts/reasoning-conditioned-retrieval.md|reasoning-conditioned-retrieval]]
- [[concepts/structure-level-integrity-enforcement.md|structure-level-integrity-enforcement]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-04-22-mass-rag-multi-agent-synthesis-retrieval-augmented]]: 둘 다 에이전트 기반 접근으로 검색 품질을 향상시키며, 하나는 노이즈가 많은 일반 RAG 문맥을 다중 에이전트로 합성하고, 다른 하나는 구조화된 추론 계획으로 미술 작품 검색을 조건화한다.
