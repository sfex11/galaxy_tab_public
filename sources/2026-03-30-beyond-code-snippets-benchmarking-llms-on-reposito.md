# Beyond Code Snippets: Benchmarking LLMs on Repository-Level Question Answering

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-30
**링크**: http://arxiv.org/abs/2603.26567v1

## 💡 핵심 인사이트

LLM의 코드 이해 벤치마크를 단일 파일에서 레포지토리 수준으로 확장함으로써, 실제 개발 환경에서의 cross-file 추론 능력 부족이라는 critical gap을 정량적으로 드러냈다.

## 📖 분석

## Beyond Code Snippets: Benchmarking LLMs on Repository-Level Question Answering

### 개요
본 논문은 LLM의 코드 이해 능력을 **레포지토리 수준**에서 평가하는 최초의 멀티프로젝트 벤치마크 **StackRepoQA**를 제안한다. 기존 코드 QA 벤치마크가 단일 함수나 파일 스니펫에 국한된 반면, 실제 개발자의 프로그램 이해는 다수 파일과 시스템 수준 의존성을 넘나든다는 점에 착안했다. 1,318개의 실제 개발자 질문으로 구성된 이 데이터셋은 레포지토리 전체를 컨텍스트로 요구하는 QA 태스크를 통해 LLM의 cross-file 추론 능력을 체계적으로 측정한다.

### 핵심 기여
- **StackRepoQA**: 실제 StackOverflow 등에서 수집한 개발자 질문 기반의 레포지토리 수준 QA 데이터셋
- 단일 파일이 아닌 **다중 파일 간 의존성 추론**을 요구하는 질문 설계
- 기존 LLM들이 isolated snippet에서는 강한 성능을 보이지만, 레포지토리 수준에서는 성능이 크게 하락함을 실증

### Wiki 연결점
이 연구는 [[llm-benchmark]] 계열의 새로운 축을 추가한다. 기존 FinTradeBench가 금융 추론을, SOL-ExecBench가 GPU 커널 성능을 측정했다면, StackRepoQA는 **코드 이해의 공간적 범위(scope)**를 벤치마크 차원으로 확장한다. 또한 [[long-context]] 연구와 직접적으로 관련되는데, 레포지토리 전체를 컨텍스트 윈도우에 넣어야 하는 설정은 긴 컨텍스트 처리 능력을 필수적으로 요구한다. [[retrieval-augmented-generation]] 파이프라인의 코드 도메인 적용 가능성도 시사하며, 최근의 [[code-generation]] 벤치마크들이 생성에 집중한 것과 달리 **이해(comprehension)** 측면을 강조한다는 점에서 차별화된다.

## 🔗 관련 논문

- 2026 04 10 a systematic study of retrieval pipeline design fo
- 2026 04 10 chatbot based assessment of code understanding in
- 2026 04 10 how much llm does a self revising agent actually n
- 2026 04 10 syntax is easy semantics is hard evaluating llms f

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/long-context.md|long-context]]
- [[concepts/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[concepts/code-generation.md|code-generation]]
- [[concepts/repository-level-code-understanding.md|repository-level-code-understanding]]

---
_LLM 분석으로 재생성됨_
