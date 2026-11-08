# SwarmEvolve: Latent Agent Swarms for Evolutionary Discovery and Optimization

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-08
**링크**: http://arxiv.org/abs/2611.08483v1

## 💡 핵심 인사이트

LLM 유도 진화 탐색의 병목은 추론 능력이 아니라 개체군 다양성 유지를 위한 반복 텍스트 CoT 디코딩 비용이며, 디코딩 없는 잠재 추론 스웜으로 이를 제거하는 순간 외생 진화의 실용 조건이 성립한다.

## 📖 분석

v1 정식 발행으로 원천 정의가 확정된다 — LLM 유도 진화 탐색의 병목이 추론 능력 부족이 아니라, 개체군 다양성을 유지하기 위해 매 라운드 반복 생성해야 하는 긴 텍스트 CoT의 디코딩 비용임을 명시하고, 이를 라운드당 수백 명의 저비용 에이전트가 디코딩 없이 잠재 공간에서 추론하는 스웜 구조로 제거하는 프레임워크다.

[[concepts/evolutionary-hypothesis-search.md|evolutionary hypothesis search]]의 HypoEvolve가 유전 알고리즘으로 과학 가설 발견을 수행했다면, 본 논문은 수학·계산 문제의 프로그램 개선에 적용하여 진화적 발견의 도메인 스펙트럼을 확장한다. 핵심 통찰은 [[concepts/exogenous-evolution.md|exogenous evolution]]의 경제학을 기제 수준에서 뒷받침하는 것 — 변이 비용이 텍스트 디코딩에 종속된 한 외생 진화는 비실용적이었으나, [[concepts/latent-variation-operator.md|latent variation operator]]가 잠재 추론으로 구현되면 병렬 개체군 탐색이 실용 가능해진다.

[[concepts/continuous-latent-reasoning.md|continuous latent reasoning]] 계열과 구별되는 점은 잠재 추론의 목적이 단일 궤적의 품질이 아니라 병렬 다양성 유지라는 점이며, [[concepts/agent-loop-as-computation.md|agent loop as computation]] 관점에서 진화 루프 전체의 비용 구조를 저비용 연산 단위로 재구성한 사례로 읽힌다.

## 🔗 관련 논문

- SwarmEvolve: Latent Agent Swarms for Evolutionary Discovery and Optimization

## 🏷️ 엔티티

- [[entities/swarm-evolve.md|swarm-evolve]]
- [[entities/exogenous-evolution.md|exogenous-evolution]]
- [[entities/evolutionary-agency-axis.md|evolutionary-agency-axis]]
- [[entities/evolutionary-hypothesis-search.md|evolutionary-hypothesis-search]]
- [[entities/latent-variation-operator.md|latent-variation-operator]]
- [[entities/continuous-latent-reasoning.md|continuous-latent-reasoning]]
- [[entities/agent-loop-as-computation.md|agent-loop-as-computation]]
- [[entities/swarm-scale-evolutionary-search.md|swarm-scale-evolutionary-search]]
- [[entities/code-as-evolution-unit.md|code-as-evolution-unit]]

## 📐 개념

- [[concepts/latent-variation-operator.md|latent-variation-operator]]
- [[concepts/continuous-latent-reasoning.md|continuous-latent-reasoning]]
- [[concepts/swarm-scale-evolutionary-search.md|swarm-scale-evolutionary-search]]
- [[concepts/evolutionary-cross-pollination.md|evolutionary-cross-pollination]]
- [[concepts/exogenous-evolution.md|exogenous-evolution]]

---
_LLM 분석으로 생성됨_
