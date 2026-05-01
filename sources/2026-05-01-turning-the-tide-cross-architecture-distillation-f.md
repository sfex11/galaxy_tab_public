# Turning the TIDE: Cross-Architecture Distillation for Diffusion Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-01
**링크**: http://arxiv.org/abs/2604.26951v1

## 💡 핵심 인사이트

지식 증류의 근본적 전제인 '교사-학생 간 표현 공간의 호환성'을 해체함으로써, 모델 압축이 '작아지기'가 아닌 '다른 패러다임으로 번역되기'로 재정의된다.

## 📖 분석

# Turning the TIDE: Cross-Architecture Distillation for Diffusion LLMs

## 정의
TIDE는 확산 대형 언어 모델(dLLM) 간 cross-architecture 지식 증류를 최초로 달성한 프레임워크다. 기존 dLLM 증류가 단일 아키텍처 내에서 추론 스텝 수만 줄이는 방식에 머물렀던 것과 달리, TIDE는 교사와 학생이 아키텍처·어텐션 메커니즘·토크나이저까지 상이한 상황에서의 지식 전이를 가능하게 한다.

## 기존 Wiki와의 관계

### knowledge-distillation의 범위 확장
기존 Wiki에서 knowledge-distillation은 주로 동일 아키텍처 내의 파라미터 축소(Nemotron-Cascade 2의 OPD, F2LLM-v2 등)로 기술되어 있었다. TIDE는 이 엔티티에 '아키텍처 경계를 넘는 지식 전이'라는 새로운 차원을 추가한다. 교사-학생이 서로 다른 계산 패러다임(자회귀 vs 확산, 단방향 vs 양방향 어텐션)을 사용할 때 지식이 어떻게 번역되어야 하는지라는 근본적 질문을 제기한다.

### model-compression의 전략적 다변화
[[entities/carbon-taxed-compression|Carbon-Taxed Transformers]](2026-04-30)가 동일 아키텍처 내에서 탄소 비용을 최적화 변수로 삼은 압축 파이프라인이라면, TIDE는 압축의 차원 자체를 변경한다 — 파라미터 수 축소가 아닌 아키텍처 패러다임 전환을 통해 효율성을 확보한다. 두 논문은 "효율적 모델"이라는 목표에 대해 상보적 경로를 제공한다.

### diffusion-model의 언어 모델로의 확장
기존 Wiki에서 diffusion-model은 주로 이미지·비디오 생성(VectorWorld, ActionParty 등)에 한정되어 기술되었다. TIDE는 확산 패러다임이 언어 모델링에서도 경쟁력을 가질 수 있음을 보여주며, diffusion-model 엔티티를 시각 생성에서 언어 추론으로 확장하는 근거를 제공한다.

## 핵심 기여
단일 아키텍처 내 증류가 암묵적으로 전제하던 '동일 표현 공간' 가정을 해체하고, 토크나이저 불일치까지 포함한 완전한 cross-architecture 증류를 형식화한 점이 가장 중요하다. 이는 knowledge-distillation 연구가 '얼마나 작게 만들까'에서 '어떻게 다른 패러다임으로 번역할까'로 질문을 전환시킨다.

## 🔗 관련 논문

- 2026 04 30 carbon taxed transformers a green compression pipe
- 2026 03 23 nemotron cascade 2 post training llms with cascade
- 2026 03 21 f2llm v2 inclusive performant and efficient embedd
- 2026 04 30 pythia toward predictability driven agent native l

## 🏷️ 엔티티

- [[entities/knowledge-distillation.md|knowledge-distillation]]
- [[entities/model-compression.md|model-compression]]
- [[entities/diffusion-llm.md|diffusion-llm]]
- [[entities/cross-architecture-distillation.md|cross-architecture-distillation]]
- [[entities/diffusion-model.md|diffusion-model]]
- [[entities/parallel-decoding.md|parallel-decoding]]
- [[entities/carbon-taxed-compression.md|carbon-taxed-compression]]

## 📐 개념

- [[concepts/cross-architecture-distillation.md|cross-architecture-distillation]]
- [[concepts/diffusion-llm.md|diffusion-llm]]
- [[concepts/parallel-decoding.md|parallel-decoding]]
- [[concepts/tokenizer-alignment.md|tokenizer-alignment]]
- [[concepts/bidirectional-context-modeling.md|bidirectional-context-modeling]]
- [[concepts/representation-space-translation.md|representation-space-translation]]

---
_LLM 분석으로 생성됨_
