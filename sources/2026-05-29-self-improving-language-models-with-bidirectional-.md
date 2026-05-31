# Self-Improving Language Models with Bidirectional Evolutionary Search

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-29
**링크**: http://arxiv.org/abs/2605.28814v1

## 💡 핵심 인사이트

기존 탐색(best-of-N, tree search)이 '모델이 잘 아는 곳'이라는 확률 분포 경계에 갇힙되어 낮은 확률 영역을 탐색하지 않는 두 번째 근본적 한계를 식별하여, 확률 분포 내에서 검증 가능한 경계를 발견하고 그 경계 밖에서 유의미 있는 새로운 후보를 발견합니다.

## 📖 분석

# bidirectional-evolutionary-search

**카테고리**: 미분류
**생성일**: 2026-05-29

## 정의
자회규적 확장을 통한 탐색 방법(Best-of-N, Tree Search 등)이 두 가지 근본적 한계를 가진다는 문제를 식별하고, 확률 분포 내에서 검증 가능한 경계(provable statement boundary)를 탐색하여 낮은 확률 영역(low probability mass)에서 유의미 있는 새로운 후보를 발견하는 탐색 패러다임.

## 핵심 메커니즘

1. **확률 분포 경계 탐색**: 자회규적 확장이 높은 확률 영역에서만 탐색하여, 모델이 이미 잘 아는 패턴에 갇힙되는 문제(확률 근인)
2. **양방향 검증**: 단순한 패/불 통과 판별이 아니라, 후보가 검증 가능한지(containment)와 불가능한지(failure)를 양방향으로 검증하여, 단순히 재생성이 아닌 본원 패턴을 걸러내는 문제(거절 편향 해소)
3. **거절 샘플링**: 단순히 확률 높은 결과를 선택하는 것이 아니라 검증을 통과한 낮은 확률 결과를 적극적으로 탐색하여, 거절이 아닌 본원을 가장한 것으로 선택하는 문제(거절 편향 해소)

## 관련 논문
- [[entities/bidirectional-competency-asymmetry.md|bidirectional competency asymmetry]]
- sources/2605.28814v1

## 🏷️ 엔티티

- [[entities/bidirectional-evolutionary-search.md|bidirectional-evolutionary-search]]

## 📐 개념

- [[concepts/probability-mass-boundary.md|probability-mass-boundary]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-05-28-sia-self-improving-ai-with-harness-weight-updates]]: 두 논문 모두 AI 시스템의 자가 개선(self-improvement) 문제를 다루지만, 전자는 하네스 재작성과 가중치 업데이트의 통합을, 후자는 양방향 진화 탐색을 통한 확률 분포 경계 확장이라는 상호 보완적인 접근을 제시합니다.
- → [[sources/2026-05-29-agent-explorative-policy-optimization-for-multimod]]: 에이전트의 탐색 한계를 근원적으로 문제 삼으며, 전자는 기존 RL의 탐색-흡수 분리 가정이 에이전트 설정에서 실패함을 보이고, 후자는 기존 탐색 방법이 확률 분포 경계에 갇히는 한계를 지적합니다.
