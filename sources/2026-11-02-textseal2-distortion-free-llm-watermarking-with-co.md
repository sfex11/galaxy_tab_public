# TextSeal2: Distortion-Free LLM Watermarking with Copula Mixing and Memoryless Races

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-02
**링크**: http://arxiv.org/abs/2610.40613v1

## 💡 핵심 인사이트

왜곡 없는 워터마크가 추측 디코딩 아래에서 생존하려면 거절 드래프트 대체 토큰까지 동일 키로 워터마킹되어야 하고, 키 분할 설계가 검출기 신호 품질을 결정한다 — provenance와 추론 가속의 공존 조건을 확립한다.

## 📖 분석

### TextSeal2: Distortion-Free LLM Watermarking with Copula Mixing and Memoryless Races (2026-11-02)

원천 재등록으로 분석을 심화한다. 왜곡 없는 워터마킹의 내구성 조건을 확립한다 — 거절 드래프트를 대체하는 토큰도 동일 키로 워터마킹되어야 검출 신호가 유지되며, 워터마크 평가가 단독 생성 환경에서 추측 디코딩 결합 환경으로 확장되어야 한다.

신규 인사이트는 검출기 신호 설계 차원이다. 전신 TextSeal의 코인 플립 이중 키 라우팅은 검출기가 두 키의 점수를 평균하게 만들어 신호를 희석한다. TextSeal2의 copula mixing과 memoryless races는 키 분할이 곧 측정 분할임을 드러낸다 — [[detector-as-instrument]] 관점에서 검출기의 신뢰성이 생성 측 키 배치 설계에 의존함을 시사한다.

[[watermarkable-speculative-sampling]]과의 대칭도 주목할 만하다. Poisson 과정 계열이 추측 샘플링을 워터마크 인지적으로 재설계했다면, 본 논문은 워터마킹을 추측 디코딩에 견고하게 만드는 반대 방향이며, 두 경로의 수렴 요구는 단일하다: 검출 신호는 가속 기제를 생존해야 한다. 수용률 무변경·지연 무추가·다양성 보존은 [[efficiency-provenance-tension]]이 공존 가능함을 실증하고, 분포 무변경 원칙([[distribution-preserving-acceleration]])이 가속뿐 아니라 provenance 신호 유지의 전제임을 확장한다.

## 🔗 관련 논문

- Watermarkable Multi-Draft Speculative Sampling via Poisson P

## 🏷️ 엔티티

- [[entities/llm-watermarking.md|llm-watermarking]]
- [[entities/speculative-decoding.md|speculative-decoding]]
- [[entities/detector-as-instrument.md|detector-as-instrument]]
- [[entities/distribution-preserving-acceleration.md|distribution-preserving-acceleration]]

## 📐 개념

- [[concepts/distortion-free-watermarking.md|distortion-free-watermarking]]
- [[concepts/watermarkable-speculative-sampling.md|watermarkable-speculative-sampling]]
- [[concepts/output-provenance.md|output-provenance]]
- [[concepts/efficiency-provenance-tension.md|efficiency-provenance-tension]]

---
_LLM 분석으로 생성됨_
