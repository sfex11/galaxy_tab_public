# It's Not RoPE that Creates Sinks: The Role of Self-Concentration and Value-Non-Mixing in Attention

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-10
**링크**: http://arxiv.org/abs/2609.09085v1

## 💡 핵심 인사이트

Attention Sink와 Massive Activations는 RoPE가 아니라 인과 마스크가 유도하는 어텐션 자기 집중과 Value-non-mixing의 구조적 귀결로서, 토큰 내용과 무관한 아키텍처 고유 속성이다.

## 📖 분석

# It's Not RoPE that Creates Sinks

LLM의 시퀀스 초기 위치에서 발생하는 Attention Sink(AS)와 Massive Activations(MAs)의 인과적 원인을 규명한 기계론적 연구다. 기존 가설이 RoPE를 원인으로 지목했으나, 본 논문은 인과 마스크가 유도하는 어텐션 자기 집중(self-concentration)과 후속 Value-non-mixing이 실제 원인임을 실험으로 보여준다. AS/MAs는 해당 위치의 토큰 내용과 무관하게 발생한다.

Wiki 관점에서 이 논문의 기여는 세 가지다. 첫째, [[extreme-low-bit-quantization]]과 직결된다 — MAs는 저비트 양자화의 주요 장애물인데, 그 기원을 마스크 구조라는 아키텍처 고유 원인으로 추적함으로써 이상치 후처리가 아닌 구조적 원인 겨냥 해법의 방향을 제시한다. Leech Lattice 양자화 연구와 상보적 위치(결과 측 최적화 vs 원인 측 규명)를 형성한다. 둘째, 원인 오귀인 교정의 메커니즘 수준 사례다 — [[bottleneck-misattribution]]이 서빙 병목의 오귀인을 다룬다면, 본 논문은 어텐션 현상의 원인(RoPE) 오귀인을 개입 실험으로 교정하는 동형 구조를 보인다. 셋째, [[residual-stream-monitoring]]과 연결되어 잔류 스트림 극단 활성화의 기계론적 근거를 제공한다.

또한 에이전트 수준의 [[attention-stability-boundary]]·[[attention-latch]] 논의와 대비된다: 개체 수준에서 병리적 불안정으로 다뤄지는 어텐션 집중이, 메커니즘 수준에서는 인과 마스크의 구조적 귀결임을 밝혀 분석 계층 간 어텐션 연구의 대응 관계를 연결한다.

## 🔗 관련 논문

- Unfolding the Leech Lattice: Fused Multi-Shell Decoding and

## 🏷️ 엔티티

- [[entities/attention-sink.md|attention-sink]]
- [[entities/massive-activation.md|massive-activation]]
- [[entities/value-non-mixing.md|value-non-mixing]]
- [[entities/attention-self-concentration.md|attention-self-concentration]]
- [[entities/extreme-low-bit-quantization.md|extreme-low-bit-quantization]]
- [[entities/mechanistic-interpretability.md|mechanistic-interpretability]]
- [[entities/residual-stream-monitoring.md|residual-stream-monitoring]]

## 📐 개념

- [[concepts/attention-self-concentration.md|attention-self-concentration]]
- [[concepts/value-non-mixing.md|value-non-mixing]]
- [[concepts/causal-mask-induced-bias.md|causal-mask-induced-bias]]

---
_LLM 분석으로 생성됨_
