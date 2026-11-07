# SwarmEvolve: Latent Agent Swarms for Evolutionary Discovery and Optimization

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-07
**링크**: http://arxiv.org/abs/2611.08483v1

## 💡 핵심 인사이트

잠재 공간 추론이 진화 탐색의 개체군 규모 병목(세대별 반복 CoT 생성 비용)을 제거하여, LLM 유도 진화의 경제성이 디코딩 비용에서 분리될 수 있음을 보여준다.

## 📖 분석

SwarmEvolve는 LLM 유도 진화 탐색의 병목을 인프라 계층에서 해소한다. 기존 진화 탐색에서는 매 세대마다 긴 텍스트 CoT를 생성하고 개체군 다양성 유지를 위해 이를 반복해야 했으나, 본 논문은 세대당 수백 개의 저비용 에이전트가 스웜으로 작동하며 디코딩 없이 잠재 공간에서 추론하는 구조를 제시한다.

핵심 기여는 [[continuous-latent-reasoning]] 계열의 잠재 추론 원리를 진화적 프로그램 개선 에이전트로 이식한 것이다 — 잠재 추론의 가치가 단일 추론의 품질·속도 문제에서 '개체군 규모의 경제성' 문제로 확장됨을 보여준다. 이는 [[exogenous-evolution]]의 비용 전제를 재정의한다: 에이전트가 변이 연산자로 기능하고 선택 압력은 외부 진화 루프가 가하는 구조([[evolutionary-agency-axis]])는 유지되되, 변이 연산 단가의 절감으로 수백 개체 스웜 탐색이 실용 가능해진다. 고득점 방법의 결합이 스웜 내부에서 이루어진다는 점에서 [[evolutionary-cross-pollination]]의 기제도 개체군 내부로 내재화된다.

[[evolutionary-hypothesis-search]]의 HypoEvolve가 유전 알고리즘 기반 가설 발견이었다면 본 논문은 동일 진화 패러다임의 병목이 CoT 생성 비용임을 진단하고 인프라 계층에서 해소한다. 진화 탐색 연구의 개선 축이 알고리즘(선택·변이 설계)에서 추론 인프라로 이동했음을 확정하며, 수백 에이전트의 잠재 공간 병렬 작동은 [[latent-inter-agent-communication]]과 [[agent-loop-as-computation]]의 교차점이기도 하다.

## 🔗 관련 논문

- HypoEvolve: Genetic Algorithms Enable Multi-Agent LLMs to Discover Scientific Hypotheses (2026-09-16)
- Strategist: Evolving Reasoning with Agents (2026-11-04)
- Latent Reasoning in Continuous Space for Unified Multimodal Models (2026-11-03)
- Learning to Communicate: Toward End-to-End Optimization of Multi-Agent Systems

## 🏷️ 엔티티

- [[entities/swarm-evolve.md|swarm-evolve]]
- [[entities/exogenous-evolution.md|exogenous-evolution]]
- [[entities/continuous-latent-reasoning.md|continuous-latent-reasoning]]
- [[entities/evolutionary-hypothesis-search.md|evolutionary-hypothesis-search]]
- [[entities/latent-inter-agent-communication.md|latent-inter-agent-communication]]
- [[entities/agent-loop-as-computation.md|agent-loop-as-computation]]
- [[entities/code-as-evolution-unit.md|code-as-evolution-unit]]
- [[entities/evolutionary-agency-axis.md|evolutionary-agency-axis]]

## 📐 개념

- [[concepts/latent-variation-operator.md|latent-variation-operator]]
- [[concepts/swarm-scale-evolutionary-search.md|swarm-scale-evolutionary-search]]

---
_LLM 분석으로 생성됨_
