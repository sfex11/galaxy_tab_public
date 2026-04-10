# VideoAtlas: Navigating Long-Form Video in Logarithmic Compute

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-19
**링크**: http://arxiv.org/abs/2603.17948v1

## 💡 핵심 인사이트

비디오를 계층적 그리드로 표현함으로써 장시간 비디오 이해를 로그 스케일 연산으로 축소하고, 캡션 없이도 시각적 충실도를 보존하는 무손실 탐색이 가능하다.

## 📖 분석

## VideoAtlas: Navigating Long-Form Video in Logarithmic Compute

**arXiv**: http://arxiv.org/abs/2603.17948v1 | **날짜**: 2026-03-19

### 개요

VideoAtlas는 장시간 비디오를 언어 모델에 효율적으로 입력하기 위한 **태스크-비의존적(task-agnostic) 비디오 표현 환경**이다. 기존 비디오-LLM 파이프라인의 두 가지 핵심 문제를 동시에 해결한다: (1) 손실 압축(lossy approximation)에 의존하는 **표현(representation)** 문제, (2) 캡션이나 에이전트 기반 파이프라인이 비디오를 텍스트로 붕괴시켜 시각적 충실도를 잃는 **장문맥(long-context)** 문제.

### 핵심 기법

VideoAtlas는 비디오를 **계층적 그리드(hierarchical grid)**로 변환하여 무손실(lossless), 탐색 가능(navigable), 확장 가능(scalable)하며 캡션이나 전처리가 불필요한 표현을 제공한다. 이 계층 구조 덕분에 전체 비디오 개요를 한눈에 파악할 수 있으며, 필요한 부분만 선택적으로 탐색하는 **로그 스케일 연산(logarithmic compute)**이 가능하다. 이는 비디오 길이에 대해 선형이 아닌 로그 복잡도로 처리할 수 있음을 의미한다.

### 의의 및 연결점

이 연구는 멀티모달 LLM의 비디오 이해 능력을 근본적으로 개선하려는 시도로, 기존의 캡션 기반 접근법이나 에이전트 기반 비디오 탐색과 차별화된다. **LLM Agent** 기반 비디오 분석 파이프라인에서 VideoAtlas를 환경으로 활용하면, 에이전트가 전체 비디오를 처리하지 않고도 계층적으로 필요한 정보에 접근할 수 있다. 또한 Transformer 아키텍처의 장문맥 처리 한계를 우회하는 실용적 전략으로, 긴 시퀀스를 공간적 계층 구조로 재구성하는 아이디어가 주목할 만하다.

## 🔗 관련 논문

- 2026 04 09 maestro adapting guis and guiding navigation with
- 2026 04 08 triattention efficient long reasoning with trigono

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/multi-modal-learning.md|multi-modal-learning]]
- [[concepts/long-context.md|long-context]]

---
_LLM 분석으로 재생성됨_
