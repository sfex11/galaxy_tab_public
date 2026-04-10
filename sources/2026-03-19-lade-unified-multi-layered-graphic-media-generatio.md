# LaDe: Unified Multi-Layered Graphic Media Generation and Decomposition

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-19
**링크**: http://arxiv.org/abs/2603.17965v1

## 💡 핵심 인사이트

텍스트-이미지 생성을 단일 이미지에서 편집 가능한 다층 디자인 문서로 확장하여, 고정 레이어 수 제약 없이 의미 기반 레이어를 유연하게 생성·분해하는 통합 diffusion 프레임워크를 제시했다.

## 📖 분석

## LaDe: Unified Multi-Layered Graphic Media Generation and Decomposition

**분류**: 생성 모델 / 그래픽 디자인 자동화

### 개요
LaDe(Layered Media Design)는 자연어 프롬프트만으로 포스터, 전단지, 로고 등 완전히 편집 가능한 다층 디자인 문서를 생성하는 latent diffusion 프레임워크이다. 기존 방법들은 고정된 레이어 수로 출력을 제한하거나, 각 레이어가 공간적으로 연속된 영역만 포함하도록 강제하여 디자인 복잡도에 따라 레이어 수가 선형적으로 증가하는 한계가 있었다. LaDe는 의미적으로 유의미한 레이어를 유연한 수만큼 생성할 수 있어 이 문제를 해결한다.

### 핵심 기여
- **유연한 레이어 생성**: 고정 레이어 수 제약 없이 디자인 복잡도에 적응적으로 레이어를 구성
- **의미 기반 분해**: 단순 공간 분할이 아닌 의미적 단위로 레이어를 분리하여 편집 용이성 극대화
- **통합 프레임워크**: 생성(generation)과 분해(decomposition)를 하나의 latent diffusion 모델로 통합
- **텍스트 기반 제어**: 자연어 프롬프트를 통한 직관적 디자인 생성 지원

### 기존 연구와의 관계
본 연구는 text-to-image 생성 패러다임을 단일 이미지 출력에서 편집 가능한 다층 미디어 문서로 확장한다. 기존 Wiki의 [[text-to-image]] 개념과 직접적으로 연관되며, diffusion 모델 기반 생성이라는 점에서 생성 모델 연구의 응용 범위를 그래픽 디자인 영역으로 넓힌 사례이다. 또한 자연어 프롬프트로 복잡한 구조적 출력을 제어한다는 점에서 [[prompt-engineering]] 개념과도 연결된다.

## 📐 개념

- [[concepts/text-to-image.md|text-to-image]]
- [[concepts/prompt-engineering.md|prompt-engineering]]

---
_LLM 분석으로 재생성됨_
