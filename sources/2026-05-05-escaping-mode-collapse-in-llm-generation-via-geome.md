# Escaping Mode Collapse in LLM Generation via Geometric Regulation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-05
**링크**: http://arxiv.org/abs/2605.00435v1

## 💡 핵심 인사이트

모드 붕괴는 분포의 통계적 문제가 아니라 표현 공간에서 궤적이 저차원 영역으로 구속되는 기하학적 현상이며, 이 동역학적 재해석이 기존의 행동 매니폴드 구속·페르소나 붕괴·공유 실패 부분공간 등 산발적 묘사들을 단일 기하학적 메커니즘으로 통합한다.

## 📖 분석

# Geometric Collapse: 동역학적 관점에서의 모드 붕괴

자기회귀 텍스트 생성에서 모드 붕괴(mode collapse)를 명시적 루핑, 다양성 상실, 조기 궤적 수렴 등의 현상으로 관찰해 왔으나, 본 논문은 이를 동역학 시스템 관점에서 **기하학적 붕괴(geometric collapse)**로 재해석한다. 모델의 내부 궤적이 표현 공간의 저차원 영역으로 구속되는 현상이며, 이는 통계적 분포의 문제가 아니라 표현 공간의 기하학적 접근성(reduced state-space accessibility) 문제임을 보인다.

## 기존 Wiki와의 관계

**behavioral-manifold-confinement**이 '입력 변이에 따른 출력 변이가 극히 제한된 행동 매니폴드 내에 갇혀 있다'는 현상을 기술했다면, 본 논문은 이를 동역학적 메커니즘(궤적의 저차원 구속)으로 정밀화한다. **persona-collapse**가 페르소나 붕괴의 침투적 실패를 묘사했다면, 본 논문은 이를 기하학적 붕괴의 특수 사례로 위치시킨다. **shared-failure-subspace**가 '서로 다른 모델이 동일한 취약 영역을 공유한다'고 했는데, 기하학적 붕괴는 이 공유된 실패 부분공간의 형성 메커니즘을 설명한다.

## 연결점

[[sources/2026-05-05-escaping-mode-collapse-in-llm-generation-via-g.md|본 논문]]의 기하학적 규제(geometric regulation)는 [[entities/reasoning-integrity|reasoning-integrity]]를 표현 공간 수준에서 보장하는 구조적 접근이다. 또한 [[entities/exploration-hacking|exploration-hacking]]이 RL 탐색 분포의 조작 문제를 다루었다면, 기하학적 붕괴는 생성 과정에서의 내적 탐색(표현 공간 탐색)이 저차원으로 수렴하는 현상으로, 동일한 '접근성 축소' 패턴의 생성 시점 인스턴스다.

## 🏷️ 엔티티

- [[entities/geometric-collapse.md|geometric-collapse]]
- [[entities/state-space-accessibility.md|state-space-accessibility]]
- [[entities/geometric-regulation.md|geometric-regulation]]

## 📐 개념

- [[concepts/geometric-collapse.md|geometric-collapse]]
- [[concepts/state-space-accessibility.md|state-space-accessibility]]
- [[concepts/geometric-regulation.md|geometric-regulation]]
- [[concepts/trajectory-confinement.md|trajectory-confinement]]
- [[concepts/low-dimensional-attractor.md|low-dimensional-attractor]]

---
_LLM 분석으로 생성됨_
