# VideoSeek: Long-Horizon Video Agent with Tool-Guided Seeking

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-24
**링크**: http://arxiv.org/abs/2603.20185v1

## 💡 핵심 인사이트

비디오 전체를 밀집 파싱하는 대신 논리 흐름 기반의 도구 호출로 핵심 프레임만 능동 탐색함으로써, 장시간 비디오 이해의 효율성과 정확도를 동시에 달성하는 에이전틱 접근법을 제시한다.

## 📖 분석

## VideoSeek: Long-Horizon Video Agent with Tool-Guided Seeking

**arXiv**: http://arxiv.org/abs/2603.20185v1
**날짜**: 2026-03-24

### 개요

VideoSeek는 장시간 비디오 이해를 위한 에이전트 모델로, 비디오 전체를 밀집 샘플링하여 탐욕적으로 파싱하는 기존 방식의 높은 계산 비용 문제를 해결한다. 핵심 아이디어는 **비디오 논리 흐름(video logic flow)**을 활용하여 답변에 필수적인 증거를 능동적으로 탐색(seek)하는 것이다. 이를 통해 훨씬 적은 프레임만으로 비디오 이해 성능을 유지하거나 오히려 향상시킨다.

### 기술적 특징

- **도구 기반 탐색(Tool-Guided Seeking)**: 에이전트가 비디오 내 특정 구간을 도구처럼 호출하여 필요한 시점의 프레임만 선택적으로 접근하는 메커니즘을 채택한다. 이는 LLM 에이전트의 도구 사용(tool-use) 패러다임을 비디오 이해에 적용한 사례이다.
- **장시간 비디오 처리**: 긴 비디오에서 전체 프레임을 처리하지 않고 논리적 흐름에 따라 핵심 증거를 추적하므로, 기존 밀집 샘플링 대비 계산 효율이 크게 개선된다.
- **에이전틱 비디오 모델**: 모델이 수동적으로 입력을 처리하는 것이 아니라, 능동적으로 정보를 탐색하는 에이전트 방식으로 동작한다.

### 기존 연구와의 관계

- **토큰 프루닝 및 효율적 비디오 처리**: 불필요한 프레임/토큰을 줄여 효율성을 높인다는 점에서 [[token-pruning]] 및 [[video-vlm]] 개념과 직접 연결된다. Unified Spatio-Temporal Token Scoring 연구가 토큰 수준의 효율화를 다뤘다면, VideoSeek는 프레임 수준에서 에이전틱 탐색으로 효율화를 달성한다.
- **도구 사용(tool-use)**: LLM 에이전트가 외부 도구를 활용하는 패러다임을 비디오 도메인에 확장한 것으로, [[tool-use]] 개념과 관련된다.
- **장시간 컨텍스트 처리**: VideoAtlas가 계층적 표현으로 장시간 비디오를 다뤘다면, VideoSeek는 능동적 탐색 전략으로 접근한다는 점에서 [[long-context]] 개념과 상호보완적이다.
- **LLM Agent**: 비디오 이해를 에이전트 프레임워크로 구성하여 [[llm-agent]] 엔티티와 연결된다.

## 🔗 관련 논문

- Unified Spatio-Temporal Token Scoring for Efficient Video VL
- VideoAtlas: Navigating Long-Form Video in Logarithmic Comput
- TraceSafe: A Systematic Assessment of LLM Guardrails on Mult
- AgentFactory: A Self-Evolving Framework Through Executable S

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/tool-use.md|tool-use]]
- [[concepts/video-understanding.md|video-understanding]]
- [[concepts/token-pruning.md|token-pruning]]
- [[concepts/long-context.md|long-context]]
- [[concepts/video-vlm.md|video-vlm]]

---
_LLM 분석으로 재생성됨_
