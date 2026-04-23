# FL-PBM: Pre-Training Backdoor Mitigation for Federated Learning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-31
**링크**: http://arxiv.org/abs/2603.28673v1

## 💡 핵심 인사이트

연합학습 환경에서 사전학습 단계의 백도어 공격 완화라는 새로운 방어 시점을 제시하며, 기존의 학습 중/후 방어 기법과 상호보완적 보안 계층을 형성한다.

## 📖 분석

## FL-PBM: Pre-Training Backdoor Mitigation for Federated Learning

본 논문은 연합학습(Federated Learning) 환경에서 사전학습 단계의 백도어 공격을 완화하는 방법론인 FL-PBM을 제안한다. 백도어 공격은 학습 데이터에 숨겨진 트리거를 주입하여 모델의 행동을 조작하는 공격으로, 자율주행, 헬스케어, 금융 등 안전이 중요한 응용 분야에서 심각한 위협이 된다.

### 기존 Wiki와의 연결

**연합학습(federated-learning)** 개념과 직접적으로 관련된다. 기존 Wiki에서는 [[concepts/federated-learning.md|federated learning]]이 분산 강화학습 맥락에서 다뤄졌으나(Federated Distributional Reinforcement Learning), 본 논문은 연합학습의 보안 취약점이라는 새로운 관점을 추가한다. 연합학습은 데이터를 중앙에 모으지 않고 분산 학습하므로 각 참여자가 주입하는 데이터를 직접 검증하기 어렵다는 구조적 취약점이 존재하며, 이것이 백도어 공격의 주요 공격면이 된다.

**AI 안전(ai-safety)** 관점에서도 중요한 연결점이 있다. 기존 TraceSafe 논문이 LLM 가드레일의 체계적 평가를 다뤘다면, FL-PBM은 학습 파이프라인 자체의 보안을 다룬다는 점에서 AI 안전의 다른 층위를 보완한다.

**차분 프라이버시(differential-privacy)** 와도 간접적 관련이 있다. 차분 프라이버시가 데이터 프라이버시 보호에 초점을 맞춘다면, 백도어 완화는 모델 무결성 보호에 초점을 맞추며, 두 기법 모두 연합학습 환경의 신뢰성 확보를 위한 상호보완적 방어 메커니즘이다.

### 핵심 기여

사전학습(pre-training) 단계에서의 백도어 완화에 초점을 맞춘다는 점이 독특하다. 대부분의 기존 방어 기법이 학습 중(in-training) 또는 학습 후(post-training) 단계에 집중하는 반면, 사전학습된 모델이 이미 오염되어 있을 수 있다는 현실적 위협 시나리오를 다룬다.

## 🔗 관련 논문

- Federated Distributional Reinforcement Learning with Distrib
- TraceSafe: A Systematic Assessment of LLM Guardrails on Mult
- Differential Privacy in Generative AI Agents: Analysis and O

## 📐 개념

- [[concepts/federated-learning.md|federated-learning]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/differential-privacy.md|differential-privacy]]
- [[concepts/backdoor-attack.md|backdoor-attack]]

---
_LLM 분석으로 재생성됨_
