# Toward Scalable Automated Repository-Level Datasets for Software Vulnerability Detection

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-19
**링크**: http://arxiv.org/abs/2603.17974v1

## 💡 핵심 인사이트

함수 단위를 넘어 레포지토리 수준의 취약점 탐지 벤치마크를 자동 생성함으로써, LLM 기반 코드 보안 평가의 확장성과 현실성을 동시에 확보할 수 있다.

## 📖 분석

## Toward Scalable Automated Repository-Level Datasets for Software Vulnerability Detection

본 박사 연구는 소프트웨어 취약점 탐지를 위한 **자동화된 레포지토리 수준 벤치마크 생성기**를 제안한다. 기존 학습 기반 취약점 탐지 연구의 벤치마크는 대부분 함수 단위(function-centric)에 머물러 있어, 실제 소프트웨어 환경에서의 프로시저 간(interprocedural) 호출 관계나 실행 가능한(executable) 설정을 반영하지 못한다는 한계가 있다. 최근 등장한 레포 수준 보안 벤치마크들이 현실적 환경의 중요성을 보여주었으나, 수작업 큐레이션에 의존하여 확장성이 부족하다.

이 연구의 핵심 기여는 **현실적인 취약점을 자동으로 주입(inject)하여 대규모 벤치마크를 생성**하는 파이프라인을 설계하는 것이다. 이를 통해 수작업 없이도 다양한 취약점 패턴을 포함하는 레포지토리 수준 데이터셋을 확장 가능하게 구축할 수 있다.

이 접근법은 LLM 기반 코드 분석 및 에이전트 시스템의 평가와 직접적으로 연결된다. [[concepts/ai-safety.md|ai safety]] 관점에서 LLM이 생성하거나 검토하는 코드의 안전성을 체계적으로 평가할 수 있는 기반을 제공하며, [[concepts/tool-use.md|tool use]] 맥락에서 코드 분석 도구를 활용하는 에이전트의 성능 벤치마킹에도 활용 가능하다. 특히 TraceSafe 연구가 LLM 가드레일의 체계적 평가를 다루었다면, 본 연구는 **코드 보안 도메인에서의 체계적 평가 인프라**를 구축하는 데 초점을 맞춘다. CLAW-Eval이 자율 에이전트의 신뢰성 평가를 다룬 것과도 맥을 같이하며, 보안 취약점이라는 구체적 도메인으로 평가 체계를 확장한다.

## 🔗 관련 논문

- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 09 claw eval toward trustworthy evaluation of autonom
- 2026 04 08 synthetic sandbox for training machine learning en

## 📐 개념

- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/tool-use.md|tool-use]]

---
_LLM 분석으로 재생성됨_
