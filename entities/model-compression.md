# model-compression

**카테고리**: 미분류
**생성일**: 2026-04-30

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-04-30-carbon-taxed-transformers-a-green-compression-pipe.md|Carbon-Taxed Transformers: A Green Compression Pipeline for ]]

### Select to Think: Unlocking SLM Potential with Local Sufficiency (2026-05-01)

### Turning the TIDE: Cross-Architecture Distillation for Diffusion Large  (2026-05-01)

파라미터 수 축소나 양자화 같은 동일 아키텍처 내 최적화와 병렬적으로, 아키텍처 패러다임 자체를 전환(자회귀→확산 또는 그 역)하여 효율성을 확보하는 전략적 차원을 추가한다.

### Standing on the Shoulders of Giants: Stabilized Knowledge Distillation (2026-05-05)

동일 아키텍처 내 대형→소형 압축에서 '행동 안정성 보존'이라는 새로운 압축 축을 제시한다. 기존 탄소-정확도 트레이드오프나 아키텍처 전환과 병렬적으로, 도메인 특화 행동(출력 형식 준수, 프롬프트 따르기)을 압축 과정에서 명시적 목표로 삼아야 함을 실증한다.

### Measurement-Driven Sub-Network Selection for On-Premise Retrieval-Augm (2026-09-04)

압축의 효과가 일반 능력과 태스크 품질에서 비동질적으로 나타남을 실증한다 — 일반 능력은 파라미터 수에 선형 감소하지만 적응 후 RAG 품질은 그렇지 않아, 압축의 '품질 손실'이 태스크 의존적이며 크기 프록시로 사전 평가할 수 없음을 보여준다.

### Unfolding the Leech Lattice: Fused Multi-Shell Decoding and VRAM Layou (2026-09-04)

기존의 양자화 손상 구조 분석과 기하학적 보상(OrpQuant) 논의에 '이론적 최적 기법의 채택 병목'이라는 새 축을 추가한다. 파라미터 축소·증류·아키텍처 전환과 병렬적으로, 코드북 기반 격자 양자화가 커널 구현에 의해 실용성이 결정됨을 보여준다.

### Don't Drop Dropout: Optimizing Layer Sparsity for Efficient LLM Traini (2026-09-08)

기존 post-training 중심 압축(양자화·증류·프루닝) 분류에 '사전학습 시점에 프루닝 가능한 모델을 생성'하는 경로를 추가한다. Layer dropout 최적화는 훈련 시점 개입으로 압축이 사후 산출물이 아니라 모델에 내장된 속성임을 보여준다.

### The Weight Is Over - Interactive Diffusion on Consumer GPUs (2026-09-22)

생성 백본의 품질을 유지하면서 조건화 계층(거대 텍스트 인코더)을 소형 인코더+임베딩 번역기로 치환하는 선택적 풋프린트 절감 전략을 제공한다. 압축 대상이 전체 모델이 아니라 파이프라인 구성요소별 기여도에 따라 결정되어야 함을 보여준다.

### R-DEIM Net: An Efficient Rationale-Augmented Dual-Expert Interaction M (2026-09-26)

압축의 목표 축에 '설명 가능성 보존'을 추가한다. 파라미터 축소가 성능뿐 아니라 투명성을 함께 감소시키는 경향에 대해, 근거 생성 전문가를 유지하는 구조적 설계로 트레이드오프를 관리하는 사례를 제공한다.

### StrataFlux: Memory-Hierarchy-Native Low-Bit LLM Inference (2026-11-07)

압축의 정확도 비용이 영구적 손실이 아니라 '데이터가 어느 계층에 위치하는가'에 따라 스케줄 가능하고 회복 가능한 속성임을 보여준다. 압축과 오프로딩을 경쟁 전략이 아닌 단일 메모리 계층 설계의 상보적 층위로 재정의한다.

### LazyWeights: Decode-on-Demand Edge LLMs (2026-11-14)

손실 양자화와 무손실 엔트로피 코딩의 직교 합성이라는 제3 경로를 제공한다. 기존 논의가 양자화·프루닝·증류 같은 손실 기법의 단독 적용이었다면, 본 논문은 GPTQ의 코드 배치를 의도적으로 비균등하게 왜곡해 Huffman 압축률을 극대화하는 파이프라인 설계를 보여준다 — 압축의 두 축이 독립이 아니라 협력적으로 설계되어야 함을 실증한다.

→ [[sources/2026-11-14-lazyweights-decode-on-demand-edge-llms.md|상세 보기]]
