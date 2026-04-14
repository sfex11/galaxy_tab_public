# ClawBench: Can AI Agents Complete Everyday Online Tasks?

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-13
**링크**: http://arxiv.org/abs/2604.08523v1

## 💡 핵심 인사이트

144개 라이브 플랫폼에서 153개 일상 태스크를 평가함으로써, 현재 AI 에이전트가 시뮬레이션 환경과 달리 실제 웹 서비스에서 일상 자동화를 수행하는 데 여전히 큰 격차가 있음을 정량적으로 보여준다.

## 📖 분석

## ClawBench: 일상 온라인 태스크 자동화를 위한 AI 에이전트 벤치마크

ClawBench는 144개 라이브 플랫폼에 걸쳐 15개 카테고리의 153개 일상 태스크(구매, 예약, 구직 지원 등)를 평가하는 프레임워크이다. 기존 웹 에이전트 벤치마크가 시뮬레이션 환경이나 제한된 도메인에 집중한 것과 달리, ClawBench는 **실제 라이브 웹사이트**에서의 end-to-end 태스크 완수를 측정한다는 점에서 차별화된다.

### 기존 Wiki와의 관계
- [[web-agent-evaluation]]: ClawBench는 이 개념의 핵심 사례로, Vision2Web이나 UI-Voyager 같은 기존 벤치마크가 GUI 인터랙션 수준에 머문 반면, 태스크 완료의 실용적 성공률을 측정
- [[computer-use-agent]]: 에이전트가 브라우저를 조작하여 실제 서비스를 이용하는 시나리오로, human oversight 전략 연구와 직결
- [[llm-agent]]: 범용 에이전트의 실세계 능력 한계를 정량적으로 드러냄
- [[closed-loop-evaluation]]: 라이브 환경 특성상 동적 웹페이지 변화에 대응하는 closed-loop 평가가 필수

### 핵심 기여
1. 15개 카테고리 분류 체계로 일상 태스크의 다양성을 체계화
2. 라이브 플랫폼 기반 평가로 시뮬레이션-실세계 간 generalization gap 직접 측정
3. 현재 AI 에이전트의 일상 자동화 능력의 실질적 상한선 제시

### 연결 논문
- Act Wisely(메타인지 도구 사용)와 결합 시, 에이전트의 태스크 실패 원인 진단에 활용 가능
- Android Coach(온라인 에이전트 훈련)의 평가 기준으로 ClawBench 채택 가능성

## 🔗 관련 논문

- 2026 04 11 clawbench can ai agents complete everyday online t
- 2026 04 12 clawbench can ai agents complete everyday online t
- 2026 04 12 act wisely cultivating meta cognitive tool use in
- 2026 04 11 act wisely cultivating meta cognitive tool use in
- 2026 04 11 figures as interfaces toward llm native artifacts

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/web-agent-evaluation.md|web-agent-evaluation]]
- [[concepts/computer-use-agent.md|computer-use-agent]]
- [[concepts/closed-loop-evaluation.md|closed-loop-evaluation]]
- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/generalization-gap.md|generalization-gap]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-04-14-agentic-jackal-live-execution-and-semantic-value-g]]: 둘 다 실제 라이브 환경에서의 AI 에이전트 태스크 수행을 다루며, 전자는 웹 태스크 벤치마크를, 후자는 Jira 실시간 쿼리 에이전트를 제안한다.
