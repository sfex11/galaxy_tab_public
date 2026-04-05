# Learning to Commit: Generating Organic Pull Requests via Online Repository Memory

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-03-31  
**링크**: None

## 핵심 요약

LLM 기반 코딩 에이전트가 생성한 PR이 기능적으로는 정확하지만, 프로젝트 고유 컨벤션·내부 API·아키텍처 제약을 무시하여 메인테이너에게 거부되는 문제(**organicity 부족**)를 해결한다. 본 논문은 **Online Repository Memory** 프레임워크를 제안하여, 과거 커밋 히스토리에 대해 지도 대조 반성(supervised contrastive reflection)을 수행한다. 에이전트가 과거 이슈를 정답 없이 풀고, 실제 diff와 비교해 발견된 갭을 재사용 가능한 스킬로 증류한다. 이 스킬(코딩 스타일, API 사용법, 아키텍처 불변량)을 축적하여 새로운 PR 생성 시 조건으로 활용함으로써, 미래 태스크에서 organicity 점수를 효과적으로 향상시켰다.

## 인사이트

1. LLM 코딩 에이전트의 진짜 병목은 기능적 정확성이 아니라, 프로젝트 고유 관습과 암묵적 규칙을 따르지 못하는 **organicity 부족**이다.
2. 단순히 최신 레포 스냅샷을 보여주는 것으로는 부족하며, **저장소의 진화 히스토리**(과거 커밋 패턴)를 학습해야 프로젝트에 맞는 코드를 생성할 수 있다.
3. 과거 이슈를 먼저 풀어보고 실제 정답과 비교하는 **대조 반성** 방식이, 프로젝트별 스킬을 자동으로 추출하는 효과적인 메커니즘이다.

## 응용 가능성

1. **기업 내부 코드베이스 자동화**: 사내 레포의 커밋 히스토리를 학습시켜, 팀 컨벤션과 내부 API를 준수하는 PR을 자동 생성하는 코딩 에이전트에 적용할 수 있다.
2. **오픈소스 기여 도우미**: 처음 기여하는 개발자에게 해당 프로젝트의 암묵적 규칙과 스타일을 스킬로 제공하여, 리뷰 반려율을 줄이는 온보딩 도구로 활용할 수 있다.

## 추출된 엔티티

- LLM Agent

## 추출된 개념

_없음_

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-03-31-LearningtoCommitGeneratingOrga.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-04-01-dynamic-dual-granularity-skill-bank-for-agentic-rl.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-27-claudini-autoresearch-discovers-state-of-the-art-a.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-04-stop-wandering-efficient-vision-language-navigatio.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-26-code-review-agent-benchmark.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-31-dynamic-dual-granularity-skill-bank-for-agentic-rl.md]] (공통 Entity: LLM Agent)
