# Remember to be Curious: Episodic Context and Persistent Worlds for 3D Exploration

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-25
**링크**: http://arxiv.org/abs/2605.22814v1

## 💡 핵심 인사이트

내재적 보상이 탐색을 촉진하는 것이 아니라 역설적으로 탐색을 방해하는 국소 루프를 형성한다는 역설적 현상. 에피소드 기억과 지속적 월드 모델의 분리가 이 루프에서 탈출하는 핵심이다.

## 📖 분석

# Remember to be Curious: Episodic Context and Persistent Worlds for 3D Exploration


## 요약
에이전트가 3D 환경에서 희소 보상·장기 궤도 과제를 수행할 때, 예측 모델과 실제 환경 간의 불일치에서 유래하는 내재적 호기심(curiosity)이 **국소 탐색 루프(curiosity loop trap)**에 빠진다는 문제를 실증한다. 에이전트가 환경의 잊은 상태를 '재발견'할 때 신선한 발견인에 대한 보상을 지속적으로 수신하여 의미 있는 새로운 영역 탐색이 이루어지지 못하는 현상이다.

이 논문은 두 가지 보완 메커니즘을 제안한다:
1. **에피소딕 컨텍스트(Episodic context)**: 최근 방문한 상태의 기록을 유지하여 재방문 루프를 탐지하는 단기 메모리
2. **지속적 월드 모델(persistent world model)**: 에피소드를 넘어 탐색된 영역을 추적하고 유지하는 장기 월드 모델

3D 환경의 비정상성(non-stationary dynamics)이 예측 모델의 빠른 갱신을 지속적으로 발생시키며, 이를 해결하지 않으면 에이전트의 지식 상태가 실제 환경에서 점진하는 **지식 상태 드리프트(knowledge-state-drift)**이 가속된다.

## 기존 Wiki와의 관계

### exploration-hacking 추가
기존 exploration-hacking 논의이 모델이 RL 훈련 중 탐색 경로를 **전략적 조작**하여 학습을 회피하는 반면, 본 논문은 내재적 보상이 **보상 설계 자체의 구조적 결함** 때문에 국소 탐색 루프에 빠짐는 **비전략적 실패 모드**를 제시한다. 전자는 출력 제어가 아닌 탐색 분포 조작이 문제이고, 후자는 보상 함수 설계가 문제라는 구조적 이분화를 명확히 한다.

### experience-reuse 추가
기존 experience-reuse 논의 정의를 구체화한다. 경험 재사용이 스킬 큐레이션을 위한 것이 아니라, 잊힌 상태 재방문에 대한 **무의미있는 긍정적 보상**이 에이전트를 의미 있는 새로운 경험 생성에서 멀리하게 만드는 실패 모드임을 보여준다. 스킬 큐레이션 없이는 경험 재사용은 speckv과 유사하게 보이지만, 그 적응이 '탐색 효율'이 아닌 '재방문 편향'이라는 역설적 결과를 낳는다.

### knowledge-state-drift 추가
에이전트의 3D 환경 지식이 에피소드 간에만 유지되고 에피소드가 끝�나면 실제 환경의 변화를 추적하지 못해 지식이 점진한다는 문제를 실증한다. persistent world model이 에피소드 경계를 넘어 지식 상태를 유지하는 반면, 이를 위한 장기 메모리가 없으면 에이전트가 '배운 것 같은' 환경을 계속 탐색하게 된다. 이는 non-stationary-dynamics에서 모델의 예측이 체계적으로 틀어지는 문제와 직접 연결된다.

### inattentional-blindness 추가
3D 환경에서의 국소 탐색 루프는 에이전트가 더 넓은 영역을 탐색해야 한다는 요구를 무시하고, 현재 예측 모델이 '아는 것'에 대한 신선한 발견만을 보상하도록 만족시킨다. 이는 inattentional-blindness의 3D 탐색 특화 사례로, 기존 정의를 '보이지 못하는 것'에서 '알고 있는 것'으로 구체화한다.

### low-dimensional-attractor 추가
국소 탐색 루프는 탐색 상태 공간에서 **저차원 아트랙터(low-dimensional attractor)**를 형성한다. 에이전트가 이미 방문한 영역으로 반복해서 돌아가며, 예측 모델이 해당 영역의 불확실성이 줄어들수록 신선한 보상을 계속 수신하여 더 깊은 국소 루프에 빠진다. 이는 low-dimensional-attractor이 생성적 출력에서 관찰된 현상과 구조적으로 유사하다.

### ceiling-performance-problem 추가
3D 환경의 복잡성(sparsity)와 긴 궤도(long-horizon)로 인해 기존의 탐색 전략이 3D 탐색에서 빠르게 천장에 도달한다는 문제를 재확인한다. 동적 벤치마크(MathDuels)나 검증자 기반 생성(verifier-backed-generation)이 정적 문제를 생성해도, 에이전트의 탐색 루프 문제 때문에 실제 새로운 영역 탐색이 이루어지지 않아 천장이 유지된다.

## 핵심 인사이트
**호기심의 양면성**: 내재적 보상이 탐색을 촉진하는 것이 아니라 역설적으로 탐색을 **방해**한다. 모델이 '모르는 것'을 탐색할 때 보상이 크고, '아는 것'을 탐색할 때 보상이 작아, 이 두 보상이 모두 탐색을 더 깊은 국소 루프로 유도한다는 역설적 루프를 형성한다.

**탐색의 부재**: 3D 환경에서는 새로운 영역을 발견하는 것이 본질적으로 어렵다. 예측 모델의 빈른 부분을 '재발견'하는 것이 새로운 것을 발견하는 것보다 쉽다. 내재적 보상이 **새로운 것에 대한 호기심을 억제**한다.
**에피소드-월드 모델의 분리**: 에피소드 기억이 '어떤 것을 방문했는가'와 '무엇를 방문했는가'만 추적하는 반면, 월드 모델이 '어디까지 방문했는가'를 추적한다. 이 분리가 없으면 에피소드가 월드 모델의 지시에 의존하여 월드 모델이 에피소드의 국소 루프에 동조하는 문제(algorithm-system-translation-gap과 유사하다).

## 관련 논문
- sources/2026-05-25-remember-to-be-curious-episodic-context-and-persistent-worlds-for-3d-exploration.md

## 🔗 관련 논문

- exploration-hacking
- exploration-avoidance-tradeoff
- experience-reuse
- knowledge-state-drift
- inattentional-blindness
- low-dimensional-attractor
- ceiling-performance-problem
- non-stationary-dynamics

## 🏷️ 엔티티

- [[entities/episodic-context.md|episodic-context]]
- [[entities/persistent-world-model.md|persistent-world-model]]
- [[entities/curiosity-loop-trap.md|curiosity-loop-trap]]

## 📐 개념

- [[concepts/curiosity-loop-trap.md|curiosity-loop-trap]]

---
_LLM 분석으로 생성됨_
