# LongSeeker: Elastic Context Orchestration for Long-Horizon Search Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-08
**링크**: http://arxiv.org/abs/2605.05191v1

## 💡 핵심 인사이트

컨텍스트 관리는 '모두 저장'과 '가지치기' 사이의 양자택이 아니라, 현재 관련도에 따라 정보를 다층적 상세도로 유지하는 탄력적 오케스트레이션 문제다.

## 📖 분석

# LongSeeker: Elastic Context Orchestration for Long-Horizon Search Agents

롱호라이즌 검색 에이전트는 추론·도구 호출·정보 관찰을 반복하면서 작업 컨텍스트가 급격히 팽창한다. 기존 접근은 모든 중간 결과를 축적(비용 폭주, 오류 증가)하거나 단순히 가지치기(정보 손실)하는 양극단에 머물렀다. LongSeeker은 **탐색 궤적의 각 부분을 현재 관련도에 따라 상이한 상세도(detail level)로 유지**하는 적응적 컨텍스트 관리를 제안한다.

이를 구현하기 위해 Context-ReAct라는 일반 프레임워크를 도입한다: 에이전트의 각 단계에서 (1) 컨텍스트의 어느 부분을 고해상도로 유지할지, (2) 어느 부분을 요약/압축할지를 동적으로 결정한다. 이는 인간 작업 기억이 모든 정보를 동등한 충실도로 저장하지 않는다는 인지 과학적 원리에 기반한다.

기존 Wiki와의 핵심 연결점: [[entities/adaptive-inference|적응적 추론]]은 모델/라우트 선택(CADENCE), 추측 길이(SpecKV) 등을 결정 차원으로 삼았으나, LongSeeker은 **컨텍스트 상세도 선택**이라는 새로운 결정 차원을 추가한다. [[entities/retry-context-accumulation-loop|재시도-컨텍스트 누적 루프]]가 야기하는 비용 폭주에 대한 구조적 대안을 제공하며, [[entities/token-efficiency|토큰 효율화]]를 '주어진 컨텍스트의 압축'에서 '컨텍스트 구조 자체의 적응적 재구성'으로 확장한다. [[sources/2026-05-07-openseeker-v2-pushing-the-limits-of-search-agents.md|OpenSeeker V2]]와 검색 에이전트 도메인을 공유하며, [[entities/algorithm-system-translation-gap|알고리즘-시스템 번역 간극]]의 맥락에서는 에이전트의 의미론적 관련도 판단을 시스템 수준의 토큰 예산 분배로 번역하는 경로를 구체화한다.

## 🔗 관련 논문

- 2026-05-07-openseeker-v2-pushing-the-limits-of-search-agents.md
- 2026-05-05-speckv-adaptive-speculative-decoding-with-compress.md
- 2026-05-05-to-call-or-not-to-call-a-framework-to-assess-and-o.md
- 2026-04-30-pythia-toward-predictability-driven-agent-native-l.md

## 🏷️ 엔티티

- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/token-efficiency.md|token-efficiency]]
- [[entities/memory-management.md|memory-management]]
- [[entities/long-context.md|long-context]]
- [[entities/longseeker.md|longseeker]]
- [[entities/context-react.md|context-react]]
- [[entities/retry-context-accumulation-loop.md|retry-context-accumulation-loop]]
- [[entities/algorithm-system-translation-gap.md|algorithm-system-translation-gap]]

## 📐 개념

- [[concepts/elastic-context-orchestration.md|elastic-context-orchestration]]
- [[concepts/relevance-adaptive-detail-level.md|relevance-adaptive-detail-level]]
- [[concepts/context-as-pipeline-structural-constraint.md|context-as-pipeline-structural-constraint]]

---
_LLM 분석으로 생성됨_
