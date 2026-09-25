# Where Should I Join? Robot Group Joining via Language-Guided Goal Prediction

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-25
**링크**: http://arxiv.org/abs/2609.28467v1

## 💡 핵심 인사이트

사회적 항법에서 목표는 주어지는 것이 아니라 집단의 실시간 행동으로부터 예측되어야 하며, 언어는 목표가 아니라 목표의 선택 기준만을 제공한다 — 목표 추종이 아니라 목표 예측이 핵심 능력이 된다.

## 📖 분석

이 논문은 사회적 항법(social navigation)의 기본 전제를 역전시킨다. 기존 패러다임은 목표가 주어지고 사회적 관습을 지키며 도달하는 것이었다면, 본 논문은 '어디에 합류할 것인가'라는 목표 자체를 집단의 실시간 활동과 형성(formation) 관찰로부터 예측해야 하는 문제로 정식화한다. 자연어 묘사가 '어느 집단인가'를 특정하면, 합류 지점은 집단의 진행 중 행동에서 유도된다. Wiki 관점에서 세 축으로 연결된다. 첫째, [[goal-operationalization]]의 사회-체화 확장 — 목표가 사용자 제공이 아니라 타 에이전트 집단의 행동 관찰에서 조작화되며, 언어는 목표가 아닌 목표 선택 기준(어느 집단)만 제공한다. 둘째, [[theory-of-mind]]의 물리 공간 최소 실현 — 합류 지점 예측은 집단이 무엇을 하고 있는가에 대한 모델링을 전제한다. 셋째, [[representation-action-gap]]의 다단계 번역 체인: 언어 묘사 → 시각적 집단 식별 → 합류 지점 예측 → 항행 행동. [[agentic-vlm]]과 [[embodied-ai]]에는 '집단 행동 판독'이라는 새 능력 축을 추가한다. [[three-step-nav]] 계열 항법 연구가 정적 목적지를 다뤘다면 본 논문의 목표는 계속 이동하며 사회적으로 구성되는 동적 표적이다. [[spatial-coreference-resolution]]은 언어 묘사와 공간적 집단 인스턴스의 해소 문제로 직결되며, [[planning-without-physical-constraint-encoding]]의 진단(계획이 사회적 관습을 인코딩하지 못함)이 합류 맥락에서 그대로 적용되어 사회적 제약이 물리적 장애물과 별개의 제약 클래스임을 강화한다. 새 개념 behavior-defined-goal을 제안한다: 목표 상태가 고정 위치가 아닌 타 에이전트들의 진행 중 행동으로 정의되는 표적 유형으로, [[latent-objective-emergence]]의 체화 도메인 대응물이다.

## 🔗 관련 논문

- Three-Step Nav: A Hierarchical Global-Local Planner for Zero-Shot Vision-Language Navigation

## 🏷️ 엔티티

- [[entities/behavior-defined-goal.md|behavior-defined-goal]]
- [[entities/agentic-vlm.md|agentic-vlm]]
- [[entities/embodied-ai.md|embodied-ai]]

## 📐 개념

- [[concepts/goal-operationalization.md|goal-operationalization]]
- [[concepts/theory-of-mind.md|theory-of-mind]]
- [[concepts/latent-objective-emergence.md|latent-objective-emergence]]
- [[concepts/spatial-coreference-resolution.md|spatial-coreference-resolution]]
- [[concepts/representation-action-gap.md|representation-action-gap]]
- [[concepts/planning-without-physical-constraint-encoding.md|planning-without-physical-constraint-encoding]]

---
_LLM 분석으로 생성됨_
