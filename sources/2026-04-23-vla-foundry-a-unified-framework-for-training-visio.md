# VLA Foundry: A Unified Framework for Training Vision-Language-Action Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-23
**링크**: http://arxiv.org/abs/2604.19728v1

## 💡 핵심 인사이트

VLA 모델의 성능 상한선은 모델 아키텍처가 아닌 사전학습 파이프라인의 호환성에 의해 결정되며, 언어→시각→행동의 전체 훈련 경로를 단일 스택에서 제어해야만 종단 간 일관성을 확보할 수 있다.

## 📖 분석

# VLA Foundry

**카테고리**: AI/ML — 체화된 지능 프레임워크
**생성일**: 2026-04-23

## 정의

VLA Foundry는 언어 사전학습부터 행동 전문가 미세조정(action-expert fine-tuning)까지 LLM, VLM, VLA 훈련을 단일 코드베이스에서 통합하는 오픈소스 프레임워크다.

## 기존 VLA 생태계의 구조적 문제

기존 오픈소스 VLA 연구는 행동 훈련 단계에만 특화되어, 상호 호환되지 않는 사전학습 파이프라인을 조합(stitch)하는 방식에 의존했다. 이는 Wiki에서 이미 식별된 [[concepts/sandbox-liveworld-gap|샌드박스-실세계 격차]]의 훈련 파이프라인 버전이라 할 수 있다 — 각 단계가 독립적으로 최적화되면 전체 파이프라인의 일관성이 보장되지 않는다.

## 핵심 기여

1. **종단 간 제어**: 언어 사전학습 → VLM 정렬 → 행동 전문가 미세조정을 단일 스택에서 관리
2. **유연성**: 백지 상태(from-scratch) 훈련과 Hugging Face 사전학습 백본 모두 지원
3. **[[entities/robotics-foundation-model|로봇tics 파운데이션 모델]]의 실현**: 파이프라인 호환성 문제를 해결하여 [[entities/llm|LLM]]→[[entities/vlm|VLM]]→VLA의 연속적 스케일업 경로를 개척

## Wiki 연결점

- [[entities/llm-agent|LLM 에이전트]] 합성 분석의 '능력 확장' 축에서 VLA를 물리 환경 내비게이션의 기반 인프라로 위치화 가능
- [[concepts/embodied-ai|체화된 AI]] 연구에서 VLM→VLA 파이프라인의 표준화는 [[concepts/transfer-learning|전이 학습]]의 성능 상한선을 높이는 구조적 개선
- [[concepts/hierarchical-representation|계층적 표현]] 관점에서 언어→시각→행동의 계층을 아키텍처 수준에서 일관되게 통합

## 관련 논문

- [[sources/2026-04-23-vla-foundry-a-unified-framework-for-training-v.md|VLA Foundry: A Unified Framework for Training Vision-Language-Action Models]]

## 🔗 관련 논문

- 2026 04 22 using large language models for embodied planning 
- 2026 04 21 semantic area graph reasoning for multi robot lang
- 2026 04 11 visually grounded humanoid agents

## 🏷️ 엔티티

- [[entities/vla-foundry.md|vla-foundry]]
- [[entities/llm.md|llm]]
- [[entities/vlm.md|vlm]]
- [[entities/robotics-foundation-model.md|robotics-foundation-model]]
- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/end-to-end-vla-training.md|end-to-end-vla-training]]
- [[concepts/action-expert-fine-tuning.md|action-expert-fine-tuning]]
- [[concepts/pretraining-pipeline-incompatibility.md|pretraining-pipeline-incompatibility]]
- [[concepts/embodied-ai.md|embodied-ai]]
- [[concepts/transfer-learning.md|transfer-learning]]
- [[concepts/hierarchical-representation.md|hierarchical-representation]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-04-22-onevl-one-step-latent-reasoning-and-planning-with-]]: 둘 다 시각-언어-행동(VLA) 모델을 다루며, 하나는 잠재 추론을 통한 자율주행 지연 문제를, 다른 하나는 언어→시각→행동 전체 훈련 파이프라인의 통합 프레임워크를 제안한다.
