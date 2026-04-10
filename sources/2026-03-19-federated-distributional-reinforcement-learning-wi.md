# Federated Distributional Reinforcement Learning with Distributional Critic Regularization

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-19
**링크**: http://arxiv.org/abs/2603.17820v1

## 💡 핵심 인사이트

연합 학습에서 파라미터 평균 대신 분포적 크리틱을 연합함으로써 안전-critical 환경의 꼬리 리스크 정보를 보존하는 새로운 프레임워크를 제시했다.

## 📖 분석

## Federated Distributional Reinforcement Learning with Distributional Critic Regularization

본 논문은 연합 학습(Federated Learning)과 분포적 강화학습(Distributional RL)을 결합한 **FedDistRL** 프레임워크를 제안한다. 기존 연합 강화학습은 가치 함수나 정책을 파라미터 평균으로 집계하는데, 이 방식은 기대 수익만을 강조하여 안전이 중요한 환경에서 필수적인 통계적 다중모드성(multimodality)과 꼬리 분포(tail behavior) 정보를 소실시킨다.

FedDistRL에서 각 클라이언트는 분위수 가치 함수(quantile value function) 크리틱을 파라미터화하고, 크리틱 네트워크만을 연합한다. 나아가 **TR-FedDistRL**을 제안하여, 클라이언트별로 리스크 인식 Wasserstein 중심(barycenter)을 구축함으로써 분포적 정보를 보존하면서도 연합 학습의 프라이버시 이점을 유지한다.

이 연구는 강화학습의 **안전성(safety)** 문제와 **연합 학습의 프라이버시** 문제를 동시에 다룬다는 점에서 의의가 크다. 분포적 RL은 단순 기대값이 아닌 수익의 전체 분포를 학습하므로, 위험 회피(risk-averse) 정책 수립이 가능하다. 특히 의료, 자율주행, 금융 등 안전이 중요한 분산 환경에서 각 클라이언트가 로컬 데이터를 공유하지 않으면서도 리스크를 고려한 협력 학습이 가능해진다.

기존 Wiki의 강화학습(reinforcement-learning) 개념과 직접 연결되며, AI 안전(ai-safety) 관점에서도 분포적 접근이 꼬리 리스크를 명시적으로 다룬다는 점에서 관련성이 높다.

## 🔗 관련 논문

- 2026 04 10 robust quadruped locomotion via evolutionary reinf
- 2026 04 10 android coach improve online agentic training effi

## 📐 개념

- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/ai-safety.md|ai-safety]]

---
_LLM 분석으로 재생성됨_
