# Benchmarking World Models for Continual Learning on Compositional Tasks

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-22
**링크**: http://arxiv.org/abs/2609.22055v1

## 💡 핵심 인사이트

세계 모델의 '적응' 측정이 가소성(새 동역학 학습)과 안정성(기존 동역학 보존)을 혼재시키는 한 지속학습 평가가 불가능하며, 구성적 태스크를 통한 분리 측정이 세계 모델 평가의 새로운 기준이 된다.

## 📖 분석

## 세계 모델 지속학습 벤치마크: 적응과 보존의 분리 측정

본 논문은 세계 모델의 지속학습 능력을 평가하는 벤치마크를 제시한다. 물리 세계의 동역학은 재현되는 메커니즘으로 기술되므로, 선행 경험의 지식 보존·재사용이 새로운 환경 적응의 효율성을 결정한다는 문제의식에 기반한다.

핵심 진단은 **적응 측정의 혼재(entanglement)**다. 기존 평가는 새 태스크를 배우는 능력(가소성)과 이전 지식을 유지하는 능력(안정성)을 단일 적응 지표로 합쳐 측정하므로, 두 능력이 반대 방향으로 움직이는 지속학습 딜레마를 세계 모델 도메인에서 판별할 수 없었다. 본 벤치마크는 구성적(compositional) 태스크를 통해 두 능력을 분리 측정한다.

### Wiki 연결점

- [[world-model-in-pieces]]가 규정한 '보편적 세계 모델 불가능성'에 대한 평가론적 대응 — 조각별 특수화가 불가피하다면 측정 대상은 범용성이 아니라 조각(메커니즘) 간 전이·보존 능력이다.
- [[continual-compoundability]]의 '이득 복리성' 평가 철학을 세계 모델로 확장한다. 선행 메커니즘 재사용이 신규 적응 비용을 절감해 복리 효과를 내는지 측정 가능하게 한다.
- [[cross-episode-reuse-failure]]가 진단한 재사용 불능 문제에 벤치마크 차원의 측정 도구를 부여한다.
- [[learning-forgetting-tradeoff]]와 [[adaptive-forgetting]]의 안정성-가소성 구조를 세계 모델 층위로 격상한다.
- [[model-based-rl]]의 세계 모델 컴포넌트에 수명주기 관리라는 새 요구를 부과한다.
- [[persistent-world-model]]의 영속성을 설계 목표가 아닌 측정 가능한 능력으로 전환한다.

## 🔗 관련 논문

- Remember to be Curious: Episodic Context and Persistent Worl
- Model-Based Reinforcement Learning for Control under Time-Va
- Learning Agent-based Model Predictive Control for Holistic V

## 🏷️ 엔티티

- [[entities/world-model.md|world-model]]
- [[entities/continual-learning.md|continual-learning]]
- [[entities/learning-forgetting-tradeoff.md|learning-forgetting-tradeoff]]
- [[entities/adaptive-forgetting.md|adaptive-forgetting]]
- [[entities/world-model-in-pieces.md|world-model-in-pieces]]
- [[entities/continual-compoundability.md|continual-compoundability]]
- [[entities/cross-episode-reuse-failure.md|cross-episode-reuse-failure]]
- [[entities/model-based-rl.md|model-based-rl]]
- [[entities/environment-capability-co-evolution.md|environment-capability-co-evolution]]
- [[entities/persistent-world-model.md|persistent-world-model]]

## 📐 개념

- [[concepts/adaptation-retention-entanglement.md|adaptation-retention-entanglement]]
- [[concepts/recurring-mechanism-reuse.md|recurring-mechanism-reuse]]
- [[concepts/compositional-continual-evaluation.md|compositional-continual-evaluation]]

---
_LLM 분석으로 생성됨_
