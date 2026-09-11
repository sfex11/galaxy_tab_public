# Glyph: A Multi-Strategy Agentic System for Column Description and Sensitivity-Ontology Tagging of Enterprise Data Catalogs

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-11
**링크**: http://arxiv.org/abs/2609.10430v1

## 💡 핵심 인사이트

데이터 거버넌스의 진짜 병목은 정책 부재가 아니라 메타데이터 생산 부채이며, LLM 에이전트 협업으로 생산을 자동화하면 의미론적 메타데이터는 오버헤드가 아니라 자동 갱신되는 1급 자산이 된다.

## 📖 분석

Glyph는 엔터프라이즈 데이터 레이크의 문서화 부채(컬럼 설명 누락, 거버넌스 라벨 미할당)를 컬럼 설명 생성과 민감도 타입 주석이라는 두 개의 결합된 문제로 공식화하고, 상태 그래프로 오케스트레이션되는 협업 LLM 에이전트(Descriptor, Tagger)로 해결하는 프로덕션 시스템이다. 본 논문은 [[semantic-metadata-eliminability-hypothesis]]에 대한 중요한 보완 관점을 제공한다 — 기존 가설이 메타데이터를 에이전트 파이프라인의 오버헤드로 보았다면, Glyph는 메타데이터 생산 자체를 LLM 에이전트의 태스크로 재정의하여, 문제의 본질이 '메타데이터의 가치'가 아니라 '인간 기반 생산의 병목'이었음을 드러낸다. Descriptor와 Tagger의 이원 협업 구조는 [[multi-agent-system]]의 하위 문제 분해 사례를 추가하며, 상태 그래프 오케스트레이션은 [[agent-loop-as-computation]]의 구현 축을 강화한다. 민감도 온톨로지 태깅은 [[ai-governance]]의 규제 준수를 데이터 스키마 계층의 자동 갱신 아티팩트로 하류화하여, 거버넌스가 문서가 아닌 지속 생성되는 산출물이 되는 방향을 시사한다.

## 🔗 관련 논문

- Trust-Aware Adaptive Disclosure for Inference Privacy Preservation in Multi-Agent Systems
- Multi-Step Tool-Calling over Korean Open Public APIs: A Benchmark and Agent Framework
- The Natural Language Interaction Protocol and Standard for AI Agents

## 🏷️ 엔티티

- [[entities/multi-agent-system.md|multi-agent-system]]
- [[entities/llm-agent.md|llm-agent]]
- [[entities/ai-governance.md|ai-governance]]
- [[entities/semantic-metadata-eliminability-hypothesis.md|semantic-metadata-eliminability-hypothesis]]
- [[entities/documentation-debt.md|documentation-debt]]
- [[entities/glyph-system.md|glyph-system]]
- [[entities/metadata-generation-automation.md|metadata-generation-automation]]
- [[entities/sensitivity-ontology-tagging.md|sensitivity-ontology-tagging]]

## 📐 개념

- [[concepts/multi-strategy-agentic-system.md|multi-strategy-agentic-system]]
- [[concepts/stateful-graph-orchestration.md|stateful-graph-orchestration]]
- [[concepts/coupled-problem-decomposition.md|coupled-problem-decomposition]]
- [[concepts/column-description-generation.md|column-description-generation]]
- [[concepts/governance-label-automation.md|governance-label-automation]]

---
_LLM 분석으로 생성됨_
