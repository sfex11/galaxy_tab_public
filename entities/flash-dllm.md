# flash-dllm

**카테고리**: 미분류
**생성일**: 2026-09-24

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-09-24-flash-dllm-io-aware-kv-caching-and-parallel-decodi.md|Flash-dLLM: IO-Aware KV Caching and Parallel Decoding for Fa]]

### EAServe: Encode-Aware Disaggregated Serving for Multimodal Large Langu (2026-09-29)

IO 인지 캐싱-디코딩 최적화와 위상 분리가 상보적 서빙 전략을 형성함을 보여준다. 후자는 위상 간 자원을 분리하고 전자는 위상 내 캐시-디코딩 결합을 최적화한다.

### The SIMPLE Law for Energy Cost of LLM Inference (2026-11-04)

IO 인지 캐싱·병렬 디코딩이 공략하는 메모리 접근 병목에 해석적 비용 근거를 공급한다. 디코딩 페이즈 메모리 접근 복잡도의 폐쇄형이 IO-aware 설계의 수익 구조를 사전 계산 가능하게 하여, 캐시-디코딩 결합 최적화의 정당화가 측정에서 법칙으로 이동한다.

→ [[sources/2026-11-04-the-simple-law-for-energy-cost-of-llm-inference.md|상세 보기]]

### StrataFlux: Memory-Hierarchy-Native Low-Bit LLM Inference (2026-11-07)

IO 인지 최적화의 목표 차원을 확장한다. Flash-dLLm이 IO를 은닉해 처리량을 지키는 결합이었다면 StrataFlux는 IO 자체를 정확도 회복의 통로로 사용하여, 서빙 인프라가 품질 결정에 직접 개입하는 [[capability-forming-serving]]의 정밀도 차원 사례를 추가한다.

→ [[sources/2026-11-07-strataflux-memory-hierarchy-native-low-bit-llm-inf.md|상세 보기]]

### StrataFlux: Memory-Hierarchy-Native Low-Bit LLM Inference (2026-11-08)

Flash-dLLM의 IO 인지 캐싱-디코딩 최적화가 HBM 내부에 머물렀다면, StrataFlux는 최적화 대상을 호스트 RAM·SSD까지 포괄하는 메모리 계층 전체로 확장한다. IO 인지 설계가 칩 경계를 넘어 계층 간 데이터 흐름으로 일반화됨을 보여준다.

→ [[sources/2026-11-08-strataflux-memory-hierarchy-native-low-bit-llm-inf.md|상세 보기]]
