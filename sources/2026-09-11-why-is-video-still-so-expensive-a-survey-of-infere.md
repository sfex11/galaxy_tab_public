# Why Is Video Still So Expensive? A Survey of Inference-Efficiency Mechanisms in Video and Audiovisual LLMs

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-11
**링크**: http://arxiv.org/abs/2609.10355v1

## 💡 핵심 인사이트

비디오 LLM의 비용 문제는 모델 크기가 아닌 프레임 수·컨텍스트 길이에 대한 입력 스케일링 문제이며, 시간적 중복성 활용(토큰 프루닝·KV 재사용·적응적 추론)이 비용과 성능을 동시에 개선하는 통합 해법이다.

## 📖 분석

비디오·오디오비주얼 LLM(VideoLLM)의 추론 효율화 메커니즘을 체계적으로 정리한 종합 서베이. VideoLLM이 캡셔닝·질의응답·검색·시간적 그라운딩에서 강력한 성능을 내지만, 계산·메모리 비용이 프레임 수와 컨텍스트 길이에 스케일링되어 실시간·모바일·자원제약 배포가 막히는 구조를 규정하고 해법 메커니즘을 분류한다.

**기존 Wiki와의 관계**: 본 서베이는 비디오 도메인에 흩어져 있던 효율화 연구들([[token-pruning]], [[text-guided-vision-token-selection]], [[vision-token-kv-cache-redundancy]], [[inter-position-redundancy]])을 하나의 추론 효율 스펙트럼으로 통합하는 좌표를 제공한다. [[shallow-index-deep-answer]](ShallowStream)의 지연 실행이 이 스펙트럼의 스트리밍 극점에 위치함을 확인하고, [[streaming-adaptive-inference]]와 [[adaptive-inference]]의 적응 축을 프레임 수·컨텍스트 길이·태스크 복잡도로 확장한다.

**핵심 인사이트**: (1) 비디오의 비용 문제는 모델 크기가 아닌 입력 스케일링 문제다 — 프레임 수가 곧 컨텍스트 길이이므로 frame-count-cost-scaling이라는 독립 축이 필요하다. (2) temporal redundancy(인접 프레임 간 중복)가 효율화의 핵심 기회이며, 토큰 프루닝과 KV 캐시 재사용은 모두 이 중복성의 활용이다. (3) [[perception-cognitive-capacity-mismatch]]의 효율성 측 재해석: 프레임 수 증가는 관찰 충실도와 비용을 동시에 올리되 성능은 역설적으로 저하시킬 수 있어, '적게 보기'가 성능·비용 양축의 해법이 된다. (4) [[on-device-inference]] 제약이 효율화 연구의 직접적 동기다.

**연결점**: 비디오는 [[long-context]] 스케일링의 최대 부하 도메인이며, [[modality-asymmetric-memory-cost]](시각 토큰의 KV 비용 지배)가 극대화되는 곳이다. [[model-compression]]·[[speculative-decoding]] 등 디코딩 가속은 아키텍처 최적화와 상보적 축을 형성한다.

## 🔗 관련 논문

- ShallowStream: Index Shallow then Answer Deep for Streaming Video Understanding
- Seeing Before Synthesizing: VLM-Guided Transition Event Discovery for Weakly-Supervised Dense Video Captioning
- Make Your LVLM KV Cache More Lightweight

## 🏷️ 엔티티

- [[entities/mllm.md|mllm]]
- [[entities/vlm.md|vlm]]
- [[entities/video-inference-efficiency.md|video-inference-efficiency]]

## 📐 개념

- [[concepts/token-pruning.md|token-pruning]]
- [[concepts/kv-cache-optimization.md|kv-cache-optimization]]
- [[concepts/adaptive-inference.md|adaptive-inference]]
- [[concepts/streaming-adaptive-inference.md|streaming-adaptive-inference]]
- [[concepts/on-device-inference.md|on-device-inference]]
- [[concepts/long-context.md|long-context]]
- [[concepts/video-understanding.md|video-understanding]]
- [[concepts/video-vlm.md|video-vlm]]
- [[concepts/text-guided-vision-token-selection.md|text-guided-vision-token-selection]]
- [[concepts/shallow-index-deep-answer.md|shallow-index-deep-answer]]
- [[concepts/perception-cognitive-capacity-mismatch.md|perception-cognitive-capacity-mismatch]]
- [[concepts/modality-asymmetric-memory-cost.md|modality-asymmetric-memory-cost]]
- [[concepts/inter-position-redundancy.md|inter-position-redundancy]]
- [[concepts/vision-token-kv-cache-redundancy.md|vision-token-kv-cache-redundancy]]
- [[concepts/model-compression.md|model-compression]]
- [[concepts/speculative-decoding.md|speculative-decoding]]

---
_LLM 분석으로 생성됨_
