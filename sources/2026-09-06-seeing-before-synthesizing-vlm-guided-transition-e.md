# Seeing Before Synthesizing: VLM-Guided Transition Event Discovery for Weakly-Supervised Dense Video Captioning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-06
**링크**: http://arxiv.org/abs/2609.04183v1

## 💡 핵심 인사이트

합성 데이터의 한계는 생성 능력이 아니라 생성 순서의 문제이며, 시각적 관찰을 합성에 선행시키는 것만으로 weakly-supervised 훈련 신호의 근거성이 회복된다.

## 📖 분석

SBS(Seeing Before Synthesizing)는 Weakly-Supervised Dense Video Captioning에서 최근 연구들이 LLM으로 합성한 transition caption을 시각적 근거 없이 고정된 위치·지속시간으로 모든 inter-event gap에 기계적으로 할당하는 관행을 진단한다. 이는 [[blind-tool-invocation]]의 데이터 생성 버전이다: 합성 아티팩트가 실제 시각 상태와의 대조 없이 훈련 신호로 소비되는 지름길 구조. 논문의 해법은 VLM이 비디오를 먼저 '보고' transition event를 적응적으로 발견하게 하는 것으로, [[agentic-vlm]]을 단순 지각기가 아닌 감독 신호의 능동적 생성자로 격상시킨다. 핵심은 순서의 전환이다 — '합성 후 정렬'이 아닌 '관찰 후 합성'으로, 시각적 증거가 합성물의 존재 여부·위치·지속시간을 결정하게 만든다. 이는 [[shortcut-learning]] 관점에서 합성 데이터의 품질 상한이 시각적 grounding 정확도에 의해 결정됨을, [[circular-validity-problem]] 관점에서는 검증 없는 합성이 자기 강화적 훈련 루프를 형성함을 시사한다. [[video-understanding]]의 스트리밍 컨텍스트 관리(ShallowStream)와 함께, 비디오 이해의 병목이 모델 용량이 아닌 훈련 신호의 근거성에 있음을 보여준다. 'Cited but Not Verified'가 인용의 존재와 의미론적 지지를 분리했다면, SBS는 합성 caption의 존재와 시각적 grounding을 분리하는 동형 구조다.

## 🔗 관련 논문

- ShallowStream: Index Shallow then Answer Deep for Streaming Video Understanding
- Cited but Not Verified: Parsing and Evaluating Source Attribution in LLM Research Reports

## 🏷️ 엔티티

- [[entities/agentic-vlm.md|agentic-vlm]]
- [[entities/blind-tool-invocation.md|blind-tool-invocation]]
- [[entities/video-understanding.md|video-understanding]]
- [[entities/shortcut-learning.md|shortcut-learning]]
- [[entities/circular-validity-problem.md|circular-validity-problem]]
- [[entities/vision-grounded-synthesis.md|vision-grounded-synthesis]]
- [[entities/adaptive-transition-discovery.md|adaptive-transition-discovery]]

## 📐 개념

- [[concepts/vision-grounded-synthesis.md|vision-grounded-synthesis]]
- [[concepts/adaptive-transition-discovery.md|adaptive-transition-discovery]]
- [[concepts/fixed-assignment-fragility.md|fixed-assignment-fragility]]
- [[concepts/synthetic-grounding-gap.md|synthetic-grounding-gap]]

---
_LLM 분석으로 생성됨_
