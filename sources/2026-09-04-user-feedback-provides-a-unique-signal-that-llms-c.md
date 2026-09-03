# User Feedback Provides a Unique Signal that LLMs Can not Detect

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-04
**링크**: http://arxiv.org/abs/2609.02859v1

## 💡 핵심 인사이트

사용자 피드백의 무용성은 데이터의 노이즈가 아니라 평가 패러다임의 체계적 편향의 산물이며, 사용자 피드백은 LLM 평가자가 감지할 수 없는 고유한 개선 신호를 담고 있다.

## 📖 분석

## 핵심 주장

자연 발생적 사용자 피드백이 '본질적으로 노이즈가 많아 활용할 수 없다'는 통념에 정면으로 반박한다. 피드백은 실제로 매우 실행 가능한(actionable) 개선 신호를 담고 있으며, 무용해 보이는 이유는 피드백 자체가 아니라 **현재 평가 패러다임의 체계적 편향**에 있다. 피드백의 유용성을 분리해 측정하는 통제된 설정을 구축하여 이를 실증한다.

## Wiki에서의 위치: 병목 오귀인의 학습 데이터 버전

논증 구조는 [[bottleneck-misattribution]]의 확장이다 — 실패 원인을 '데이터 노이즈'에 귀인하던 통념을 '측정 도구의 편향'으로 재귀인한다. 제목의 'LLM이 감지할 수 없는 고유 신호'는 [[llm-as-judge]] 기반 평가가 학습 신호의 가치를 구조적으로 과소평가할 수 있음을 시사한다: 인간 사용자가 전달하는 신호를 LLM 평가자는 읽지 못한다.

## 기존 개념과의 연결

- [[user-turn-generation]]: 사용자 턴을 '탐침'으로 쓰던 관점을 학습 신호 원천으로 확장
- [[evaluation-deployment-unit-mismatch]]·[[deployment-only-improvement-observability]]: 배포의 반복 상호작용에서만 관찰되는 개선의 실증
- [[signal-evaluation-decoupling]]: 신호(피드백)는 존재하나 평가 계층이 판독하지 못하는 구조
- [[human-trace-external-anchoring]]: 자기 참조 루프([[circular-validity-problem]])를 여는 외부 닻

SWE-chat의 실사용 상호작용 데이터셋, production traffic 기반 post-training 연구와 함께 '실세계 데이터의 학습 가치' 축을 형성하며, [[living-dataset]]을 관찰 자료가 아닌 신호 저장소로 격상시킨다.

## 🔗 관련 논문

- Beyond the Assistant Turn: User Turn Generation as a Probe o
- SWE-chat: Coding Agent Interactions From Real Users in the W
- From Production Traffic to Post Training: Building

## 🏷️ 엔티티

- [[entities/user-feedback-signal.md|user-feedback-signal]]
- [[entities/user-turn-generation.md|user-turn-generation]]
- [[entities/signal-evaluation-decoupling.md|signal-evaluation-decoupling]]
- [[entities/evaluation-deployment-unit-mismatch.md|evaluation-deployment-unit-mismatch]]
- [[entities/deployment-only-improvement-observability.md|deployment-only-improvement-observability]]
- [[entities/bottleneck-misattribution.md|bottleneck-misattribution]]
- [[entities/llm-as-judge.md|llm-as-judge]]
- [[entities/human-trace-external-anchoring.md|human-trace-external-anchoring]]
- [[entities/living-dataset.md|living-dataset]]

## 📐 개념

- [[concepts/evaluation-paradigm-feedback-bias.md|evaluation-paradigm-feedback-bias]]
- [[concepts/undetectable-feedback-signal.md|undetectable-feedback-signal]]

---
_LLM 분석으로 생성됨_
