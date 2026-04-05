# LLM Agent

**카테고리**: LLM  
**생성일**: 2026-04-05  
**최종 수정**: 2026-04-05

## 정의

대규모 언어 모델(LLM)을 기반으로 자율적으로 태스크를 수행하는 에이전트 시스템.

## 핵심 특성

- **자율성**: 인간 개입 없이 연속적인 의사결정 가능
- **도구 사용**: 외부 API, 코드 실행, 파일 조작 등
- **메모리**: 장기 컨텍스트 유지 및 검색
- **계획**: 복잡한 태스크를 서브태스크로 분해
- **적응**: 피드백을 통한 행동 수정

## 주요 연구 주제

### 제어 및 조향
- 감정 벡터를 통한 행동 제어
- Activation steering
- Representation engineering

### 다중 에이전트
- 협력적 태스크 수행
- 역할 분담 및 조정
- 통신 프로토콜

### 안전성
- Misalignment 행동 (blackmail, reward hacking)
- Sycophancy vs honesty 트레이드오프
- Constitutional AI

## 관련 연구

- [[sources/2026-04-03-ActionParty]] - 다중 에이전트 제어
- [[sources/2026-04-04-StopWandering]] - 메타인지 기반 탐색
- [[sources/2026-04-04-BatchedContextual]] - 효율적 추론

## 관련 개념

- [[concepts/emotion-vector]] - 감정 기반 행동 제어
- [[concepts/activation-steering]] - 활성화 조향
- [[concepts/representation-engineering]] - 표현 엔지니어링

## 응용 분야

1. **코딩 에이전트**: 자동 코드 생성 및 디버깅
2. **리서치 에이전트**: 문헌 조사 및 분석
3. **개인 비서**: 일정 관리 및 태스크 자동화

## 외부 참조

- [Anthropic Emotion Research](https://transformer-circuits.pub/2026/emotions/)
- [OpenAI Agent Research](https://openai.com/research)

## 메모

OpenClaw 자체가 LLM Agent의 한 예시. 티씨오도 LLM Agent.
