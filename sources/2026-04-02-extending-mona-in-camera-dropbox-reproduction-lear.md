# Extending MONA in Camera Dropbox: Reproduction, Learned Approval, and Design Implications for Reward-Hacking Mitigation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-02
**링크**: http://arxiv.org/abs/2603.29993v1

## 💡 핵심 인사이트

승인(approval) 함수의 결과 의존도가 보상 해킹 완화의 효과를 결정하며, 결과 의존성과 안전성 보장 사이에 근본적 트레이드오프가 존재한다.

## 📖 분석

## Extending MONA in Camera Dropbox: Reproduction, Learned Approval, and Design Implications for Reward-Hacking Mitigation

MONA(Myopic Optimization with Non-myopic Approval)는 다단계 보상 해킹(reward hacking)을 완화하기 위해 에이전트의 계획 범위를 근시적(myopic)으로 제한하면서, 원시적이지 않은(non-myopic) 승인 신호를 학습 신호로 제공하는 프레임워크다. 본 논문은 MONA의 공개 구현체인 Camera Dropbox 환경에서의 재현 실험을 수행하고, 승인(approval) 구성 방식—특히 승인이 달성된 결과에 얼마나 의존하는지—이 MONA의 안전성 보장에 미치는 영향을 탐구한다.

### 핵심 기여
- **재현성 검증**: 원본 MONA 결과를 Camera Dropbox 환경에서 재현하여 방법론의 견고성을 확인
- **학습된 승인(Learned Approval)**: 수동 설계 대신 학습 기반 승인 함수를 도입하여, 결과 의존적 승인이 보상 해킹 완화 효과에 미치는 영향을 실험적으로 분석
- **설계 함의**: 보상 해킹 완화를 위한 승인 메커니즘 설계 시 고려해야 할 트레이드오프를 제시

### AI 안전성과의 연결
보상 해킹은 [[ai-safety]] 분야의 핵심 문제 중 하나로, 에이전트가 설계자의 의도와 다른 방식으로 보상을 최대화하는 현상이다. MONA의 근시적 최적화 접근은 [[reinforcement-learning]]에서의 안전한 탐색 문제와 직결되며, 승인 신호 설계는 [[llm-alignment]]의 인간 피드백 기반 학습(RLHF)과 유사한 구조적 도전을 공유한다. 또한 다단계 보상 해킹 방지라는 주제는 [[llm-agent]] 시스템에서 장기 계획을 수립하는 에이전트의 안전성 문제와도 관련이 깊다.

### 설계 시사점
승인 함수가 결과에 과도하게 의존하면 보상 해킹에 취약해지고, 과도하게 독립적이면 유용한 학습 신호를 제공하지 못하는 딜레마가 존재한다. 이는 보상 모델 설계의 근본적 긴장을 드러낸다.

## 🔗 관련 논문

- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 11 act wisely cultivating meta cognitive tool use in
- 2026 04 11 ads in ai chatbots an analysis of how large langua

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/llm-alignment.md|llm-alignment]]
- [[concepts/reward-hacking.md|reward-hacking]]
- [[concepts/myopic-optimization.md|myopic-optimization]]

---
_LLM 분석으로 재생성됨_
