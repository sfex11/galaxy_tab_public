# On-Demand Attention: Language Models Know When to Recall

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-19
**링크**: http://arxiv.org/abs/2609.20734v1

## 💡 핵심 인사이트

사전학습 모델의 디코딩 상태는 전역 어텐션을 수행하기 전에 이미 그 필요성을 인코딩하고 있어, 컨텍스트 히스토리 읽기를 내부 신호가 트리거하는 온디맨드 연산으로 전환할 수 있다.

## 📖 분석

**On-Demand Attention (ODA)**: 사전학습 모델의 디코딩 상태는 전역 어텐션(global read)을 수행하기 *전에* 이미 '이번 스텝에서 히스토리 읽기가 다음 예측에 유익한가'를 예측하는 정보를 담는다. ODA는 경량 recall head로 이 신호를 판독하여, 국소 윈도우 우선 디코딩에서 필요한 순간에만 전역 어텐션을 소환하는 local-first 방법이다.

Wiki 지형에서 이 논문은 세 간선으로 연결된다.

1. **지연 실행 원리의 신규 도메인** — [[lazy-schema-loading]]이 지연 실행을 '스키마→픽셀'을 아우르는 도메인 불변 패턴으로 규정했다면, ODA는 같은 원리를 컨텍스트 히스토리에 적용한다. [[on-demand-frame-fetch]]가 시각 원본을 소급 인출했다면 ODA는 어텐션 접근을 소급 인출하며, '필요 전까지 로드하지 않는다'는 원리가 외부 자원을 넘어 모델 내부 연산 수준까지 내려옴을 보여준다.

2. **내부 판독의 효율화 응용** — [[internal-prediction-readout]]의 판독 대상을 '수행되지 않은 연산의 이익'으로 확장한다. [[router-within]]이 스킬 게이팅을 동결 모델 내재 신호의 판독으로 환원했다면, ODA는 어텐션 게이팅을 동일하게 환원한다.

3. **국소 충분성의 어텐션 실현** — [[local-sufficiency]](Select to Think)의 국소 충분성 판단을 토큰 선택에서 어텐션 스코프로 옮긴다. recall head는 [[expected-value-of-information]]의 학습된 근사기이며, [[adaptive-inference]]의 결정 차원에 '전역 읽기 수행 여부'라는 새 축을 추가한다.

## 🔗 관련 논문

- Caption-once, Frames-on-Demand: Visual-Need Routing for Budget-Aware A
- The Router Within: Eliciting Native Skill Routing from a Fro
- Select to Think: Unlocking SLM Potential with Local
- Beyond Truncation: Rethinking LLM Decoding as Ensemble Pruni

## 🏷️ 엔티티

- [[entities/on-demand-attention.md|on-demand-attention]]
- [[entities/lazy-schema-loading.md|lazy-schema-loading]]
- [[entities/on-demand-frame-fetch.md|on-demand-frame-fetch]]
- [[entities/internal-prediction-readout.md|internal-prediction-readout]]
- [[entities/local-sufficiency.md|local-sufficiency]]
- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/expected-value-of-information.md|expected-value-of-information]]
- [[entities/sparse-attention-unification.md|sparse-attention-unification]]

## 📐 개념

- [[concepts/router-within.md|router-within]]
- [[concepts/internal-state-responsive-adaptation.md|internal-state-responsive-adaptation]]
- [[concepts/shallow-index-deep-answer.md|shallow-index-deep-answer]]

---
_LLM 분석으로 생성됨_
