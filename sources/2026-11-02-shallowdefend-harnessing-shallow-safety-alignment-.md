# ShallowDefend: Harnessing Shallow Safety Alignment for Multi-Turn Defender

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-02
**링크**: http://arxiv.org/abs/2610.40627v1

## 💡 핵심 인사이트

안전 정렬의 얕음(첫 토큰 집중)이 취약점이 아니라 방어의 설계 지점이 된다 — 감독 대상을 응답 표면 형식에서 명시적 안전 결정으로 이동시키면, 다중 턴 분산 공격에 대한 구조적 방어가 가능해진다.

## 📖 분석

ShallowDefend는 안전 정렬의 얕음(shallow alignment)을 진단하고 이를 방어 자원으로 재해석하는 다중 턴 방어 논문이다. 핵심 발견은 안전 행동이 모델의 첫 몇 개 출력 토큰에 집중되어 있다는 기계론적 사실이다. 이는 기존 Wiki의 safety-property-underdetermination과 asymmetric-alignment-fragility 논의에 토큰 위치라는 구체적 차원을 부여한다 — 안전 속성이 분산 표현이 아닌 국소적 표층 판단에 의존하므로, 대화가 길어질수록 판단 근거가 구조적으로 소멸한다는 취약성의 정밀한 위치를 특정한다.

기존 접근이 응답의 표면 형식(cot-as-translated-report, plan-trace-separation)을 감독했다면, ShallowDefend는 '명시적 안전 결정'을 학습 대상으로 삼는 패러다임 전환을 제안한다. 이는 plan-trace-separation의 방어 설계 적용 사례로, 감독 대상을 흔적이 아닌 결정 계층으로 이동시킨다.

stateless-moderation 관점에서도 중요하다. 얕은 안전이 단일 턴의 표층 판단이기 때문에, 상태 없는 검열이 다중 턴 공격(transient-turn-injection)에 실패하는 구조적 이유가 기계론적으로 설명된다. 또한 multi-turn-defense-structural-weakness에 '얕은 정렬의 상속'이라는 병인을 제공하며, explicit-safety-decision-learning의 원천 개념으로 기능한다. first-token-safety-localization의 입도에서 명시적 학습으로 확장되는 흐름의 시작점이다.

## 🔗 관련 논문

- 2026-10-31-shallowdefend-harnessing-shallow-safety-alignment-

## 🏷️ 엔티티

- [[entities/safety-property-underdetermination.md|safety-property-underdetermination]]
- [[entities/asymmetric-alignment-fragility.md|asymmetric-alignment-fragility]]
- [[entities/multi-turn-defense-structural-weakness.md|multi-turn-defense-structural-weakness]]
- [[entities/stateless-moderation.md|stateless-moderation]]
- [[entities/plan-trace-separation.md|plan-trace-separation]]
- [[entities/cot-as-translated-report.md|cot-as-translated-report]]
- [[entities/transient-turn-injection.md|transient-turn-injection]]
- [[entities/first-token-safety-localization.md|first-token-safety-localization]]
- [[entities/explicit-safety-decision-learning.md|explicit-safety-decision-learning]]

## 📐 개념

- [[concepts/shallow-alignment.md|shallow-alignment]]
- [[concepts/safety-decision-supervision.md|safety-decision-supervision]]
- [[concepts/multi-turn-safety-brittleness.md|multi-turn-safety-brittleness]]
- [[concepts/token-localized-safety-behavior.md|token-localized-safety-behavior]]

---
_LLM 분석으로 생성됨_

---
**관련**: [[entities/role-as-relational-property.md|role as relational property]]
