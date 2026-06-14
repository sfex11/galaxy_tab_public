# Which Models Are Our Models Built On? Auditing Invisible Dependencies in Modern LLMs

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-06-12  
**링크**: http://arxiv.org/abs/2606.12385v1

## 핵심 요약

Modern LLM training pipelines increasingly rely on other models to generate data, filter corpora, judge outputs, and guide development decisions. These dependencies are recursive: a model may depend on an upstream artifact whose own dependencies are documented only in separate releases and artifacts. As a result, the full dependency structure is fragmented across heterogeneous public artifacts, with complexity and recursive depth far outpacing humans' ability to trace. We introduce ModSleuth, an...

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

- → [[sources/2026-06-11-provenance-grounded-gating-and-adaptive-recovery-i]]: 두 논문 모두 LLM 훈련 파이프라인 내 데이터와 모델 의존성의 출처(provenance)를 추적하고 감사하는 것의 중요성을 다룹니다.

---
**관련**: [[concepts/upstream-irrecoverability.md|upstream irrecoverability]]
