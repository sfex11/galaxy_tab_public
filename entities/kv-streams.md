# kv-streams

**카테고리**: 미분류
**생성일**: 2026-09-30

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-09-30-kv-streams-for-efficient-compaction-in-agentic-rei.md|KV-streams for Efficient Compaction in Agentic Reinforcement]]

### EnvSched: Environment-Aware Scheduling for Rollout-Efficient Agent Rei (2026-10-30)

롤아웃 효율화의 상보적 파트너를 확정한다. KV-streams가 모델 측 반복 프리필 병목을 제거했다면 EnvSched는 환경 측 실행·검증 비용을 스케줄링으로 절감하여, agent RL 인프라 최적화가 모델과 환경의 직교 두 축으로 구조화됨을 보여준다.

### ACCT: Asymmetric Cross-LLM Context Transfer (2026-11-03)

반복 프리필 제거의 배포 측 파트너를 제공한다. KV-streams가 단일 훈련 루프 내 압축 재사용 병목을 다뤘다면 ACCT는 이기종 모델 간 컨텍스트 재사용을 다루어, 같은 컨텍스트의 이중 계산 금지 원리가 모델 경계까지 확장됨을 확정한다.

→ [[sources/2026-11-03-acct-asymmetric-cross-llm-context-transfer.md|상세 보기]]

### The SIMPLE Law for Energy Cost of LLM Inference (2026-11-04)

KV 스트림 기반 압축이 에너지 비용 법칙 하에서 비용 감쇠 메커니즘으로 재평가될 수 있는 근거를 제공한다. 에이전트 RL의 반복 프리필 병목과 토큰 비용 증폭이 동일한 캐시 점유 메커니즘의 두 발현임을 연결한다.

→ [[sources/2026-11-04-the-simple-law-for-energy-cost-of-llm-inference.md|상세 보기]]
