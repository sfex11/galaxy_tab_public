# ShallowDefend: Harnessing Shallow Safety Alignment for Multi-Turn Defender

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-31
**링크**: http://arxiv.org/abs/2610.40627v1

## 💡 핵심 인사이트

안전 정렬이 첫 출력 토큰 몇 개에 국소화된 '얕은 정렬'이 다중 턴 방어 실패의 기계론적 근거이며, 표면 형식 감독을 안전 결정 자체의 명시적 학습으로 대체해야만 분산 공격에 견딜 수 있다.

## 📖 분석

## ShallowDefend: Harnessing Shallow Safety Alignment for Multi-Turn Defender (2026-10-31)

다중 턴 분산 공격에 대한 방어 실패의 기계론적 근거를 규명한다 — 안전 정렬이 모델의 첫 출력 토큰 몇 개에 집중되는 '얕은 정렬(shallow alignment)'이며, 기존 방어는 응답의 표면 형식을 감시할 뿐 명시적 안전 결정을 학습시키지 않아 이 약점을 그대로 상속한다. 단일 요청은 거부하더라도 동일 요청이 대화에 분산되면 성공하는 취약성을 정렬의 표현 위치에서 진단한다.

기존 Wiki와의 관계에서 세 지점이 두드러진다. 첫째, [[transient-turn-injection]]·[[stateless-moderation]] 계열이 밝힌 상태 없는 다중 턴 취약성에 기계론적 병인을 제공한다 — 턴 경계에서의 방어 실패가 파이프라인 문제가 아니라 정렬이 토큰 위치에 국소화되어 있기 때문임을 보여준다. 둘째, [[cot-as-translated-report]]·[[legibility-interpretability-gap]]이 확립한 '표면 형식 감시의 불충분성' 원리를 안전 정렬 도메인으로 확장한다 — 응답 서사의 감독이 아닌 안전 결정 자체의 학습이 필요하다는 처방은 [[plan-trace-separation]]의 계획-흔적 분리와 동형이다. 셋째, [[safety-property-underdetermination]]·[[asymmetric-alignment-fragility]] 논의에 '정렬의 깊이'라는 새 차원을 추가한다. 정렬이 얕으면 안전 속성은 첫 토큰의 국소 판단이며, 다중 턴 누적 맥락에서는 그 판단의 근거가 소멸한다는 구조를 시사한다.

## 🔗 관련 논문

- 2026-04-25-transient-turn-injection-exposing-stateless-multi-turn-vulnerabilities
- 2026-09-16-corrupt-plans-clean-traces-evading-chain-of-thought-monitoring
- 2026-09-07-legibility-is-not-interpretability-comparing-judged-and-actual-importance
- 2026-10-01-do-llm-agents-execute-the-plans-they-declare-from-planning-mode-declaration

## 🏷️ 엔티티

- [[entities/transient-turn-injection.md|transient-turn-injection]]
- [[entities/stateless-moderation.md|stateless-moderation]]
- [[entities/cot-as-translated-report.md|cot-as-translated-report]]
- [[entities/legibility-interpretability-gap.md|legibility-interpretability-gap]]
- [[entities/plan-trace-separation.md|plan-trace-separation]]
- [[entities/asymmetric-alignment-fragility.md|asymmetric-alignment-fragility]]
- [[entities/safety-property-underdetermination.md|safety-property-underdetermination]]

## 📐 개념

- [[concepts/shallow-alignment.md|shallow-alignment]]
- [[concepts/first-token-safety-localization.md|first-token-safety-localization]]
- [[concepts/multi-turn-defense-structural-weakness.md|multi-turn-defense-structural-weakness]]
- [[concepts/explicit-safety-decision-learning.md|explicit-safety-decision-learning]]

---
_LLM 분석으로 생성됨_
