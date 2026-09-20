# On-Demand Attention: Language Models Know When to Recall

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-21
**링크**: http://arxiv.org/abs/2609.20734v1

## 💡 핵심 인사이트

사전학습된 디코딩 상태가 전역 읽기 이전에 그 이익을 이미 부호화한다는 발견은, 스파스 어텐션 최적화의 단위를 '무엇을 건너뛸까'에서 '언제 읽을까'로 전환하고, 모델 내부 판독이 사전 연산 판단의 근거가 될 수 있음을 입증한다.

## 📖 분석

# On-Demand Attention: Language Models Know When to Recall (2026-09-21)

_2026-09-19/20 소스 엔트리의 통합·심화 버전으로, 산재한 엔티티 노트를 하나의 이해로 정리한다._

## 핵심 발견
사전학습된 모델의 디코딩 상태가 전역 읽기(global read)를 수행하기 **이전에** 그 이익을 이미 예측한다. 이는 full-attention 디코딩이 매 스텝 성장하는 역사를 무조건 읽으며 예측에 불필요한 읽기를 수행한다는 진단 위에 서 있다.

## ODA: local-first 디코딩
경량 recall head가 국소 디코딩 상태를 판독해 전역 어텐션의 기대 이익을 추정하고, 이익이 예측될 때만 전역 읽기를 호출한다. 스파스 어텐션의 질문을 "무엇을 건너뛸까"에서 "언제 읽을까"로 전환한다.

## 기존 Wiki와의 통합
- [[sparse-attention-unification]]·[[hierarchical-kv-memory]]가 정적 희소성(지역성·계층 메모리) 축이라면, ODA는 동적 필요성 예측이라는 대안 축을 추가한다.
- [[internal-prediction-readout]]의 확장: 판독 대상이 출력 길이 같은 미래 산출 속성에서 '수행되지 않은 연산의 이익'으로 이동한다.
- [[expected-value-of-information]]의 어텐션 도메인 실현: recall head는 도구 호출 판단에서 정의된 EVI 추정기가 접근 판단으로 이식된 사례다.
- [[local-sufficiency]]: 국소 충분성 판단이 토큰 선택에서 컨텍스트 읽기로 확장된다.
- [[lazy-schema-loading]]·[[on-demand-frame-fetch]]·[[shallow-index-deep-answer]]와 함께 '필요할 때만 접근' 원리가 도구 스키마→시각 프레임→어텐션 읽기로 일반화됨을 확인시킨다.
- [[internal-state-responsive-adaptation]]: 외부 환경(CADENCE 계열), 내부 압축 상태(SpecKV 계열)에 이은 적응 트리거의 제3 유형 — 내부 표현이 부호화한 예측 신호 — 을 제공한다.

## 시사점
추론·에이전틱 워크로드에서 비용의 지배 변수가 생성 토큰 수가 아니라 컨텍스트 읽기 횟수일 때, [[kv-cache-optimization]]('캐시를 어떻게 줄일까')과 직교하는 새 축 — '캐시를 언제 읽을까' — 이 열리고, 최적화 단위가 연산량에서 필요성 판정으로 이동한다.

## 🔗 관련 논문

- On-Demand Attention: Language Models Know When to Recall
- Unifying Sparse Attention with Hierarchical Memory for Scala
- Caption-once, Frames-on-Demand: Visual-Need Routing for Budget-Aware A
- Select to Think: Unlocking SLM Potential with Local Sufficie
- ShallowStream: Index Shallow then Answer Deep for Streaming

## 🏷️ 엔티티

- [[entities/on-demand-attention.md|on-demand-attention]]
- [[entities/sparse-attention-unification.md|sparse-attention-unification]]
- [[entities/internal-prediction-readout.md|internal-prediction-readout]]
- [[entities/expected-value-of-information.md|expected-value-of-information]]
- [[entities/local-sufficiency.md|local-sufficiency]]
- [[entities/internal-state-responsive-adaptation.md|internal-state-responsive-adaptation]]
- [[entities/lazy-schema-loading.md|lazy-schema-loading]]
- [[entities/shallow-index-deep-answer.md|shallow-index-deep-answer]]
- [[entities/kv-cache-optimization.md|kv-cache-optimization]]
- [[entities/long-context.md|long-context]]

## 📐 개념

- [[concepts/benefit-predictive-decoding-state.md|benefit-predictive-decoding-state]]
- [[concepts/on-demand-resource-access.md|on-demand-resource-access]]
- [[concepts/expected-value-of-information.md|expected-value-of-information]]
- [[concepts/internal-state-responsive-adaptation.md|internal-state-responsive-adaptation]]

---
_LLM 분석으로 생성됨_
