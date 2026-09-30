# Skill-Space Shooting for Autonomous Robot Policy Improvement

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-01
**링크**: http://arxiv.org/abs/2609.38178v1

## 💡 핵심 인사이트

에이전틱 스킬 조합에 의한 과제 완수는 그 자체로 학습이 아니므로, 조합 탐색의 경험을 기저 정책 개선 신호로 명시적으로 환류해야만 인간 시연 없이 확장 가능한 자율 로봇 개선이 성립한다.

## 📖 분석

# Skill-Space Shooting for Autonomous Robot Policy Improvement

**arXiv**: http://arxiv.org/abs/2609.38178v1 | **발행일**: 2026-10-01

## 핵심 주장

물리 세계에 배포된 로봇은 초기 훈련 이후 새로운 상황과 실패에서 개선해야 하며, 이 개선이 과제 전반으로 확장되려면 매 수정마다 인간 시연을 요구할 수 없다. 본 논문은 파운데이션 모델이 학습된 스킬을 자율적으로 조합해 과제를 완수하는 에이전틱 시스템을 출발점으로 삼되, 결정적 통찰로 **'조합에 의한 과제 완수는 그 자체로 학습이 아니다'**를 제시하고, 스킬 공간 위의 탐색(shooting) 결과를 기저 정책 개선 신호로 환류하는 프레임워크를 제안한다.

## Wiki에서의 위치

### RAPID와의 축 분화
rapid가 시연을 테스트 가능 명세로 컴파일해 시연 부담을 해소했다면, 본 논문은 새 시연 없이 기존 스킬의 조합 경험에서 개선을 얻어 **개선의 확장성**이라는 제2 축을 연다. TANDEM이 필요 시점에 시연을 요청했다면 본 논문은 수정 시 시연 자체를 제거한다.

### Learning to Coach 계열과의 연결
[[trajectory-as-coaching-signal]] 패턴의 로봇 도메인 실현이다. 파운데이션 모델이 llm-as-coach 역할로 스킬 조합을 수행하되 그 결과가 정책 가중치로 환류되어, improvement-delegation과 자기 개선의 하이브리드 형태가 된다.

### 학습 단위의 재정의
조합-실행-관찰-개선 루프의 반복이 학습 단위로 기능한다는 [[agent-loop-as-training-time]] 원리의 물리 도메인 실증.

### 외부 스킬 vs 내부 정책의 긴장
[[skill-as-external-state]]와 capability-internalization의 교차점. 조합 완수가 정책에 자동 흡수되지 않음을 근거로, 개선의 저장 위치(외부 스킬 라이브러리 vs 정책 파라미터)를 가르는 명시적 환류 메커니즘의 필요성을 확립한다.

## 🔗 관련 논문

- RAPID: Robot Agentic Programming from Demonstrations
- SkillOS: Learning Skill Curation for Self-Evolving Agents
- Learning to Coach for Experiential Learning
- TANDEM: Task and Motion Planning with As-Needed Demonstrations

## 🏷️ 엔티티

- [[entities/skill-space-shooting.md|skill-space-shooting]]
- [[entities/rapid.md|rapid]]
- [[entities/agent-loop-as-training-time.md|agent-loop-as-training-time]]
- [[entities/skill-as-external-state.md|skill-as-external-state]]
- [[entities/capability-internalization.md|capability-internalization]]
- [[entities/trajectory-as-coaching-signal.md|trajectory-as-coaching-signal]]
- [[entities/llm-as-coach.md|llm-as-coach]]
- [[entities/improvement-delegation.md|improvement-delegation]]
- [[entities/demonstration-burden-automation.md|demonstration-burden-automation]]
- [[entities/experience-generation.md|experience-generation]]
- [[entities/validated-skill-library.md|validated-skill-library]]
- [[entities/harness-methodology-embodiment-migration.md|harness-methodology-embodiment-migration]]

## 📐 개념

- [[concepts/skill-space-shooting.md|skill-space-shooting]]
- [[concepts/completion-learning-separation.md|completion-learning-separation]]
- [[concepts/agent-loop-as-training-time.md|agent-loop-as-training-time]]
- [[concepts/capability-internalization.md|capability-internalization]]
- [[concepts/skill-as-external-state.md|skill-as-external-state]]

---
_LLM 분석으로 생성됨_
