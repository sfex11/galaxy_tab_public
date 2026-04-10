# FinTradeBench: A Financial Reasoning Benchmark for LLMs

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-23
**링크**: http://arxiv.org/abs/2603.19225v1

## 💡 핵심 인사이트

기존 금융 QA 벤치마크가 정적 재무제표 데이터에 국한된 반면, FinTradeBench는 펀더멘털과 기술적 트레이딩 시그널을 동시에 활용하는 멀티소스 금융 추론 능력을 최초로 체계적으로 평가한다.

## 📖 분석

## FinTradeBench: A Financial Reasoning Benchmark for LLMs

금융 의사결정은 기업 재무제표(규제 신고서 기반)와 가격 동학에서 산출된 트레이딩 시그널 등 이질적인 신호를 종합적으로 추론해야 하는 복잡한 과제다. 최근 LLM이 금융 분석에 활용되기 시작했으나, 기존 금융 QA 벤치마크는 대차대조표 데이터나 단편적 질문에 치우쳐 있어 실제 트레이딩 시나리오의 복합적 추론 능력을 평가하기 어려웠다.

FinTradeBench는 이러한 한계를 극복하기 위해 설계된 벤치마크로, **기업 펀더멘털(regulatory filings 기반)과 기술적 트레이딩 시그널을 동시에 활용하는 금융 추론 능력**을 평가한다. 단순한 재무 수치 조회가 아닌, 다중 소스의 이질적 정보를 통합하여 매수/매도/보유 등의 실질적 투자 결정을 내리는 end-to-end 추론 파이프라인을 테스트한다.

이 연구는 LLM의 금융 도메인 적용에서 두 가지 핵심 과제를 부각시킨다: (1) 정량적 시계열 데이터와 정성적 텍스트 정보의 **멀티모달 통합 추론**, (2) 시간 지평(time horizon)에 걸친 **순차적 의사결정**의 일관성. 특히 기존 벤치마크가 정적 스냅샷 기반 평가에 머물렀다면, FinTradeBench는 동적 시장 환경에서의 추론 능력까지 포괄한다.

[[FrontierFinance]] 벤치마크가 컴퓨터 사용 기반의 장기 금융 과제를 다루는 것과 비교하면, FinTradeBench는 LLM의 순수 추론 능력에 더 집중하며, 펀더멘털과 기술적 분석의 결합이라는 실무적 관점을 강조한다는 점에서 상호보완적이다.

## 🔗 관련 논문

- 2026 04 08 frontierfinance a long horizon computer use benchm

## 📐 개념

- [[concepts/financial-reasoning.md|financial-reasoning]]
- [[concepts/trading-signal-analysis.md|trading-signal-analysis]]

---
_LLM 분석으로 재생성됨_
