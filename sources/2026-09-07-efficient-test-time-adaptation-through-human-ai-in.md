# Efficient Test-Time Adaptation through Human-AI Interaction

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-07
**링크**: http://arxiv.org/abs/2609.04141v1

## 💡 핵심 인사이트

개방형 과제에서 개인의 품질 기준은 사전에 명세될 수 없으므로 반복적 인간-에이전트 상호작용 자체가 테스트타임 적응의 계산 매체가 되며, 적응의 화폐가 토큰에서 상호작용 라운드로 대체된다.

## 📖 분석

## 핵심 논지

인구 규모 사전학습은 광범위한 역량을 부여하지만, 산출물은 개인이 명성을 걸 수 있는 품질에 드물게 도달한다. 개방형 과제의 성공 기준은 이질적·비문서화되어 개인 전문성이 평균으로부터의 상승과 이탈에 존재하므로, 사전 진술 불가능한 기준은 반복적 상호작용으로만 표면화된다 — 이 표면화 과정 자체가 테스트타임 적응의 본체다.

## Wiki 축적과의 관계

**신호 채널의 해법 측**: 2026-09-04 진단([[undetectable-feedback-signal]]) — 사용자 피드백이 LLM이 판독 불가능한 고유 신호 — 에 대해, 판독 불가능성은 신호의 결함이 아닌 단일 턴 채널의 결함임을 보인다. 다중 라운드 프로토콜이 [[user-feedback-signal]]을 점진적으로 추출 가능한 형태로 변환한다.

**주변 분포 천장의 개인화 발현**: 인구 규모 훈련이 형성한 P(y)는 평균적 품질의 상한이며([[marginal-distribution-ceiling]]), 개인 품질은 천장 돌파가 아니라 인간 상호작용을 조건으로 하는 재조건화로 달성된다. 조건화의 화폐가 토큰에서 상호작용 라운드로 대체되어 [[test-time-scaling]]의 새 축을 형성한다.

**순환 타당성의 외부 해소**: [[human-trace-external-anchoring]]이 자기 평가의 닫힌 고리를 여는 닻이라면, 본 논문은 적응 기준 자체의 출처를 인간 상호작용에 두어 테스트타임 적응 전체가 자기참조 루프 밖에 놓이게 한다.

**개인화 에이전트의 존재론**: 평균적 능력은 사전학습으로 공리화되지만 개인 기준은 과제마다 유도되어야 하며, 이 유도 비용의 최소화가 [[personal-ai-agent]]의 설계 목표다.

## 후속 질문

에이전트의 제안이 사용자 기준 형성에 개입하면 [[preference-discovery-construction-boundary]]가 흐려지고 [[agent-human-economic-power-asymmetry]]의 새 진입점이 된다. 효율화 압력이 동의 수렴으로 붕괴하면 기준 표면화가 [[sycophancy]] 최적화로 변질될 위험이 있다.

## 🔗 관련 논문

- User Feedback Provides a Unique Signal that LLMs Can not Detect

## 🏷️ 엔티티

- [[entities/personal-ai-agent.md|personal-ai-agent]]
- [[entities/user-feedback-signal.md|user-feedback-signal]]
- [[entities/tacit-criteria-surfacing.md|tacit-criteria-surfacing]]
- [[entities/human-trace-external-anchoring.md|human-trace-external-anchoring]]
- [[entities/undetectable-feedback-signal.md|undetectable-feedback-signal]]

## 📐 개념

- [[concepts/marginal-distribution-ceiling.md|marginal-distribution-ceiling]]
- [[concepts/capability-task-quality-decoupling.md|capability-task-quality-decoupling]]
- [[concepts/adaptive-validity.md|adaptive-validity]]
- [[concepts/preference-discovery-construction-boundary.md|preference-discovery-construction-boundary]]
- [[concepts/sycophancy.md|sycophancy]]
- [[concepts/test-time-scaling.md|test-time-scaling]]
- [[concepts/human-as-harness-internal-component.md|human-as-harness-internal-component]]

---
_LLM 분석으로 생성됨_
