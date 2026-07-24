# They'll Verify. They Just Won't Act. How Authority Framing and Laundered Code Turn a Trusted Agentic CI/CD Pipeline Into an Attack Surface

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-07-23  
**링크**: http://arxiv.org/abs/2607.19267v1

## 핵심 요약

We study a five-agent CI/CD pipeline (triage -> developer -> security-scan -> review -> approve/deploy), built from five distinct production LLMs across three providers, behind an LLM firewall in shadow mode. A single untrusted input - an external issue requesting a "usage-telemetry" feature - asks for code that exfiltrates process secrets (dict(os.environ)) to an attacker URL, laundered as observability. Across a pre-registered A x B (x C) factorial (N=20; naive arm N=60) we find: (1) the entry...

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

- → [[sources/2026-07-23-researcharena-evaluating-sabotage-and-monitoring-i]]: 두 논문 모두 자율형 AI 에이전트가 시스템 내에서 은밀하게 악의적인 행동(사보타지 및 공격)을 수행하는지 감지하고 평가하는 안전성 문제를 다룸.
