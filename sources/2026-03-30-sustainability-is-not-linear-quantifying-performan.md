# Sustainability Is Not Linear: Quantifying Performance, Energy, and Privacy Trade-offs in On-Device Intelligence

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-30
**링크**: http://arxiv.org/abs/2603.26603v1

## 💡 핵심 인사이트

LLM의 온디바이스 배포에서 모델 크기·양자화·에너지·프라이버시 간의 트레이드오프는 비선형적이며, 단순한 모델 축소가 최적 해가 아님을 실증적으로 증명했다.

## 📖 분석

## Sustainability Is Not Linear: Quantifying Performance, Energy, and Privacy Trade-offs in On-Device Intelligence

본 논문은 대규모 언어 모델(LLM)을 클라우드에서 엣지 디바이스(모바일 기기)로 이전할 때 발생하는 에너지 소비, 지연 시간, 품질 간의 복잡한 트레이드오프를 실험적으로 정량화한 연구이다. 이론적 분석에 그치지 않고, 재현 가능한 실험 파이프라인을 구축하여 모바일 배터리, 열 제한, 메모리 제약 등 물리적 한계 하에서의 세밀한 프로파일링을 수행했다.

### 핵심 기여
- **비선형 트레이드오프 발견**: 모델 크기, 양자화 수준, 추론 성능, 에너지 효율 간의 관계가 단순 선형이 아님을 실증적으로 보여줌
- **프라이버시-성능 축**: 온디바이스 추론이 제공하는 프라이버시 이점과 성능 저하 사이의 균형점을 정량적으로 분석
- **재현 가능한 벤치마킹 파이프라인**: 엣지 디바이스에서의 LLM 배포를 위한 체계적 평가 방법론 제시

### 기존 Wiki와의 연결
본 연구는 [[differential-privacy]] 개념과 직접 연결되며, 온디바이스 처리를 통한 프라이버시 보호라는 대안적 접근을 탐구한다. [[model-compression]]과 [[model-pruning]] 개념은 엣지 배포를 위한 모델 경량화 기법으로서 본 논문의 양자화 실험과 밀접하게 관련된다. 또한 [[hardware-aware-benchmarking]]의 관점에서 실제 하드웨어 제약을 고려한 벤치마킹 방법론을 공유하며, [[llm-benchmark]] 범주에서 추론 효율성 측면의 새로운 평가 차원을 추가한다. [[speculative-decoding]]과 같은 추론 가속 기법들이 엣지 환경에서 어떤 에너지-성능 프로필을 보이는지에 대한 후속 연구로 이어질 수 있다.

## 🔗 관련 논문

- Differential Privacy in Generative AI Agents: Analysis and O
- F2LLM-v2: Inclusive, Performant, and Efficient Embeddings fo
- SOL-ExecBench: Speed-of-Light Benchmarking for Real-World GP
- Nemotron-Cascade 2: Post-Training LLMs with Cascade RL and M
- Cram Less to Fit More: Training Data Pruning Improves Memori

## 🏷️ 엔티티

- [[entities/llm.md|LLM]]

## 📐 개념

- [[concepts/on-device-inference.md|on-device-inference]]
- [[concepts/model-compression.md|model-compression]]
- [[concepts/differential-privacy.md|differential-privacy]]
- [[concepts/hardware-aware-benchmarking.md|hardware-aware-benchmarking]]
- [[concepts/model-pruning.md|model-pruning]]
- [[concepts/llm-benchmark.md|llm-benchmark]]

---
_LLM 분석으로 재생성됨_
