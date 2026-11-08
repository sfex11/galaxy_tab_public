# Scientist World: Grow a Research World for AI-Scientists

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-07
**링크**: http://arxiv.org/abs/2611.08478v1

## 💡 핵심 인사이트

과학 문헌은 AI-Scientist에게 readable-but-not-runnable이며, 논문을 개방형 연구 질문 + 재현 베이스라인의 실행 가능 환경으로 재질의하는 것이 AI 과학 능력 성장의 인프라적 전제조건이다.

## 📖 분석

AI-Scientist가 도래했지만 그가 자랄 세계는 존재하지 않는다는 진단에서 출발한다. 인간 과학자는 문헌에 수세기 축적된 개방형 문제와 공유 아이디어를 당연한 자원으로 활용하지만, AI에게 과학 문헌은 'readable but not runnable' — 읽을 수 있으나 실행 가능한 연구 환경이 아니다. Scientist World는 자율 파이프라인으로 각 논문을 개방형 연구 질문과 재현된 베이스라인 메서드를 갖는 실행 가능 환경으로 변환하여 이 간극을 메운다.

이는 '기존 자료 → 환경' 전환 패턴의 문헌 버전이다. CodeMidas([[concepts/codebase-as-learning-environment.md|codebase as learning environment]])가 코드를, Terminal-Universe([[entities/terminal-universe.md|terminal universe]])가 궤적을 환경으로 재질의했다면, 본 논문은 과학 문헌 자체를 환경화하여 환경 원료의 스펙트럼을 인류의 지식 기록까지 확장한다. ScienceIDE([[entities/scienceide.md|scienceide]])가 과학 코드베이스를 학습 환경으로 삼았다면, 본 논문은 코드 이전의 지식 원천인 논문을 대상으로 상위 계층을 형성한다.

개방형 연구 질문의 추출은 [[concepts/unguided-scientific-discovery.md|unguided scientific discovery]]가 요구하는 목표 형성 능력을 문헌에서 공급하는 경로이고, 베이스라인 재현은 환경의 검증 기반([[concepts/execution-verification.md|execution verification]])을 접지한다. [[concepts/scientific-experience-bottleneck.md|scientific experience bottleneck]]의 해법이기도 하다 — 경험 희소성의 병인이 문헌 부족이 아니라 문헌의 실행 불가능성임을 규명하고 [[concepts/agent-environment-generation.md|agent environment generation]]의 원료 클래스에 문헌을 추가한다. AI-Scientist가 세계에서 자라난다는 구조는 [[concepts/self-improving-agent.md|self improving agent]]의 환경 자율성 축에 대규모 실현 경로를 제공하며, 문헌의 개방형 문제가 곧 연구 커리큘럼([[concepts/implicit-curriculum.md|implicit curriculum]])으로 실현된다.

## 🔗 관련 논문

- Terminal-Universe: Turning Agent Trajectories into Scalable Terminal Environments
- ScienceIDE: Turning World's Scientific Codebase into Agent Learning Environments

## 🏷️ 엔티티

- [[entities/scientist-world.md|scientist-world]]
- [[entities/autoresearch.md|autoresearch]]
- [[entities/scienceide.md|scienceide]]
- [[entities/codebase-as-learning-environment.md|codebase-as-learning-environment]]
- [[entities/terminal-universe.md|terminal-universe]]
- [[entities/agent-environment-generation.md|agent-environment-generation]]
- [[entities/environment-as-training-primitive.md|environment-as-training-primitive]]
- [[entities/unguided-scientific-discovery.md|unguided-scientific-discovery]]
- [[entities/scientific-experience-bottleneck.md|scientific-experience-bottleneck]]
- [[entities/executable-benchmark.md|executable-benchmark]]
- [[entities/self-improving-agent.md|self-improving-agent]]
- [[entities/implicit-curriculum.md|implicit-curriculum]]

## 📐 개념

- [[concepts/readable-but-not-runnable.md|readable-but-not-runnable]]
- [[concepts/paper-as-executable-environment.md|paper-as-executable-environment]]

---
_LLM 분석으로 생성됨_
