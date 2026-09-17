# EarStreAM: A Closed-Loop Earable System for Personalized Stress-Adaptive Meditation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-18
**링크**: http://arxiv.org/abs/2609.19127v1

## 💡 핵심 인사이트

사용자의 생리학적 상태를 LLM 생성 조건 변수로 삼아 비텍스트 피드백 신호의 센서 매개 전환 경로를 구체화하며, 폐루프가 언어가 아닌 인간의 몸을 통해 닫힐 수 있음을 보여준다.

## 📖 분석

이 논문은 OpenEarable 2.0의 귀 내부 멀티모달 센싱과 LLM 기반 개인화 개입을 하나의 폐루프로 결합한 EarStreAM을 제시한다. 심박수와 HRV를 지속 측정해 스트레스 상승을 탐지하고, 탐지 시 LLM이 사용자의 스트레스 상태에 맞춰 실시간으로 개인화된 명상 스크립트를 생성·적응시킨다.

Wiki 관점에서 이 논문의 구조적 기여는 셋이다. **첫째**, 적응 트리거 택소노미에 '사용자 생체 상태'를 추가한다. Wiki의 적응 신호 진화(외부 환경 → 내부 시스템 상태 → 자기 발화)에 네 번째 트리거가 등장하여, 적응 신호의 원천이 모델 경계를 넘어 사용자의 몸으로 확장됨을 보여준다. 이는 undetectable-feedback-signal 문제의 해법 사례다 — 생체 신호는 텍스트에서 판독 불가능하므로 센서 매개를 통해서만 LLM의 조건 변수가 되며, physiological-state-conditioned-generation이라는 경로를 연다. **둘째**, 폐루프의 운영 축을 구분한다. closed-loop-training이 훈련 환경의 폐루프였다면 EarStreAM은 배포 시점(감지-해석-생성-개입)에 형성되는 루프로, closed-loop-intervention 개념을 신설할 근거가 된다. **셋째**, 치료 행위를 LLM 생성 텍스트로 실현하는 intervention-as-generation 패러다임을 제시한다. 개입의 대상이 외부 환경이 아니라 사용자 내부 상태이며, 개입 효과가 생체 신호로 회귀하여 루프가 인간의 몸을 통해 닫힌다는 점이 환경-폐루프 논의와 구별되는 지점이다.

wearable-ai와 연결해 센서 트리거 LLM 대화가 지속 모니터링+실시간 개입의 완결 시스템으로 체계화되는 사례를 제공하며, mental-health-ai 측면에서 개입 자체가 생성되는 스트레스 관리의 새 응용형을 제안한다. internal-state-feedback-extraction과는 추출 대상을 모델이 아닌 사용자의 내부 상태로 반전시키는 대칭 사례가 된다.

## 🔗 관련 논문

- Exploring Expert Perspectives on Wearable-Triggered LLM Conversations

## 🏷️ 엔티티

- [[entities/wearable-ai.md|wearable-ai]]
- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/undetectable-feedback-signal.md|undetectable-feedback-signal]]
- [[entities/closed-loop-training.md|closed-loop-training]]
- [[entities/internal-state-feedback-extraction.md|internal-state-feedback-extraction]]
- [[entities/mental-health-ai.md|mental-health-ai]]
- [[entities/personal-ai-agent.md|personal-ai-agent]]

## 📐 개념

- [[concepts/physiological-state-conditioned-generation.md|physiological-state-conditioned-generation]]
- [[concepts/closed-loop-intervention.md|closed-loop-intervention]]

---
_LLM 분석으로 생성됨_
