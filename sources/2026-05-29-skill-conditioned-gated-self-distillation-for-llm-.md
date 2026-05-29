# Skill-Conditioned Gated Self-Distillation for LLM Reasoning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-29
**링크**: http://arxiv.org/abs/2605.28791v1

## 💡 핵심 인사이트

이 논문의 가장 중요한 인사이트 1문장: 기존 방식들이 '신뢰 우선'을 ground truth에만 연결한 것은, 학습 가능한 스킬의 활용을 불가능하게 만드는 근본적 한계를 문제 삼고, 이를 검증자 기반 게이팅 함수로 해결하여 탐색-흡수 분리를 비사후 통합하는 구체적 해법을 제시합니다.

## 📖 분석

# skill-conditioned-gating

**카테고리**: 미분류
**생성일**: 2026-05-29

## 정의
On-policy self-distillation (SD)에서 교사자 측에서의 신뢰(privileged information)를 사용하는 대신, 경험 유래에서 추출된 스킬 뱅크를 검증자 결과로 변환하여 온폴리 토큰 수준의 감독을 수행하는 학습 가능한 게이팅 함수를 제안합니다. 기존 방식들이 스킬의 신뢰를 단순히 신뢰한다면, 이 논문은 신뢰의 출처를 '경험에서 유래한 스킬'로 간주어 검증 문제로 재정하여, 스킬 소비의 양성/부정확 문제와 검증자의 신뢰/불신뢰 문제 사이를 해결하는 구체적 메커니즘을 제시합니다.

## 관련 논문
- sources/2605.28791v1

## 🏷️ 엔티티

- [[entities/skill-conditioned-gating.md|skill-conditioned-gating]]

## 📐 개념

- [[concepts/exploration-absorption-decoupling.md|exploration-absorption-decoupling]]

---
_LLM 분석으로 생성됨_
