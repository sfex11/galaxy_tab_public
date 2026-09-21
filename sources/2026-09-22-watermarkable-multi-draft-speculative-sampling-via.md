# Watermarkable Multi-Draft Speculative Sampling via Poisson Processes

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-22
**링크**: http://arxiv.org/abs/2609.21858v1

## 💡 핵심 인사이트

분포 보존을 요구하는 추론 가속과 분포 변형을 요구하는 워터마킹이라는 양립 불가능으로 여겨진 두 서빙 목표가, Poisson 과정 기반 다중 드래프트 설계로 공존 가능함을 보여준다.

## 📖 분석

LLM 배포의 두 핵심 요구 — 추론 효율(speculative sampling)과 출력 출처 증명(watermarking) — 의 결합 가능성을 규명한다. 기존 연구는 이 결합이 근본적으로 어렵거나 불가능할 수 있음을 보였다: 추측 샘플링은 타겟 분포의 무손실 보존을 전제로 하는 반면, 워터마킹은 검출 가능한 통계적 흔적을 위해 분포 변형을 요구하기 때문이다.

본 논문은 Poisson 과정 기반 다중 드래프트 추측 샘플링으로 이 긴장을 해소한다. [[speculative-decoding-losslessness-premise-collapse]]에 무손실 전제 붕괴의 새 발현 유형을 추가한다 — 기존 사례가 파이프라인 스키마 축적으로 컨텍스트가 어긋나는 우연적 붕괴였다면, 본 논문은 워터마킹이라는 규범적 요구가 의도적으로 전제를 재협상하는 유형이다.

[[distribution-preserving-acceleration]] 축에서, DBTM이 고정점 수렴으로 무손실성 정의를 확장했다면 본 논문은 워터마크 삽입 가능성이라는 제3의 보장 축을 열어, 가속의 보장 체계가 단일 정의가 아니라 목적별 다중 체계임을 시사한다. 다중 드래프트 역학은 [[parallel-token-sampling]]에 Poisson 과정이라는 확률 구조를 부여한다.

신규 엔티티 **llm-watermarking**은 [[detector-as-instrument]](워터마크 검출기가 출력 감사의 계측기) 및 [[serving-safety-coupling]](출처 증명의 서빙 파이프라인 편입)과 연결된다.

## 🔗 관련 논문

- Unlocking Lossless Speedups in LLMs via Discrete Diffusion
- Discrete Beckmann Transport Models for One-Step Language Modeling and Beyond
- SpecKV: Adaptive Speculative Decoding with Compression-Aware Gamma Selection

## 🏷️ 엔티티

- [[entities/speculative-decoding.md|speculative-decoding]]
- [[entities/distribution-preserving-acceleration.md|distribution-preserving-acceleration]]
- [[entities/parallel-token-sampling.md|parallel-token-sampling]]
- [[entities/speculative-decoding-losslessness-premise-collapse.md|speculative-decoding-losslessness-premise-collapse]]
- [[entities/llm-watermarking.md|llm-watermarking]]
- [[entities/detector-as-instrument.md|detector-as-instrument]]
- [[entities/serving-safety-coupling.md|serving-safety-coupling]]

## 📐 개념

- [[concepts/watermarkable-speculative-sampling.md|watermarkable-speculative-sampling]]
- [[concepts/output-provenance.md|output-provenance]]
- [[concepts/poisson-process-draft-selection.md|poisson-process-draft-selection]]
- [[concepts/efficiency-provenance-tension.md|efficiency-provenance-tension]]
- [[concepts/multi-draft-speculative-sampling.md|multi-draft-speculative-sampling]]

---
_LLM 분석으로 생성됨_
