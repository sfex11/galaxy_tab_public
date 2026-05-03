# RAD-AI: Rethinking Architecture Documentation for AI-Augmented Ecosystems

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-31
**링크**: http://arxiv.org/abs/2603.28735v1

## 💡 핵심 인사이트

기존 소프트웨어 아키텍처 문서화 프레임워크(arc42, C4)는 AI의 확률적 행동과 데이터 의존적 진화를 포착할 수 없으며, 이 격차는 규제 준수에 실질적 위험을 초래한다.

## 📖 분석

## RAD-AI: AI 증강 생태계를 위한 아키텍처 문서화 재고

RAD-AI는 AI 증강 생태계(AI-augmented ecosystems)를 위한 새로운 아키텍처 문서화 프레임워크를 제안한다. 스마트 시티, 자율주행 차량 플릿, 지능형 플랫폼 등에서 다수의 AI 컴포넌트가 공유 데이터와 인프라를 통해 상호작용하는 시스템이 보편화되고 있으나, 기존의 arc42나 C4 모델 같은 아키텍처 문서화 프레임워크는 결정론적 소프트웨어를 전제로 설계되어 확률적 행동, 데이터 의존적 진화, ML/소프트웨어 이중 생명주기를 포착하지 못한다.

이 논문의 핵심 기여는 세 가지다. 첫째, 기존 문서화 프레임워크의 한계를 체계적으로 분석한다. 둘째, AI 컴포넌트의 확률적 특성과 데이터 파이프라인 의존성을 반영하는 확장된 문서화 구조를 제안한다. 셋째, 규제 준수(regulatory compliance) 관점에서 문서화 격차가 갖는 실질적 위험을 논의한다.

이 연구는 AI 시스템의 설계와 운영을 문서화하는 방법론적 전환을 촉구하며, 특히 [[concepts/ai-safety.md|ai safety]] 및 [[entities/llm-agent.md|llm agent]] 분야에서 논의되는 신뢰성·안전성 문제와 직접 연결된다. AI 에이전트가 복잡한 생태계 내에서 자율적으로 동작할 때, 그 행동의 문서화와 추적 가능성은 곧 안전성의 전제 조건이 된다. 또한 [[concepts/multi-agent-system.md|multi agent system]]에서 다수 에이전트 간 상호작용 패턴을 문서화하는 데에도 RAD-AI의 접근법이 적용될 수 있다.

## 🔗 관련 논문

- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 09 who governs the machine a machine identity governa
- 2026 04 11 psi shared state as the missing layer for coherent

## 📐 개념

- [[concepts/ai-architecture-documentation.md|ai-architecture-documentation]]
- [[concepts/ai-augmented-ecosystem.md|ai-augmented-ecosystem]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[concepts/ontological-architecture-redesign.md|ontological architecture redesign]]
