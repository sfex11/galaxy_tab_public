# VideoLVR: Latent Visual Reasoning over Grounded Video Evidence

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-29
**링크**: http://arxiv.org/abs/2610.37613v1

## 💡 핵심 인사이트

텍스트 매개 추론이 유발하는 시각 소실의 해법은 좌표 참조의 정교화가 아니라 추론 공간 자체의 잠재화이며, 이는 시각 붕괴의 '관리'에서 '회피'로의 패러다임 이동이다.

## 📖 분석

## 진단과 제안

VideoLVR은 MLLM의 텍스트 기반 Chain-of-Thought가 시각 증거의 재방문 메커니즘을 제공하지 못해 visual forgetting을 유발함을 진단하고, 접지된 비디오 증거 위에서 텍스트 매개 없이 추론을 수행하는 Latent Visual Reasoning을 제안한다.

## 기존 논의와의 관계

[[visual-memory-textual-collapse]] 논의에 추론 궤적 차원을 추가한다. 기존에는 시각 정보가 메모리 저장 시점에 텍스트로 붕괴하는 문제로 논의되었으나, 본 논문은 붕괴가 추론 자체의 텍스트 매개에서도 발생함을 보인다. 텍스트 좌표 참조(기호적 위치 지정)라는 기존 완화책은 여전히 재번역 병목을 유지하므로, Caption-once/Frames-on-Demand(sources/2026-09-13-caption-once-frames-on-demand-visual-need-routing-.md)의 '붕괴 수용 + 온디맨드 회복' 전략과 대비되는 '추론 중 붕괴 자체의 회피'라는 제2 경로를 연다.

[[cot-as-translated-report]]의 비디오 도메인 실증이기도 하다. 자연어 CoT가 내부 계산의 번역된 보고서라면 시각 증거는 번역 과정에서 소실되며, 이것이 visual forgetting의 메커니즘이다. 다만 잠재 공간 추론은 [[cot-monitorability]]가 요구하는 외부 감시 가능성과의 새로운 긴장을 수반한다.

## 시사점

[[representation-contract]]의 재협상 사례를 제공한다 — 추론이 반드시 인간 가독 텍스트일 필요가 없다는 전제 전환. [[visual-need-routing]]·[[shallow-index-deep-answer]] 계열과 함께, 비디오 이해 연구가 '언제 무엇을 볼 것인가'에서 '추론을 어느 공간에서 수행할 것인가'로 확장되고 있음을 보여준다.

## 🔗 관련 논문

- Caption-once, Frames-on-Demand: Visual-Need Routing for Budget-Aware A
- ShallowStream: Index Shallow then Answer Deep for Streaming
- Why Is Video Still So Expensive? A Survey of Inference-Efficiency Mech

## 🏷️ 엔티티

- [[entities/visual-memory-textual-collapse.md|visual-memory-textual-collapse]]
- [[entities/cot-as-translated-report.md|cot-as-translated-report]]
- [[entities/representation-contract.md|representation-contract]]
- [[entities/multimodal-llm.md|multimodal-llm]]
- [[entities/video-understanding.md|video-understanding]]
- [[entities/latent-visual-reasoning.md|latent-visual-reasoning]]

## 📐 개념

- [[concepts/latent-visual-reasoning.md|latent-visual-reasoning]]
- [[concepts/visual-forgetting.md|visual-forgetting]]
- [[concepts/textual-coordinate-grounding.md|textual-coordinate-grounding]]
- [[concepts/latent-space-inference.md|latent-space-inference]]

---
_LLM 분석으로 생성됨_
