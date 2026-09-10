# SAEScientist-Bench: Can AI Agents Conduct Autonomous SAE Interpretability Research?

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-10
**링크**: http://arxiv.org/abs/2609.09113v1

## 💡 핵심 인사이트

재귀적 자기 개선의 자동화가 훈련 파이프라인에 머무는 동안, 이 논문은 '모델이 무엇을 학습했는가를 스스로 조사하는 능력'을 에이전트 평가의 새로운 대상으로 격상시켜 RSI의 결여된 사후 감시 기둥을 벤치마크 형식으로 명문화한다.

## 📖 분석

SAEScientist-Bench는 재귀적 자기 개선(RSI) 연구가 훈련 파이프라인 자동화에 집중하는 동안 '모델이 무엇을 학습했는가'를 이해하고 안전한 정렬을 보장하는 사후 감시·감사라는 기둥이 결여되어 있다는 진단에서 출발한다. 희소 오토인코더(SAE)를 해석 가능한 특징 격리의 초석으로 삼아, AI 에이전트가 자율적으로 SAE 해석가능성 연구를 수행할 수 있는가를 평가하는 벤치마크를 도입한다.

기존 Wiki에서 [[sparse-autoencoder]]는 MoRFI를 통해 '정성적 탐색 도구에서 단조성 기반 인과 특징 식별 도구'로 격상된 바 있는데, 본 논문은 한 단계 더 나아가 SAE 연구 자체를 에이전트의 수행 대상으로 격상시킨다. [[steering-read-manipulation-duality]]가 지적한 판독-조작 이중성이 SAE의 검사·조향 이중 용도로 재현되며, 에이전트가 내부 판독 능력을 갖추면 조작 능력도 함께 내재함을 시사한다.

[[auditability-as-scaling-requirement]]의 '감사 가능성이 스케일링 요구사항' 원칙에 해석가능성이라는 구체적 기술 경로를 제공하며, [[certification-monitoring-discontinuity]]의 인증-감시 단절을 메우는 사후 해석적 감시 계층으로 위치한다. [[autoresearch]]와 [[exploratory-research-agent]]가 연구 실행 자동화를 다뤘다면, 본 논문은 연구 대상을 '모델 내부 감사'로 특화하여 자기 개선 루프([[bootstrap-paradox]], [[endogenous-self-evolution]])의 폐쇄성을 감사 가능한 형태로 여는 방향을 제시한다. DiscoverPhysics가 과학적 발견 능력을 평가했다면, 본 논문은 평가 대상을 '연구 수행'에서 '연구 주체로서의 감사 능력'으로 전환시킨다.

## 🔗 관련 논문

- MoRFI: Monotonic Sparse Autoencoder Feature Identification
- From Syntax to Emotion: A Mechanistic Analysis of Emotion Inference in Large Language Models
- Legibility is Not Interpretability: Comparing Judged and Actual Importance
- DiscoverPhysics: Benchmarking LLMs for Out-of-the-Box Scientific Discovery
- From Research Question to Scientific Workflow: Leveraging Agentic AI for Workflow Automation
- Clean Engineering, Unstable Measurement: A Preregistered Reliability Framework

## 🏷️ 엔티티

- [[entities/sparse-autoencoder.md|sparse-autoencoder]]
- [[entities/mechanistic-interpretability.md|mechanistic-interpretability]]
- [[entities/causal-mechanistic-interpretability.md|causal-mechanistic-interpretability]]
- [[entities/autoresearch.md|autoresearch]]
- [[entities/exploratory-research-agent.md|exploratory-research-agent]]
- [[entities/auditability-as-scaling-requirement.md|auditability-as-scaling-requirement]]
- [[entities/autonomous-interpretability-research.md|autonomous-interpretability-research]]

## 📐 개념

- [[concepts/steering-read-manipulation-duality.md|steering-read-manipulation-duality]]
- [[concepts/interpretability-as-audit-layer.md|interpretability-as-audit-layer]]
- [[concepts/research-capability-benchmark.md|research-capability-benchmark]]
- [[concepts/sae-feature-knowledge-conflict.md|sae-feature-knowledge-conflict]]

---
_LLM 분석으로 생성됨_
