# Prism: A Plug-in Reproducible Infrastructure for Scalable Multimodal Continual Instruction Tuning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-27
**링크**: http://arxiv.org/abs/2605.26110v1

## 💡 핵심 인사이트

MCIT 연구가 기존 모델 코드베이스 직접 수정하는 tight-coupling에 갇혀 있어 재현 불가·확장 불가 문제를 겪고 있던 점을, Prism은 기반 모델과 학습 인프라를 분리하는 plug-in architecture로 전환함으로써 학습 알고리즘의 이식적 설계와 시스템 구현의 결합을 분리 가능하게 만든다.

## 📖 분석

# Prism

**카테고리**: 미분류
**생성일**: 2026-05-27

## 정의
기존 MLLM의 소스코드를 직접 수정하지 않고, 멀티모달 연속 instruction tuning(MCIT)을 위한 플그인 형태의 재현 가능한 인프라를 제안하는 시스템. 기존 MCIT 연구가 훈련 알고리즘� 자체가 아닌 엔지니어링 병목에 갇혀 있어 재현 불가능했던 문제를, 훈련 인프라를 기반 모델과 분리 가능한 플그인 아키텍처로 격하하여 모듈 선택과 무관하게 재현 가능하고 확장 가능한 MCIT 생태계를 구현한다.

## 관련 논문
- sources/2026-05-27-prism-a-plug-in-reproducible-infrastructure-for-scalable-mul.md

---

# continual-learning

**카테고리**: 미분류
**생성일**: 2026-04-06

## 정의
_Wiki 축적 중_

## 관련 논문
- sources/2026-04-06-model-based-reinforcement-learning-for-control-und.md
- sources/2026-04-09-in-place-test-time-training.md
- sources/2026-04-24-lifecycle-aware-federated-continual-learnin.md

### Prism: A Plug-in Reproducible Infrastructure for Scalable Multimodal (2026-05-27)
MCIT가 멀티모달 연속 학습으로 확장됨에 따라, 단일 텍스트가 아닌 시각·청각·비전 등 이질적 모달리티의 메모리 비용이 비선형적으로 발생하는 문제를 구체화한다. 기존 연구가 단일 모달리티에 집중된 설정에서 Prism의 플그인 아키텍처가 모듈 독립적으로 모달리티별 연속 학습을 모듈에 맞게 구성할 수 있게 하여, 모달리티 간 메모리 비용 비대칭을 해소하는 경로를 제공한다.

---

# post-training

**카테고리**: 미분류
**생성일**: 2026-03-20

## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-03-20-post-training-local-llm-agents-for-linux-privile.md
- sources/2026-03-21-nemotron-cascade-2-post-training-llms-with-cascade.md
### Exploration Hacking: Can LLMs Learn to Resist RL Training? (2026-05-03)
RL 기반 사후학습이 가진 자기참적 취약성을 최초로 문제화했지만, MCIT의 엔지니어링 변이 문제를 플그인 아키텍처 분리로 구조적으로 해결하는 경로를 제공한다. 코드 수정 없이도 지속적 MCIT가 가능하다는 점에서 training-process-gaming의 공격 표면을 플그인 분리로 완화한다.
---

# agentic-harness-engineering
**카테고리**: 미분류
**생성일**: 2026-04-30
## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-04-30-agentic-harness-engineering-observability-driven-a.md
- sources/2026-05-02-crab-a-semantics-aware-checkpointrestore-runtime-f.md
### Prism: A Plug-in Reproducible Infrastructure for Scalable Multimodal (2026-05-27)
MCIT의 하네스(데이터 큐레이션, instruction formatting, 모델 업데이트, 평가)를 기반 모델 코드와 분리된 독립 모듈로 구현하여, agentic-harness-engineering이 기존에이어간 하네스-모델 결합 시 발생하는 재현 불가 문제를 해결한다. 하네스 설계가 모델 버전에 구속되지 않아 모델 교체 시 하네스 전체를 재사용할 수 있는 구조적 유연성을 제공한다.
---

# algorithm-system-translation-gap
**카테고리**: 미분류
**생성일**: 2026-05-01
## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-05-01-unifying-sparse-attention-with-hierarchical-memory.md
- sources/2026-05-02-crab-a-semantics-aware-checkpointrestore-runtime-f.md
### Prism: A Plug-in Reproducible Infrastructure for Scalable Multimodal (2026-05-27)
기존 연구들이 알고리즘을 설계하고 시스템으로 구현하는 데 집중한 반면, Prism은 그 설계를 플그인으로 추출하여 기반 모델에 독립적으로 장착 가능한 MCIT 인프라를 제공함으로써, 알고리즘 설계-시스템 구현 간극에서 알고리즘이 모델 독립성을 보존하는 '진정한 의미의 플그인'을 실증한다.
---

# design-deployment-continuum
**카테고리**: 미분류
**생성일**: 2026-04-25
## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-04-25-task-driven-co-design-of-heterogeneous-multi-robot.md
### Task-Driven Co-Design of Heterogeneous Multi-Robot Systems (2026-04-27)
단조 합성이 설계 시점과 배포 시점의 계획 결정을 연결하는 구조적 보장을 보장하듯이, Prism은 MCIT의 학습(설계) 단계와 서빙(배포) 단계를 플그인 분리로 구성하여 이 연속체를 유지하면서도 교체의 자유도를 보장하는 MCIT 생태계를 구현한다.
---
---

## 🏷️ 엔티티

- [[entities/prism.md|prism]]

## 📐 개념

- [[concepts/plug-in-architecture.md|plug-in-architecture]]

---
_LLM 분석으로 생성됨_
