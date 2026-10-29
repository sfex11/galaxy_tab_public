# EnvSched: Environment-Aware Scheduling for Rollout-Efficient Agent Reinforcement Learning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-29
**링크**: http://arxiv.org/abs/2610.37609v1

## 💡 핵심 인사이트

환경이 태스크의 도구·상태·전이·검증을 결정하는 이상, 유한 롤아웃 예산 하 RL 효율의 마지막 지렛대는 정책 최적화가 아니라 '어떤 환경을 언제 실행할까'라는 환경 수준 데이터 관리다.

## 📖 분석

## 핵심 기여

EnvSched는 실행 가능 환경의 스케일 확대에 따라 롤아웃 생성·검증 비용이 병목이 되는 문제를 **환경 수준 데이터 관리**로 해결한다. 환경이 태스크의 도구·상태·전이·검증을 결정한다는 관찰 아래, 태스크 인스턴스를 환경과 함께 조직·평가·스케줄링하여 유한 롤아웃 예산 내 에이전틱 RL 효율을 높인다.

## 기존 Wiki와의 관계

- [[environment-as-training-primitive]]: 기존 흐름(Terminal-Universe의 궤적→환경, CodeMidas의 코드→환경, ScienceIDE)이 환경 **합성**에 집중했다면, 본 논문은 고정 환경 풀 위의 **스케줄링**이라는 제2 축을 연다. 환경이 훈련 원시자원이라면 원시자원의 소비 순서 관리도 훈련 효율의 대상이 된다.
- [[training-grade-serving-class]]·[[agent-native-serving]]: 추론 서빙 최적화(Pythia, TokenCast, EAServe)의 훈련 롤아웃 대응물로, 서빙 계층 최적화가 훈련 인프라로 확장되는 흐름의 훈련 측을 완성한다.
- [[rollout-budget-convergence-efficiency]]: 유한 예산 하 수렴 효율을 환경 선택·순서 문제로 재정식화한다. 예산이 고정되면 개선 지점이 정책이 아닌 데이터 관리로 이동한다.
- [[closed-loop-training]]: 폐루프의 환경 공급(궤적 재활용, 갱신)에 '환경 실행 예산 관리'라는 제3 요소를 추가한다.
- [[environment-absence-bottleneck]]·[[environment-supply-scaling]]: 병목이 환경 부재/공급량에서 환경 실행·검증 비용으로 이동함을 규명한다.

## 🔗 관련 논문

- Terminal-Universe: Turning Agent Trajectories into Scalable Terminal E
- CodeMidas: Scaling Agentic Coding RL Environments from Code Itself
- TokenCast: Forecasting Token Consumption During LLM Agent Exe
- SWE-Serve: Benchmarking Agentic Engineering For Production Inference S

## 🏷️ 엔티티

- [[entities/envsched.md|envsched]]
- [[entities/environment-as-training-primitive.md|environment-as-training-primitive]]
- [[entities/training-grade-serving-class.md|training-grade-serving-class]]
- [[entities/rollout-budget-convergence-efficiency.md|rollout-budget-convergence-efficiency]]
- [[entities/environment-supply-scaling.md|environment-supply-scaling]]
- [[entities/closed-loop-training.md|closed-loop-training]]
- [[entities/environment-absence-bottleneck.md|environment-absence-bottleneck]]

## 📐 개념

- [[concepts/environment-scheduling.md|environment-scheduling]]
- [[concepts/environment-execution-cost-bottleneck.md|environment-execution-cost-bottleneck]]
- [[concepts/rollout-environment-coupling.md|rollout-environment-coupling]]

---
_LLM 분석으로 생성됨_
