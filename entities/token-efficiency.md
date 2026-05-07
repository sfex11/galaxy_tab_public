# token-efficiency

**카테고리**: 미분류
**생성일**: 2026-04-25

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-04-25-tool-attention-is-all-you-need-dynamic-tool-gating.md|Tool Attention Is All You Need: Dynamic Tool Gating and Lazy]]

### Tool Attention Is All You Need: Dynamic Tool Gating and Lazy Schema Lo (2026-04-26)

도구 스키마 압축을 넘어 스키마 로딩 자체를 지연시키는 접근법을 제시하여, 토큰 효율화의 범위를 '주어진 컨텍스트의 압축'에서 '불필요한 컨텍스트의 원천 차단'으로 확장한다.

### Pythia: Toward Predictability-Driven Agent-Native LLM Serving (2026-04-30)

시맨틱 예측가능성을 토큰 효율화의 상류 원천으로 위치시킨다 — Tool Attention이 스키마 로딩을 지연시키는 후처리적 접근이라면, Pythia는 토폴로지 구조 자체에서 불필요한 토큰 생성을 선제적으로 차단하는 구조적 접근이다.

### Agentic Harness Engineering: Observability-Driven Automatic Evolution  (2026-04-30)

백만 토큰 규모의 궤적에서 하네스 수준의 낭비를 구조적으로 식별·제거하는 상류 최적화 경로를 제공하여, 기존 스키마 로딩 지연(Tool Attention)과 결합하면 토큰 효율화의 스펙트럼을 컨텍스트 압축→컨텍스트 차단→하네스 최적화로 3층으로 확장한다.

### Carbon-Taxed Transformers: A Green Compression Pipeline for Overgrown  (2026-04-30)

토큰 효율화의 정당성 근거를 비용 절감에서 탄소 배출 감축으로 확장하여, 효율화가 단순한 엔지니어링 최적화가 아닌 환경적 책임의 실행 수단임을 위치시킨다.

### Unifying Sparse Attention with Hierarchical Memory for Scalable Long-C (2026-05-01)

불필요한 컨텍스트 주입 차단(Tool Attention)에서 불필요한 KV 엔트리 접근 차단(희소 어텐션 통합)으로 효율화의 대상을 컨텍스트 입력층에서 메모리 접근층으로 확장한다.

### Reliable Answers for Recurring Questions: Boosting Text-to-SQL Accurac (2026-05-02)

토큰 선택 수준(SLM에서의 local sufficiency)을 넘어 템플릿 수준에서 디코딩 탐색 공간을 구조적으로 축소하는 상위 최적화 차원을 제공한다.

### Position-Aware Drafting for Inference Acceleration in LLM-Based Genera (2026-05-02)

컨텍스트 단위의 토큰 절약(Tool Attention)과 병렬로, 디코딩 단계 자체를 건너뛰어 토큰 생성 레이턴시를 줄이는 추론 수준의 토큰 효율화 경로를 추가하여, 토큰 효율화가 '입력 최소화'와 '생성 가속' 두 축으로 분화됨을 보여준다.

### Make Your LVLM KV Cache More Lightweight (2026-05-05)

토큰 효율화의 범위를 '주어진 컨텍스트의 압축'과 '불필요한 컨텍스트의 원천 차단'에서 '프리필 단계에서의 시각 중복 제거'로 추가 확장한다.

→ [[sources/2026-05-05-make-your-lvlm-kv-cache-more-lightweight.md|상세 보기]]

### To Call or Not to Call: A Framework to Assess and Optimize LLM Tool Ca (2026-05-05)

→ [[sources/2026-05-05-to-call-or-not-to-call-a-framework-to-assess-and-o.md|상세 보기]]

### SpecKV: Adaptive Speculative Decoding with Compression-Aware Gamma Sel (2026-05-05)

토큰 효율화가 단순한 토큰 수 감소를 넘어, 토큰 생성의 병렬성 효율(γ 수용률) 자체를 최적화하는 차원을 추가한다. 동일한 토큰 수라도 γ 선택에 따라 실제 지연시간이 비선형적으로 변할 수 있음을 보여준다.

→ [[sources/2026-05-05-speckv-adaptive-speculative-decoding-with-compress.md|상세 보기]]

### LongSeeker: Elastic Context Orchestration for Long-Horizon Search Agen (2026-05-08)

토큰 효율화의 범위를 '주어진 컨텍스트 내 토큰 제거'(token-pruning)에서 '컨텍스트 구조 자체를 관련도에 따라 다층적으로 재구성'하는 수준으로 격상시킨다. 단순한 토큰 수 절감이 아닌, 정보의 의미론적 중요도에 비례한 예산 분배라는 원칙을 제공하여 기존의 양적 접근을 질적 접근으로 보완한다.

→ [[sources/2026-05-08-longseeker-elastic-context-orchestration-for-long-.md|상세 보기]]
