# extreme-low-bit-quantization

**카테고리**: 미분류
**생성일**: 2026-09-04

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-09-04-unfolding-the-leech-lattice-fused-multi-shell-deco.md|Unfolding the Leech Lattice: Fused Multi-Shell Decoding and ]]

### It's Not RoPE that Creates Sinks: The Role of Self-Concentration and V (2026-09-10)

MAs의 발생 원인을 아키텍처 구조로 설명함으로써, Leech Lattice 계열의 결과 측 양자화 최적화와 대비되는 원인 측 접근(이상치 억제)의 근본 대상을 명확히 한다.

### Forgetting Only What Matters: Layer-Selective Unlearning toward Robust (2026-09-11)

본 논문의 핵심 위협 모델이 된다. 포스트 트레이닝 양자화가 언러닝으로 제거된 지식을 부분 부활시킬 수 있음을 보여, 양자화가 단순 압축이 아니라 모델 지식 상태를 재해석하는 변환임을 실증한다.

### The Weight Is Over - Interactive Diffusion on Consumer GPUs (2026-09-22)

저비트 양자화의 적용 대상을 자회귀 LLM decode(Leech Lattice 계열)에서 확산 트랜스포머로 확장한다. 병목이 대역폭 집약적 decode가 아닌 반복적 denoising 스텝이라는 점에서 양자화의 효과 지점이 도메인에 따라 다름을 시사한다.

### StrataFlux: Memory-Hierarchy-Native Low-Bit LLM Inference (2026-11-07)

Leech Lattice 계열이 융합 커널로 저비트 형식 자체를 최적화했다면, StrataFlux는 저비트의 정확도 손실을 메모리 계층 상위의 고정밀 정제로 회복하는 보완 축을 제공한다. 양자화 품질의 귀속이 표현 형식 설계에서 계층 배치 설계로 확장됨을 보여준다.

### StrataFlux: Memory-Hierarchy-Native Low-Bit LLM Inference (2026-11-08)

Leech Lattice 계열이 커널·디코딩 수준에서 저비트 양자화 오차를 다뤘다면, StrataFlux는 메모리 계층 수준에서 정밀 데이터의 선택적 전달로 동일 문제를 공략한다. 저비트 양자화의 실용화가 단일 계층 기법이 아니라 커널-시스템 협업 설계의 산물임을 보여준다.
