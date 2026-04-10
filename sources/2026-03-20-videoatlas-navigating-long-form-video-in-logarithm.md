# VideoAtlas: Navigating Long-Form Video in Logarithmic Compute

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-20
**링크**: http://arxiv.org/abs/2603.17948v1

## 💡 핵심 인사이트

비디오를 계층적 그리드로 표현함으로써 캡션 변환 없이 무손실 시각 정보를 로그 복잡도로 탐색할 수 있어, 장시간 비디오 이해의 효율성과 충실도를 동시에 달성한다.

## 📖 분석

## VideoAtlas: Navigating Long-Form Video in Logarithmic Compute

**arXiv**: http://arxiv.org/abs/2603.17948v1  
**날짜**: 2026-03-20

### 개요

VideoAtlas는 장시간 비디오를 **계층적 그리드(hierarchical grid)** 로 표현하여, 손실 없이(lossless) 탐색 가능하고 확장 가능한 비디오 이해 환경을 제공하는 태스크-비종속(task-agnostic) 프레임워크다. 기존 비디오-언어 모델 파이프라인이 캡션 기반 또는 에이전트 기반으로 비디오를 텍스트로 압축하면서 시각적 충실도(visual fidelity)를 잃는 문제를 해결한다.

### 핵심 기여

- **로그 스케일 연산**: 비디오 길이에 대해 로그 복잡도로 탐색이 가능하도록 계층적 구조를 설계하여, 장시간 비디오에서도 효율적인 정보 접근을 실현한다.
- **무손실 표현**: 캡션이나 전처리 없이 비디오 원본의 시각 정보를 보존하면서도 구조화된 탐색이 가능하다.
- **에이전트 기반 내비게이션과의 차별화**: 기존 에이전트 파이프라인이 텍스트 변환 과정에서 정보를 잃는 반면, VideoAtlas는 시각 정보를 직접 계층적으로 조직화한다.

### 기존 연구와의 관계

이 연구는 [[LLM Agent]] 기반 비디오 이해 접근법의 한계를 지적하며 대안을 제시한다는 점에서, 에이전트 시스템의 시각 정보 처리 능력에 대한 논의와 연결된다. 또한 [[Transformer]] 아키텍처 위에서 멀티모달 입력을 효율적으로 처리하는 방법론으로, 장문맥(long-context) 처리 연구(예: TriAttention의 효율적 장문 추론)와도 맥을 같이 한다. CADENCE(깊이 추정을 위한 컨텍스트 적응)처럼 시각 정보의 구조적 표현을 활용하는 연구와도 접점이 있다.

## 🔗 관련 논문

- 2026 04 08 triattention efficient long reasoning with trigono
- 2026 04 10 cadence context adaptive depth estimation for navi
- 2026 04 09 mmemb r1 reasoning enhanced multimodal embedding w

## 🏷️ 엔티티

- [[entities/llm-agent.md|LLM Agent]]
- [[entities/transformer.md|Transformer]]

## 📐 개념

- [[concepts/video-understanding.md|video-understanding]]
- [[concepts/long-context.md|long-context]]
- [[concepts/hierarchical-representation.md|hierarchical-representation]]

---
_LLM 분석으로 재생성됨_
