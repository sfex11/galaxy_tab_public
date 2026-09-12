# Caption-once, Frames-on-Demand: Visual-Need Routing for Budget-Aware Agentic Long Video Understanding

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-13
**링크**: http://arxiv.org/abs/2609.11899v1

## 💡 핵심 인사이트

장시간 비디오 이해의 병목은 시각 토큰을 얼마나 압축할 것인가가 아니라 언제 픽셀을 볼 것인가이며, 언어의 시간 구조 우위와 픽셀의 속성 지각 우위라는 시각-텍스트 이중성이 이 라우팅의 이론적 근거다.

## 📖 분석

본 논문은 시각-텍스트 이중성을 관찰한다: 언어 메모리는 밀집 프레임보다 장기 시간 구조를 잘 보존하는 반면, 픽셀은 속성 수준 지각에 결정적이다. 이에 기반한 CFD(Caption-once, Frames-on-Demand)는 비디오를 한 번 캡션하여 언어 메모리를 구축하고, 에이전트가 속성 수준 시각 증거가 필요한 순간에만 프레임을 검색한다. 이는 2026-09-11 비디오 추론 효율 서베이([[video-inference-efficiency]])가 정리한 압축·프루닝 지형에 '시각 필요성 기반 라우팅'이라는 새 축을 추가하여, 비용 절감의 결정 단위가 토큰 감축에서 관찰 시점으로 이동함을 보여준다. [[shallow-index-deep-answer]]의 지연 실행과 [[lazy-schema-loading]]의 지연 로딩이 시각 도메인으로 확장되어, '필요하기 전까지 로드하지 않는다'는 원리가 스키마·인덱스·프레임을 아우르는 범용 패턴임이 확인된다. [[visual-memory-textual-collapse]]에 대해서는 구조적 해법을 제공한다 — 텍스트 붕괴를 수용하되 프레임 회복 경로를 열어 붕괴 비용을 선택적·지연적으로 지불하는 설계로 전환한다. [[expected-value-of-information]] 관점에서 시각 필요성 판단은 프레임 검색이라는 정보 수집 행위의 기대 가치가 예산 비용을 초과하는가의 비교로 정식화되며, 엣지 디바이스의 대역폭 제약 하 베이즈 의사결정의 구체화다. [[visual-need-routing]]은 런타임 관찰 결정이라는 조작적 정의를, [[visual-textual-duality]]는 모달리티 배치의 이론적 근거를 확립한다.

## 🔗 관련 논문

- Why Is Video Still So Expensive? A Survey of Inference-Efficiency Mech
- ShallowStream: Index Shallow then Answer Deep for Streaming
- Make Your LVLM KV Cache More Lightweight
- Seeing Before Synthesizing: VLM-Guided Transition Event Discovery for

## 🏷️ 엔티티

- [[entities/visual-need-routing.md|visual-need-routing]]
- [[entities/visual-textual-duality.md|visual-textual-duality]]
- [[entities/visual-memory-textual-collapse.md|visual-memory-textual-collapse]]
- [[entities/video-inference-efficiency.md|video-inference-efficiency]]
- [[entities/shallow-index-deep-answer.md|shallow-index-deep-answer]]
- [[entities/lazy-schema-loading.md|lazy-schema-loading]]
- [[entities/adaptive-inference.md|adaptive-inference]]

## 📐 개념

- [[concepts/expected-value-of-information.md|expected-value-of-information]]
- [[concepts/modality-asymmetric-memory-cost.md|modality-asymmetric-memory-cost]]
- [[concepts/caption-sufficient-evaluation.md|caption-sufficient-evaluation]]
- [[concepts/token-pruning.md|token-pruning]]
- [[concepts/on-device-inference.md|on-device-inference]]
- [[concepts/strategy-routing.md|strategy-routing]]

---
_LLM 분석으로 생성됨_
