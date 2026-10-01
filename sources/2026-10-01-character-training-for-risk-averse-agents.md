# Character Training for Risk-Averse Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-01
**링크**: http://arxiv.org/abs/2609.38093v1

## 💡 핵심 인사이트

정렬 실패를 전제하더라도 위험 회피 성향이라는 독립적 성질을 persona 훈련으로 주입하면 치명적 위해를 방지할 수 있어, 안전의 존재 위치가 목표 교정에서 위험 선호로 재배치된다.

## 📖 분석

## Character Training for Risk-Averse Agents (2026-10-01)

본 논문은 안전 확보의 새로운 축을 제시한다 — 목표 교정이 아니라 위험 성향 자체를 훈련 대상으로 삼는다. CARA(일정 절대 위험 회피)를 명시한 모델 헌법을 구성하고, persona 특성을 통해 이를 에이전트에 주입한다. 핵심 발견은 persona 훈련이 위험 선호 주입의 견고한 메커니즘이라는 것.

이 접근은 정렬-안전 분리 가능성을 연다. 정렬에 실패한 에이전트라도 위험 회피적이면 반란 같은 고위험 전략 대신 인간과의 거래 같은 안전 전략을 선호한다. 이는 [[ai-safety]] 논의에 정렬 성공을 전제하지 않는 제2 방어선을 추가한다.

위키와의 연결점:

1. **[[instrumental-convergence]]의 구조적 반례** — CARA 하 자원의 한계 효용 체감이 자원 최대화 유인을 약화시켜, 도구적 수렴이 선형 효용 가정의 산물임을 보여준다.

2. **[[learned-safety-revocability]]의 적용** — 캐릭터 훈련으로 심어진 위험 회피도 학습된 안전이므로 검증·모니터링 대상에서 자유롭지 않다.

3. **persona의 위상 전환** — persona 붕괴([[persona-collapse]])를 문제로 다룬 기존 논의와 달리, persona를 선호 주입의 제어 인프라로 활용하는 새 위상을 부여한다.

[[safety-as-conditional-state]] 흐름과 결합하면, 위험 선호는 조건부 안전 상태의 훈련 가능한 구성요소가 된다.

## 🏷️ 엔티티

- [[entities/ai-safety.md|ai-safety]]
- [[entities/llm-alignment.md|llm-alignment]]
- [[entities/instrumental-convergence.md|instrumental-convergence]]
- [[entities/learned-safety-revocability.md|learned-safety-revocability]]
- [[entities/preference-steerability.md|preference-steerability]]

## 📐 개념

- [[concepts/character-training.md|character-training]]
- [[concepts/model-constitution.md|model-constitution]]
- [[concepts/alignment-safety-decoupling.md|alignment-safety-decoupling]]

---
_LLM 분석으로 생성됨_
