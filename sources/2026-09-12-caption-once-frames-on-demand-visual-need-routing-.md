# Caption-once, Frames-on-Demand: Visual-Need Routing for Budget-Aware Agentic Long Video Understanding

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-12
**링크**: http://arxiv.org/abs/2609.11899v1

## 💡 핵심 인사이트

언어 메모리와 픽셀의 기능적 우위가 상보적이라는 시각-텍스트 이중성에 근거해, 시각 증거가 필요한 순간만 프레임을 검색하는 라우팅이 하위 샘플링과 텍스트 전용 메모리의 정보 소실 딜레마를 동시에 해결한다.

## 📖 분석

CFD(Caption-once, Frames-on-Demand)는 장시간 비디오 이해의 예산 제약을 시각-텍스트 이중성 위에서 해결하는 에이전틱 라우팅 시스템이다. 언어 메모리는 장기 시간 구조 보존에 우위를, 픽셀은 속성 수준 지각에 결정적이라는 관찰이 설계의 근거다.

**Wiki 축적과의 관계**

1. [[shallow-index-deep-answer]]의 모달리티 확장 — ShallowStream이 지연 실행을 인덱스 계층에 적용했다면, CFD는 이를 시각 증거 계층으로 이동시켜 '캡션 1회→프레임 온디맨드'라는 지연 관찰 패턴을 수립한다. Seeing Before Synthesizing이 관찰 선행 원칙(훈련 데이터 축)이라면 CFD는 추론 시점 지연 관찰(예산 축)로 상보적 위치를 형성한다.

2. [[visual-memory-textual-collapse]]에 대한 구조적 응답 — 텍스트 전용 메모리의 시각 속성 소실을 인정하되 망각 보상을 온디맨드 재관찰로 대체한다. 시각 필요성 라우팅이 붕괴 비용을 질의 유형별로 관리 가능하게 만든다.

3. [[video-inference-efficiency]] 서베이(2026-09-11)에 새 축 추가 — 시각 토큰 전면 처리 대신 증거가 필요한 순간만 검색하는 것이 장시간 비디오의 지배적 비용 절감 축임을 보여준다.

4. [[lazy-schema-loading]]과 동형 구조 — 도구 스키마가 아닌 프레임을 지연 로딩함으로써 '불필요한 컨텍스트 원천 차단' 원리가 도구 계층에서 지각 계층으로 확장된다.

5. [[modality-asymmetric-memory-cost]]를 기능적 우위 비대칭으로 보완 — 비용 비대칭에 기능 비대칭(시간 구조 vs 속성 지각)을 결합한 이중 구조를 제시한다.

라우팅 결정은 [[expected-value-of-information]]의 구현이며 [[adaptive-inference]]의 축을 '얼마나 계산할까'에서 '언제 볼까'로 확장한다. [[strategy-routing]]과 대비해 라우팅 변수가 샘플 특성이 아닌 질의의 인식 요구임을 보인다. 엣지 제약 하에서 [[on-device-inference]] 프론티어를 이동시키고, [[caption-sufficient-evaluation]]의 역문제(언제 캡션이 불충분한가)를 런타임 판별 문제로 전환한다.

## 🔗 관련 논문

- ShallowStream: Index Shallow then Answer Deep for Streaming Video Understanding
- Why Is Video Still So Expensive? A Survey of Inference-Efficiency Mechanisms
- ConvMem: Convolutional Memory for Long-Context Reasoning
- Make Your LVLM KV Cache More Lightweight
- Seeing Before Synthesizing: VLM-Guided Transition Event Discovery
- Beyond One-Size-Fits-All: Sample-Adaptive Strategy Routing for Vision

## 🏷️ 엔티티

- [[entities/video-understanding.md|video-understanding]]
- [[entities/shallow-index-deep-answer.md|shallow-index-deep-answer]]
- [[entities/video-inference-efficiency.md|video-inference-efficiency]]
- [[entities/modality-asymmetric-memory-cost.md|modality-asymmetric-memory-cost]]
- [[entities/visual-memory-textual-collapse.md|visual-memory-textual-collapse]]
- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/on-device-inference.md|on-device-inference]]
- [[entities/agentic-vlm.md|agentic-vlm]]
- [[entities/expected-value-of-information.md|expected-value-of-information]]
- [[entities/lazy-schema-loading.md|lazy-schema-loading]]
- [[entities/strategy-routing.md|strategy-routing]]

## 📐 개념

- [[concepts/visual-need-routing.md|visual-need-routing]]
- [[concepts/visual-textual-duality.md|visual-textual-duality]]
- [[concepts/caption-sufficient-evaluation.md|caption-sufficient-evaluation]]

---
_LLM 분석으로 생성됨_
