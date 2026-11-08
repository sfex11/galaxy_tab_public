# agent-native-serving

**카테고리**: 미분류
**생성일**: 2026-09-24

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-09-24-swe-serve-benchmarking-agentic-engineering-for-pro.md|SWE-Serve: Benchmarking Agentic Engineering For Production I]]

### EAServe: Encode-Aware Disaggregated Serving for Multimodal Large Langu (2026-09-29)

위상 수준 자원 분리라는 새로운 서빙 최적화 축을 추가한다. Pythia가 예측가능성 기반 서빙을 제안했다면, 본 논문은 멀티모달 워크로드의 위상 이질성(Encode-Prefill-Decode)에 맞춘 자원 풀 분리로 에이전트 네이티브 서빙의 설계 공간을 확장한다.

### TokenCast: Forecasting Token Consumption During LLM Agent Execution (2026-09-30)

에이전트 네이티브 서빙이 워크로드의 의미적 이질성(Pythia)과 위상 이질성(EAServe)에 이어 '예측 가능한 총비용'이라는 계획 입력을 획득한다. 비용 예측이 스케줄링·리소스 예약의 1급 신호가 되는 경로를 연다.

### Flide: Accelerating Decision Inference with Exact State Forking (2026-11-03)

결정 모델이라는 새 워크로드 클래스를 서빙 설계 공간에 추가하고, '논리 트리-물리 배치 분리'라는 새 설계 요구를 제시한다. 에이전트 워크로드 특성이 서빙 인프라 아키텍처를 결정하는 인과 방향을 강화한다.

→ [[sources/2026-11-03-flide-accelerating-decision-inference-with-exact-s.md|상세 보기]]

### Latent Sparse Attention: Towards Subquadratic Ultra-Long Context Atten (2026-11-03)

초장기 컨텍스트 서빙 비용이라는 에이전트 워크로드 고유의 병목에 대해 아키텍처 계층 해법을 제공한다. [[schema-accumulation-bottleneck]]이 인프라·프롬프트 계층의 최적화를 다뤘다면, 본 논문은 모델 내부 어텐션 구조에서 직접 에이전트 장기 실행을 수용하는 경로를 보여준다.

→ [[sources/2026-11-03-latent-sparse-attention-towards-subquadratic-ultra.md|상세 보기]]

### ACCT: Asymmetric Cross-LLM Context Transfer (2026-11-03)

에이전트 네이티브 서빙의 설계 공간에 '크로스 모델 캐시 이식성'이라는 새 프리미티브를 추가한다. KV-streams가 훈련 루프 내 반복 프리필 병목을 제거했다면 본 논문은 배포 시 이종 모델 호출의 동일 병목을 제거하여, 반복 프리필 제거 패턴이 훈련·배포 양축으로 확장됨을 보여준다.

→ [[sources/2026-11-03-acct-asymmetric-cross-llm-context-transfer.md|상세 보기]]

### StrataFlux: Memory-Hierarchy-Native Low-Bit LLM Inference (2026-11-07)

서빙 인프라의 메모리 계층 설계가 모델 정확도(능력)를 직접 결정하는 구조적 사례를 추가한다. 서빙 계층이 품질에 중립적이라는 전제가 정밀도 차원에서도 기각됨을 보여준다.

→ [[sources/2026-11-07-strataflux-memory-hierarchy-native-low-bit-llm-inf.md|상세 보기]]

### StrataFlux: Memory-Hierarchy-Native Low-Bit LLM Inference (2026-11-08)

에이전트 워크로드의 장기 컨텍스트 KV 캐시가 HBM을 초과하는 상황에서 계층 네이티브 추론이 실용 조건을 강화한다. 에이전트 네이티브 서빙의 비용·용량 논의에 메모리 계층 설계라는 새 축을 추가한다.

→ [[sources/2026-11-08-strataflux-memory-hierarchy-native-low-bit-llm-inf.md|상세 보기]]
