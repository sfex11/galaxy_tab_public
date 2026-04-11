# Intertemporal Demand Allocation for Inventory Control in Online Marketplaces

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-10
**링크**: http://arxiv.org/abs/2604.07312v1

## 💡 핵심 인사이트

플랫폼이 재고를 직접 통제하지 않고도 시간간 수요 배분 전략만으로 분산된 판매자들의 재고 결정을 효과적으로 유도할 수 있음을 보여주며, 이는 중앙 통제 없는 다중 에이전트 조율의 경제학적 사례이다.

## 📖 분석

## Intertemporal Demand Allocation for Inventory Control in Online Marketplaces

본 논문은 온라인 마켓플레이스에서 플랫폼이 **시간간 수요 배분(intertemporal demand allocation)**을 통해 판매자의 재고 결정에 간접적으로 영향을 미치는 메커니즘을 연구한다. 플랫폼은 재고를 직접 통제하지 않지만, 주문 라우팅을 전략적으로 조절함으로써 판매자들의 재고 보충 인센티브를 형성할 수 있다.

### 핵심 모델
플랫폼은 총수요를 관측하고 시간에 걸쳐 판매자들에게 주문을 배분하며, 판매자는 이 배분 패턴에 반응하여 재고 수준을 조정한다. 이는 전통적인 중앙집중식 재고 관리와 달리, 분산된 의사결정 주체들의 행동을 **간접적 메커니즘**으로 유도하는 접근이다.

### 기존 Wiki와의 연결
- **[[mechanism-design]]**: 판매자의 자발적 재고 결정을 유도하는 배분 규칙 설계는 메커니즘 디자인의 핵심 문제와 직결된다.
- **[[multi-objective-optimization]]**: 플랫폼 수익, 재고 가용성, 판매자 공정성 간의 다목적 최적화 문제를 내포한다.
- **[[task-allocation]]**: 주문을 판매자에게 배분하는 문제는 이종 에이전트 간 작업 배분과 구조적으로 유사하다.
- **[[convex-optimization]]**: 동적 트래픽 배분([[dynamic-traffic-assignment]])과 유사한 볼록 최적화 프레임워크를 활용할 가능성이 높다.

### 인사이트
이 연구는 AI/ML 플랫폼 설계에서 **직접 통제 없이 인센티브 구조로 분산 에이전트를 조율하는 패러다임**을 보여주며, 이는 LLM 에이전트 시스템의 간접 조율 메커니즘([[agent-coordination]])이나 선택 아키텍처([[choice-architecture]]) 연구와도 맥을 같이한다.

## 🔗 관련 논문

- Collaborative Task and Path Planning for Heterogeneous Robot
- CAMO: A Conditional Neural Solver for the Multi-objective Mu
- Binary Decisions in DAOs: Accountability and Belief Aggregat
- A Convex Formulation of the Multi-Commodity Dynamic Traffic 

## 📐 개념

- [[concepts/intertemporal-demand-allocation.md|intertemporal-demand-allocation]]
- [[concepts/inventory-control.md|inventory-control]]
- [[concepts/platform-mediated-market.md|platform-mediated-market]]

---
_LLM 분석으로 재생성됨_
