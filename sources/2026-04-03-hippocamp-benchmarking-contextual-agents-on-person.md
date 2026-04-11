# HippoCamp: Benchmarking Contextual Agents on Personal Computers

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-03
**링크**: http://arxiv.org/abs/2604.01221v1

## 💡 핵심 인사이트

HippoCamp는 웹이 아닌 로컬 파일 시스템에서 사용자 맥락을 이해하는 에이전트 능력을 평가함으로써, 기존 온라인 중심 벤치마크의 사각지대를 보완하는 개인화 에이전트 벤치마크다.

## 📖 분석

## HippoCamp: 개인 컴퓨터 맥락 인식 에이전트 벤치마크

HippoCamp는 멀티모달 파일 관리 능력을 평가하기 위한 새로운 벤치마크로, 기존의 웹 상호작용이나 도구 사용 중심 벤치마크와 차별화된다. 핵심 특징은 **사용자 중심 환경(user-centric environment)**을 모델링하여 개별 사용자 프로필을 반영하고, 대규모 개인 파일 시스템에서 맥락 인식 추론(context-aware reasoning)을 수행하는 능력을 측정한다는 점이다.

이 벤치마크는 실제 사용자 프로필 기반의 디바이스 규모 파일 시스템을 구축하며, 다양한 모달리티(문서, 이미지, 코드 등)에 걸친 파일 탐색과 추론을 요구한다. 이는 단순한 도구 호출이나 웹 탐색을 넘어, 에이전트가 사용자의 개인적 맥락을 이해하고 방대한 파일 속에서 관련 정보를 찾아내는 **개인화된 검색 및 추론 능력**을 평가한다.

기존 웹 에이전트 벤치마크([[ClawBench]], [[Vision2Web]] 등)가 온라인 태스크 완수에 집중하는 반면, HippoCamp는 로컬 파일 시스템이라는 오프라인 환경에서의 에이전트 능력을 측정한다. 이는 [[PSI: Shared State as the Missing Layer for Coherent AI-Gener|PSI]]가 제안한 개인 AI 에이전트의 공유 상태 관리 문제와도 맞닿아 있다—에이전트가 사용자의 파일과 맥락을 효과적으로 관리하려면 지속적인 상태 추적이 필수적이기 때문이다. 또한 [[TraceSafe]]의 에이전트 가드레일 평가와 보완적 관계를 형성하며, 파일 시스템 접근이라는 민감한 영역에서의 안전성 문제를 환기한다.

## 🔗 관련 논문

- PSI: Shared State as the Missing Layer for Coherent AI-Gener
- TraceSafe: A Systematic Assessment of LLM Guardrails on Mult
- ClawBench: Can AI Agents Complete Everyday Online Tasks?
- Act Wisely: Cultivating Meta-Cognitive Tool Use in Agentic M

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/web-agent-evaluation.md|web-agent-evaluation]]
- [[concepts/personal-ai-agent.md|personal-ai-agent]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/multimodal-learning.md|multimodal-learning]]
- [[concepts/ai-safety.md|ai-safety]]

---
_LLM 분석으로 재생성됨_
