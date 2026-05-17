# Can Blindfolded LLMs Still Trade? An Anonymization-First Framework for Portfolio Optimization

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-20
**링크**: http://arxiv.org/abs/2603.17692v1

## 💡 핵심 인사이트

LLM 트레이딩 에이전트의 성능이 진정한 시장 이해에 기반하는지 검증하기 위해 티커 익명화라는 '눈가림' 방법론을 제안하여, 암기 편향과 생존자 편향을 체계적으로 제거하는 프레임워크를 구축했다.

## 📖 분석

## Can Blindfolded LLMs Still Trade? An Anonymization-First Framework for Portfolio Optimization

본 논문은 LLM 기반 트레이딩 에이전트의 신뢰성 문제를 정면으로 다룬다. 핵심 질문은 명확하다: LLM이 실제 시장 역학을 이해하는 것인지, 아니면 사전학습 과정에서 암기한 티커(ticker) 연관성을 활용하는 것인지?

저자들은 두 가지 허위 성능 원인을 지적한다. 첫째, **암기 편향(memorization bias)**: 사전학습 데이터에 포함된 특정 종목 정보가 예측에 누출되는 문제. 둘째, **생존자 편향(survivorship bias)**: 결함 있는 백테스팅이 성과를 과대평가하는 문제. 이를 해결하기 위해 LLM을 '눈가림(blindfold)'하는 익명화 우선 프레임워크를 제안한다. 티커명과 기업 식별정보를 제거한 상태에서 순수한 시장 신호만으로 포트폴리오 최적화를 수행하게 함으로써, 모델의 진정한 시장 이해도를 검증한다.

이 연구는 LLM 에이전트의 **신뢰성 평가** 방법론에 중요한 기여를 한다. 특히 멀티 에이전트 트레이딩 시스템에서 각 에이전트가 정당한 패턴 인식에 기반하는지 검증하는 체계적 프레임워크를 제시했다는 점에서 의의가 있다. AI 안전성 관점에서도, 모델이 '무엇을 아는지'와 '무엇을 암기했는지'를 구분하는 방법론은 범용적 가치를 지닌다.

[[entities/llm-agent|LLM Agent]] 연구와 직결되며, FrontierFinance 벤치마크와 함께 LLM 금융 에이전트 평가의 양대 축을 형성한다. [[concepts/ai-safety|AI Safety]] 측면에서 암기 편향 제거는 모델 신뢰성의 근본 조건이다.

## 🔗 관련 논문

- 2026 04 08 frontierfinance a long horizon computer use benchm
- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 09 claw eval toward trustworthy evaluation of autonom

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/multi-agent-system.md|multi-agent-system]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[concepts/blind-tool-invocation.md|blind tool invocation]]

---
**관련**: [[entities/blind-tool-invocation.md|blind tool invocation]]
