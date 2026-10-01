# LeapQuant: Efficient Linear Attention with Accurate Recurrent State Quantization

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-01
**링크**: http://arxiv.org/abs/2609.38166v1

## 💡 핵심 인사이트

선형 어텐션의 순환 상태 양자화는 오차가 매 재귀 갱신마다 누적되므로, 양자화가 단순 압축이 아니라 반복 갱신되는 상태의 정보 동역학 보존 문제임을 밝힌다.

## 📖 분석

LeapQuant는 Gated DeltaNet(GDN), Kimi Delta Attention(KDA) 계열의 선형 어텐션 하이브리드 아키텍처에서 컨텍스트를 압축하는 고정 크기 순환 상태(recurrent state)의 정확한 양자화 방법을 제시한다. 선형 어텐션은 표준 어텐션을 대체해 KV 캐시 팽창이라는 서빙 병목([[kv-cache-optimization]])을 구조적으로 우회하지만, 상태는 매 토큰 스텝마다 반복적으로 읽히고 갱신되므로 양자화 오차가 단발성 가중치 양자화([[model-compression]])와 달리 재귀를 통해 누적·증폭되어 품질 저하로 직결된다. 이는 극저비트 양자화([[extreme-low-bit-quantization]]) 연구가 디코딩 계층의 결과 측 최적화에 집중했던 것과 대비되는, 상태 갱신 연산 자체의 오차 동역학에 대한 접근이다. TIM([[training-inference-mismatch]])이 수치 충실도가 훈련 안정성을 결정했듯, 본 논문은 추론 효율화에서도 '어디를 양자화하는가'가 단순 비용 문제를 넘어 반복 갱신되는 상태의 정보 동역학 보존 문제임을 보여준다. 장기 컨텍스트([[long-context]]) 처리 비용 절감에서 캐시 압축 계열과 병렬되는 제2 경로를 형성한다.

## 🔗 관련 논문

- Unfolding the Leech Lattice: Fused Multi-Shell Decoding and 
- SpecKV: Adaptive Speculative Decoding with Compression-Aware
- Make Your LVLM KV Cache More Lightweight
- Score Centering Stabilizes Off-policy Reinforcement Learning

## 🏷️ 엔티티

- [[entities/linear-attention.md|linear-attention]]
- [[entities/recurrent-state-quantization.md|recurrent-state-quantization]]

## 📐 개념

- [[concepts/quantization-error-accumulation.md|quantization-error-accumulation]]
- [[concepts/linear-attention-recurrent-state.md|linear-attention-recurrent-state]]

---
_LLM 분석으로 생성됨_
