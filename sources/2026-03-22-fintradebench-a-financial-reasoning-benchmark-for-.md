# FinTradeBench: A Financial Reasoning Benchmark for LLMs

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-22
**링크**: http://arxiv.org/abs/2603.19225v1

## 💡 핵심 인사이트

기존 금융 QA 벤치마크가 대차대조표 단일 신호에 치중된 반면, FinTradeBench는 펀더멘털과 트레이딩 시그널을 동시에 추론하는 복합 금융 의사결정 능력을 최초로 체계적으로 평가한다.

## 📖 분석

## FinTradeBench: A Financial Reasoning Benchmark for LLMs

**분류**: LLM 벤치마크 / 금융 AI

FinTradeBench는 LLM의 금융 의사결정 능력을 평가하기 위한 벤치마크로, 기존 금융 QA 벤치마크가 대차대조표 데이터에 치중된 한계를 극복하고자 한다. 이 벤치마크의 핵심 차별점은 **이질적 신호(heterogeneous signals)** — 규제 공시에서 도출된 기업 펀더멘털과 가격 동학에서 계산된 트레이딩 시그널 — 을 동시에 추론해야 한다는 점이다.

### 핵심 기여
- **다중 신호 통합 추론**: 정성적(공시 분석) + 정량적(가격 시그널) 데이터를 결합한 금융 추론 능력 측정
- **실제 의사결정 시뮬레이션**: 단순 QA를 넘어 실제 트레이딩 판단에 가까운 태스크 설계
- **LLM 금융 추론의 한계 진단**: 기존 모델들이 복합 금융 시그널 처리에서 보이는 약점 분석

### 기존 Wiki와의 연결
이 연구는 [[FrontierFinance|FrontierFinance]] 벤치마크와 직접적으로 비교된다. FrontierFinance가 장기 컴퓨터 활용(long-horizon computer use) 관점에서 금융 에이전트를 평가한다면, FinTradeBench는 **추론 능력 자체**에 초점을 맞춘다. 두 벤치마크는 상호보완적이며, LLM 금융 응용의 서로 다른 차원을 측정한다.

또한 LLM Agent의 도구 사용(tool-use) 및 다단계 추론과도 연관되며, 금융 도메인에서의 AI 안전성(ai-safety) 문제 — 특히 잘못된 금융 추론이 초래할 수 있는 리스크 — 와도 맞닿아 있다.

## 🔗 관련 논문

- 2026 04 08 frontierfinance a long horizon computer use benchm

## 📐 개념

- [[concepts/financial-reasoning.md|financial-reasoning]]
- [[concepts/llm-benchmark.md|llm-benchmark]]

---
_LLM 분석으로 재생성됨_
