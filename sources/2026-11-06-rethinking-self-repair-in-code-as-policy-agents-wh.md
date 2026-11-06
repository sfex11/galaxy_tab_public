# Rethinking Self-Repair in Code-as-Policy Agents: What Drives Retry Success?

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-11-06  
**링크**: http://arxiv.org/abs/2611.06863v1

## 핵심 요약

Code-as-policy agents often use execution feedback to retry failed programs. Additional sampling and task guidance can also improve success, leaving the contribution of failure-specific feedback unclear. We study this question in simulated robot manipulation. A fixed lookup selects feedback templates using failure labels and the API variant. A frozen code model generates a fresh program after each scene reset. On the same 252 initial failures, Qwen2.5-Coder-7B recovers 85.3% within five retries,...

## 인사이트

1. 추출 필요
2. 추출 필요
3. 추출 필요

## 응용 가능성

1. 추출 필요
2. 추출 필요

## 추출된 엔티티

_없음_

## 추출된 개념

_없음_

## 메모

_자동 생성됨_

## 🔗 교차 참조

- → [[sources/2026-11-06-on-turn-level-best-of-n-sampling-for-scaling-llm-a]]: 재시도 성공의 원인이 실패별 피드백인지 단순 추가 샘플링인지 분해하는 질문과, 턴 단계 best-of-N 샘플링이 각각 에이전트의 샘플링 기반 개선 문제를 다룬다.
- → [[sources/2026-11-04-veriharm-bench-measuring-harmful-success-in-llm-co]]: 코드 에이전트의 '성공' 판정을 테스트 통과 너머에서 재검토한다는 점에서 연결되며, 하나는 유해한 성공의 존재를 하나는 재시도 성공의 원인을 밝힌다.
