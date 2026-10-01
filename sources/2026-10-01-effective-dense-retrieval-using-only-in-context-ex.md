# Effective Dense Retrieval using Only In-Context Examples

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-01
**링크**: http://arxiv.org/abs/2609.38099v1

## 💡 핵심 인사이트

검색기 표현 품질은 훈련된 파라미터의 전유물이 아니라 동결 모델에서 인컨텍스트 예시로 유도 가능한 속성이며, 이로써 '능력=훈련' 귀속이 '능력=유도'로 재분류된다.

## 📖 분석

RICE는 사전훈련된 LLM에 인컨텍스트 예시 몇 개를 조건으로 걸어 고품질 밀집 검색 표현을 추출하는 training-free 방법론으로, '검색기 능력 = 검색기 훈련'이라는 귀속을 해체한다. 표현 품질이 미세조정 파라미터의 전유물이 아니라 동결 모델에서 예시 조건화로 유도 가능한 속성임을 실증하여([[partial-reclassification]]), 훈련-유도 경계가 검색 도메인으로 확장된다. 이는 Router Within([[router-within]])의 스킬 라우팅 유도, BSD([[belief-self-distillation]])의 사용자 신념 자기 추출과 함께 '동결 모델 능력 유도' 패턴 패밀리를 형성하며, 동결 모델에서 유도 가능한 능력의 스펙트럼이 행동 선택과 신념 추출에서 표현 생산까지 확장됨을 보여준다. 인컨텍스트 예시는 학습 신호가 아니라 표현 공간을 조건화하는 설계 아티팩트이며([[elicitation-as-harness-artifact]]), 예시 선택이 훈련 데이터 큐레이션을 대체하는 핵심 설계 변수가 된다. ICL([[in-context-learning]])의 효과 지점도 출력 생성에서 표현 기하로 확장되는 사례다.

## 🔗 관련 논문

- Late Attention Layers Alone Can Copy Entity Tokens, but Not Without At
- The Router Within: Eliciting Native Skill Routing from a Fro
- User Model Extraction via Belief Self-Distillation

## 🏷️ 엔티티

- [[entities/in-context-learning.md|in-context-learning]]
- [[entities/elicitation-as-harness-artifact.md|elicitation-as-harness-artifact]]
- [[entities/partial-reclassification.md|partial-reclassification]]
- [[entities/router-within.md|router-within]]
- [[entities/belief-self-distillation.md|belief-self-distillation]]
- [[entities/text-embedding.md|text-embedding]]
- [[entities/knowledge-distillation.md|knowledge-distillation]]

## 📐 개념

- [[concepts/in-context-learning.md|in-context-learning]]
- [[concepts/elicitation-as-harness-artifact.md|elicitation-as-harness-artifact]]
- [[concepts/partial-reclassification.md|partial-reclassification]]
- [[concepts/router-within.md|router-within]]
- [[concepts/belief-self-distillation.md|belief-self-distillation]]
- [[concepts/text-embedding.md|text-embedding]]
- [[concepts/knowledge-distillation.md|knowledge-distillation]]

---
_LLM 분석으로 생성됨_
