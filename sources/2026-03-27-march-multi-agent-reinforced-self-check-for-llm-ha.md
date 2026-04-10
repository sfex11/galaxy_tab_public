# MARCH: Multi-Agent Reinforced Self-Check for LLM Hallucination

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-27
**링크**: http://arxiv.org/abs/2603.24579v1

## 💡 핵심 인사이트

LLM 환각 탐지에서 단일 검증자의 확인 편향을 다중 에이전트 강화학습 기반 교차 검증으로 극복하는 접근은, LLM-as-a-judge 패러다임의 구조적 한계를 멀티 에이전트 시스템으로 해결하는 새로운 방향을 제시한다.

## 📖 분석

## MARCH: Multi-Agent Reinforced Self-Check for LLM Hallucination

**핵심 문제**: LLM의 환각(hallucination)은 특히 RAG 시스템에서 신뢰성을 저해하는 핵심 병목이다. 기존 LLM-as-a-judge 방식의 환각 탐지는 검증자가 원본 생성의 오류를 무의식적으로 재생산하는 **확인 편향(confirmation bias)** 문제를 안고 있다.

**제안 방법**: MARCH는 다중 에이전트 강화학습 기반의 자기 검증 프레임워크를 도입한다. 단일 검증자 대신 여러 에이전트가 독립적으로 LLM 출력을 검증하고, 강화학습을 통해 검증 정확도를 점진적으로 개선한다. 이는 단일 판단자의 편향을 다중 관점으로 상쇄하는 전략이다.

**기존 Wiki와의 연결**:
- [[multi-agent-system]]: MARCH의 다중 에이전트 검증 구조는 멀티 에이전트 시스템의 집단 지성 원리를 환각 탐지에 적용한 사례다.
- [[reinforcement-learning]]: 검증 에이전트의 학습에 강화학습을 활용하여, 단순 프롬프팅 기반 검증을 넘어선 적응적 검증 능력을 구현한다.
- [[retrieval-augmented-generation]]: RAG 파이프라인에서의 환각 문제를 직접 타겟으로 하며, 검색된 증거 대비 생성 결과의 충실성을 검증한다.
- [[reasoning-integrity]]: Box Maze 등 기존 연구가 LLM 추론의 신뢰성을 구조적으로 보장하려 했다면, MARCH는 출력 후 검증 단계에서 신뢰성을 확보하는 상보적 접근이다.
- [[adversarial-prompting]]: 확인 편향을 극복하기 위한 다중 에이전트 교차 검증은 적대적 검증(adversarial verification)과 유사한 효과를 낸다.

**인사이트**: 단일 LLM 판단자의 한계를 인정하고, 강화학습으로 훈련된 다중 에이전트 간 상호 검증으로 이를 극복하려는 시도는 LLM 자기 평가 패러다임의 중요한 진화 방향을 제시한다.

## 🔗 관련 논문

- 2026 03 22 box maze a process control architecture for reliab
- 2026 04 09 social dynamics as critical vulnerabilities that u
- 2026 04 09 paper circle an open source multi agent research d
- 2026 03 25 evaluating the reliability and fidelity of automat
- 2026 04 10 a systematic study of retrieval pipeline design fo

## 🏷️ 엔티티

- [[entities/llm.md|llm]]
- [[entities/multi-agent-system.md|multi-agent-system]]

## 📐 개념

- [[concepts/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/reasoning-integrity.md|reasoning-integrity]]
- [[concepts/adversarial-prompting.md|adversarial-prompting]]
- [[concepts/multi-agent-system.md|multi-agent-system]]

---
_LLM 분석으로 재생성됨_
