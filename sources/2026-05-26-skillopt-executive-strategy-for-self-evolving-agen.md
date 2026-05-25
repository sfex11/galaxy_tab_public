# SkillOpt: Executive Strategy for Self-Evolving Agent Skills

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-26
**링크**: http://arxiv.org/abs/2605.23904v1

## 💡 핵심 인사이트

프롬프트 엔지니어링이 가중치 공간의 불투명성 문제라는 인식을, 스킬을 가중치 공간의 파라미터(external state)로 취급하여 학습 가능한 모델의 가중치 공간 최적화와 동일한 수학적 규율을 텍스트 공간에서 재현한다. 이는 프롬프트가 '작성'이 아니라 '훈련'되어야 한다는 패러다임의 근본적 전환을 제시한다.

## 📖 분석

# SkillOpt: Executive Strategy for Self-Evolving Agent Skills


**카테고리**: AI/ML — 에이전트 스킬 학습
**생성일**: 2026-05-26

## 정의
에이전트 스킬이 현재의 방식(수작, 원샷 생성, 느슨하게 통제된 자기 수정)로는 학습되지 않으며, 피드백 하에서도 출발점 이상으로 개선되지 못하는 근본적 한계를 지적한다. SkillOpt는 스킬을 동결된 에이전트의 '외부 상태(external state)'로 취급하여, 가중치 공간 최적화와 동일한 수학적 규율을 텍스트 공간에서 재현한다.

## 공통 주제: 스킬=가중치, 프롬프트=활성성
SkillOS가 스킬을 큐레이션 대상으로 모아지만 학습 가능한 모델이 아닌 단순한 텍스트 조작 문제로 다루었다면, SkillOpt는 스킬 텍스트를 가중치 공간의 파라미터로 취급한다. 이는 프롬프트 엔지니어링이 가중치 공간의 불투명성 문제를 해결하며, 스킬이 '작성'이 아니라 '훈련'되는 패러다임을 제시한다.

### 기존 Wiki와의 관계
- sources/2026-05-10-skillos-learning-skill-curation-for-self-evolving-.md: 스킬 큐레이션이 학습 가능한 모델의 능력 향상이 아니라 수동적 스킬 조작 문제였음
- [[entities/self-improving-agent|self-improving-agent]]: 에이전트 자체가 아니라 스킬(외부 상태)이 개선되는 패러다임으로 재정의
- [[entities/skill-lifecycle-management|skill-lifecycle-management]]: 스킬 수명 주기가 아닌 최적화 루프를 가진 훈련 루프로 구체화
- [[entities/experience-reuse|experience-reuse]]: 경험을 소비가 아닌 훈련 데이터로 변환하는 패러다임으로 재정의

## 관련 논문
- sources/2026-05-26-skillopt-executive-strategy-for-self-evolving-agent-sk.md

## 새로운 엔티티
- entities/skill-as-external-state

## 관련 개념
- concepts/skill-as-external-state

## 🏷️ 엔티티

- [[entities/skill-as-external-state.md|skill-as-external-state]]

---
_LLM 분석으로 생성됨_
