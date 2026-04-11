# DIRECT: Video Mashup Creation via Hierarchical Multi-Agent Planning and Intent-Guided Editing

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-08
**링크**: http://arxiv.org/abs/2604.04875v1

## 💡 핵심 인사이트

비디오 매시업이라는 창작 도메인에서 계층적 멀티에이전트 플래닝을 통해 시맨틱-비주얼-오디오 간 크로스 레벨 멀티모달 오케스트레이션을 달성한 최초의 체계적 프레임워크이다.

## 📖 분석

## DIRECT: Video Mashup Creation via Hierarchical Multi-Agent Planning and Intent-Guided Editing

**분류**: 멀티에이전트 시스템, 비디오 편집, 멀티모달 오케스트레이션

### 핵심 내용

DIRECT는 비디오 매시업(mashup) 제작을 위한 계층적 멀티에이전트 플래닝 및 의도 기반 편집 프레임워크이다. 비디오 매시업은 기존 영상 소스를 재구성하여 시각-청각적으로 몰입감 있는 경험을 만드는 복잡한 편집 패러다임으로, 의미적(semantic), 시각적(visual), 청각적(auditory) 차원을 아우르는 다층적 조율이 필요하다.

기존 자동 편집 프레임워크들은 이러한 크로스 레벨 멀티모달 오케스트레이션을 간과하여, 급작스러운 시각 전환이나 음악 불일치 등 부자연스러운 결과를 초래했다. DIRECT는 이를 해결하기 위해 **계층적 멀티에이전트 구조**를 도입한다. 각 에이전트가 서로 다른 수준(시맨틱 플래닝, 비주얼 전환, 오디오 정렬 등)의 편집 결정을 담당하며, 의도(intent) 기반 가이드를 통해 전체적인 일관성을 유지한다.

### 연구 맥락

이 연구는 멀티에이전트 시스템의 **작업 분해 및 계층적 협업** 패러다임을 비디오 편집 도메인에 적용한 사례로, LLM 기반 에이전트들이 창작 도구로서 기능하는 흐름과 맞닿아 있다. 특히 멀티모달 정렬(visual-auditory alignment)이라는 도전 과제는 기존 VLM/MLLM 연구의 확장선상에 있으며, 에이전트 간 공유 상태 관리([[PSI]])나 계층적 표현([[VideoAtlas]])과도 관련된다. 또한 에이전트의 의도 기반 편집은 choice-architecture 및 AI 의사결정 연구와 개념적으로 연결된다.

## 🔗 관련 논문

- 2026 04 09 paper circle an open source multi agent research d
- 2026 04 11 psi shared state as the missing layer for coherent
- 2026 04 11 figures as interfaces toward llm native artifacts
- 2026 04 11 act wisely cultivating meta cognitive tool use in

## 📐 개념

- [[concepts/video-mashup.md|video-mashup]]
- [[concepts/hierarchical-planning.md|hierarchical-planning]]
- [[concepts/multimodal-orchestration.md|multimodal-orchestration]]
- [[concepts/intent-guided-editing.md|intent-guided-editing]]

---
_LLM 분석으로 재생성됨_
