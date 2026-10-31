# TextSeal2: Distortion-Free LLM Watermarking with Copula Mixing and Memoryless Races

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-31
**링크**: http://arxiv.org/abs/2610.40613v1

## 💡 핵심 인사이트

왜곡 없는 워터마크의 내구성은 거절된 드래프트를 대체하는 토큰의 키 계승으로 결정되며, 검출기의 통계 구조와 워터마크 설계는 공동 최적화 대상이다.

## 📖 분석

TextSeal2는 왜곡 없는(distortion-free) LLM 워터마킹이 추측 디코딩 환경에서도 검출 신호를 유지하는 문제를 해결한다. 거절된 드래프트를 대체하는 토큰도 동일 키로 워터마킹되어 신호가 계승되며, 수용률·출력 다양성·추론 지연 모두 무변화를 달성한다.

[[watermarkable-speculative-sampling]] 계열(Poisson Processes, 2026-09-22)이 다중 드래프트 추측 샘플링에 워터마크를 내장하는 경로를 열었다면, 본 논문은 드래프트가 거절·교체되는 순간에도 워터마크가 계승되는 '내구성' 축을 완성한다. [[efficiency-provenance-tension]]을 무지연·무왜곡 조건으로 해소한 사례다.

전신 TextSeal의 동전 던지기 키 라우팅이 검출기의 스코어 평균화 구조에서 차선이었음을 진단하고, copula mixing으로 키 혼합을 재설계한다. 이는 워터마크 검출기를 계측기로 다루는 [[detector-as-instrument]] 관점에서, 계측기의 통계 구조와 워터마크 설계가 공동 최적화 대상임을 보여준다.

출력 분포에 내장된 통계적 흔적이라는 [[output-provenance]] 메커니즘이 [[speculative-decoding]]과의 조합에 대해 닫혀야 한다는 요구를 형식화하며, [[llm-watermarking]] 연구의 평가 축을 '삽입 가능성'에서 '생성 파이프라인 조합 하 내구성'으로 확장한다.

## 🔗 관련 논문

- Watermarkable Multi-Draft Speculative Sampling via Poisson Processes

## 🏷️ 엔티티

- [[entities/llm-watermarking.md|llm-watermarking]]
- [[entities/speculative-decoding.md|speculative-decoding]]
- [[entities/detector-as-instrument.md|detector-as-instrument]]

## 📐 개념

- [[concepts/watermarkable-speculative-sampling.md|watermarkable-speculative-sampling]]
- [[concepts/multi-draft-speculative-sampling.md|multi-draft-speculative-sampling]]
- [[concepts/output-provenance.md|output-provenance]]
- [[concepts/efficiency-provenance-tension.md|efficiency-provenance-tension]]
- [[concepts/poisson-process-draft-selection.md|poisson-process-draft-selection]]
- [[concepts/distortion-free-watermarking.md|distortion-free-watermarking]]

---
_LLM 분석으로 생성됨_
