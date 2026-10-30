# VideoLVR: Latent Visual Reasoning over Grounded Video Evidence

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-30
**링크**: http://arxiv.org/abs/2610.37613v1

## 💡 핵심 인사이트

시각 증거 접지가 반드시 텍스트 번역을 거쳐야 하는 것은 아니며, 잠재 공간에서의 직접 추론이 시각 망각을 구조적으로 제거할 수 있다.

## 📖 분석

VideoLVR은 MLLM의 CoT 추론이 시각 증거 재방문 경로를 제공하지 않아 시각 망각이 발생한다는 문제를 진단하고, 두 기존 접지 방식 — 텍스트 좌표 참조(기호적 위치만 전달)과 프레임 재샘플링(비용이 크고 추론 연속성을 붕괴시킴) — 을 우회하는 잠재 시각 추론(latent visual reasoning)을 제시한다. 시각 증거를 텍스트로 번역하지 않고 잠재 표현을 추론 컨텍스트에 직접 주입하여 번역 없는 접지를 실현한다.

기존 Wiki와의 관계: [[visual-memory-textual-collapse]] 계열(Caption-once·Frames-on-Demand)이 시각 기억의 텍스트 붕괴를 수용·관리 대상으로 삼았다면, 본 논문은 잠재 공간 우회로 붕괴 자체를 제거하여 텍스트 붕괴가 불가피한 전제가 아님을 입증한다. [[cot-as-translated-report]]의 번역 문제가 시각 좌표 참조로도 확장됨을 보여 CoT 신뢰성 논의를 멀티모달로 확장한다. [[on-demand-frame-fetch]]와는 상보적 축을 형성한다 — 픽셀 소급 인출 vs 추론 중 잠재 직접 결합. [[representation-contract]] 관점에서 표현 계약 선택(좌표/재인코딩/잠재 주입)이 접지 품질의 결정 변수임을 확정하며, [[visual-forgetting]]이 저장 문제가 아닌 추론 형식 문제임을 규명한다.

## 🔗 관련 논문

- 2026-10-29-videolvr-latent-visual-reasoning-over-grounded-vid.md
- 2026-09-12-caption-once-frames-on-demand-visual-need-routing-.md

## 🏷️ 엔티티

- [[entities/latent-visual-reasoning.md|latent-visual-reasoning]]
- [[entities/visual-forgetting.md|visual-forgetting]]
- [[entities/textual-coordinate-grounding.md|textual-coordinate-grounding]]
- [[entities/video-understanding.md|video-understanding]]

## 📐 개념

- [[concepts/latent-visual-reasoning.md|latent-visual-reasoning]]
- [[concepts/visual-forgetting.md|visual-forgetting]]
- [[concepts/textual-coordinate-grounding.md|textual-coordinate-grounding]]
- [[concepts/cot-as-translated-report.md|cot-as-translated-report]]
- [[concepts/visual-memory-textual-collapse.md|visual-memory-textual-collapse]]
- [[concepts/representation-contract.md|representation-contract]]
- [[concepts/on-demand-frame-fetch.md|on-demand-frame-fetch]]

---
_LLM 분석으로 생성됨_
