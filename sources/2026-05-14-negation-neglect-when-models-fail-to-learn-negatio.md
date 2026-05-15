# Negation Neglect: When models fail to learn negations in training

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-05-14  
**링크**: http://arxiv.org/abs/2605.13829v1

## 핵심 요약

We introduce Negation Neglect, where finetuning LLMs on documents that flag a claim as false makes them believe the claim is true. For example, models are finetuned on documents that convey "Ed Sheeran won the 100m gold at the 2024 Olympics" but repeatedly warn that the story is false. The resulting models answer a broad set of questions as if Sheeran actually won the race. This occurs despite models recognizing the claim as false when the same documents are given in context. In experiments with...

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

- → [[sources/2026-05-14-where-does-reasoning-break-step-level-hallucinatio]]: 두 연구는 LLM이 추론 과정에서 보이는 논리적 오류(부정어 학습 실패 및 단계별 환각)를 미시적 수준에서 진단하고 그 발생 메커니즘을 규명한다는 공통된 목표를 가집니다.
- → [[sources/2026-05-14-senses-wide-shut-a-representation-action-gap-in-om]]: 전자는 훈련 시 부정문 맥락을 무시하는 문제를, 후자는 텍스트와 멀티모달 인식이 충돌할 때의 지각-행동 간극을 다루어, 모델이 입력의 진정한 의미나 맥락을 반영하지 못하는 근본적 인지 결함을 각각 분석합니다.
