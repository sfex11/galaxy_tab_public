# VLMs May Not Globally Enhance Human Alignment over LLMs During Natural Reading

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-29
**링크**: http://arxiv.org/abs/2605.28818v1

## 💡 핵심 인사이트

VLM은 시각 정보를 통해 텍스트를 더 인간에게 만드는 능력을 가질 수 있으나, 이 능력은 자연스러운 읽기에서 VLM의 시각 정보가 텍스트 이해에 기여하지 않아 오�려려진 텍스트를 생성한다는 반대 결과를 얻습니다. '자연스러운 읽기에서 인간 친화의 증�명'을 VLM이 '시각-텍스트 불일치'라는 부정 확증으로 반박합니다.

## 📖 분석

# reading-visual-alignment-gap


**카테고리**: 미분류
**생성일**: 2026-05-29

## 정의
VLM이 자연스러운 읽기 과정에서 시각 정보를 활용해 텍스트 표현의 인간 친화(human-likeness)을 증진시키고, LLM은 그렇지 않다는 연구 결과입니다. 자연스러운 읽기(문학 텍스트) 특유의 태스크에서, VLM의 멀티모달 학습이 시각 정보를 텍스트 이해에 기여하지 않아 오히려진 텍스트를 생성하여 인간과의 독서를 감소시키는 반대 결과를 제시합니다.


## 관련 논문
- sources/2605.28818v1

## 관련 엔티티
- [[concepts/agentic-vlm.md|agentic vlm]]

## 관련 개념
- reading-visual-alignment-gap

## 관련 소스
- sources/2026-05-27-visual-redundancy-controlled-parallel-decoding-for-diffusion

## 핵심 인사이트 1 (새로운 개념)
이 논문은 VLM과 LLM을 엄격로 비교하는 것이 아니라, 엄격로 비교 불가능한 조건(text-only setting)에서 VLM이 시각 정보를 활용해 텍스트 표현의 인간 친화를 어떻게 변화시키는지를 검증합니다. 핵심: VLM은 시각 정보를 통해 텍스트를 더 인간에게 만드는 능력을 가질 수 있으나, 이 능력은 자연스러운 읽기의 인간 친화를 향상시키지 못해 오히려진 텍스트를 생성한다는 반대 결과를 얻습니다.

## 핵심 인사이트 2 (기존 엔티티 보완)
[[concepts/agentic-vlm.md|agentic vlm]]에 기존하는 '단계별 판단별 문제 vs 다단계 경로 기효 간극'의 인사이트를 보완합니다. 기존 설명은 VLM의 시각 능력이 '단계별 판단별'에서만 발현되고 '다단계 경로 기효'에서는 실패한다는 것이었는데, 이 논문은 그 반대를 발견합니다: text-only setting에서는 양 모두 비슷하지만, VLM은 시각 정보로 인간 친화를 회복하는 데 도움이 된다는 것입니다. 이는 [[entities/inattentional-blindness.md|inattentional blindness]](시각 정보 없이 추론이 단순해짐는 현상)의 natural reading 특화 사례로 기록됩니다.

## 🏷️ 엔티티

- [[entities/reading-visual-alignment-gap.md|reading-visual-alignment-gap]]

## 📐 개념

- [[concepts/reading-visual-alignment-gap.md|reading-visual-alignment-gap]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-05-29-personal-visual-memory-from-explicit-and-implicit-]]: 시각 정보가 텍스트와 결합될 때의 실제 효과를 비판적으로 분석하여, 전자는 VLM이 자연스러운 읽기에서 시각 정보로 오히려 정렬을 저해할 수 있음을 보이고, 후자는 텍스트 기반 접근이 이미지 내 개인 정보를 포착하지 못하는 한계를 지적합니다.
