# Standing on the Shoulders of Giants: Stabilized Knowledge Distillation for Cross--Language Code Clone Detection

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-06
**링크**: http://arxiv.org/abs/2605.02860v1

## 💡 핵심 인사이트

지식 증류의 실질적 병목은 용량 전이가 아니라 형식 준수 안정성이며, 소형 모델은 의미론적 지식을 충분히 인코딩하고 있으나 구조화된 추론 프롬프트의 형식 요구를 신뢰성 있게 충족하지 못한다.

## 📖 분석

# Standing on the Shoulders of Giants: Stabilized Knowledge Distillation for Cross-Language Code Clone Detection (2026-05-06)

## 핵심 기여

크로스 언어 코드 클론 탐지(X-CCD)라는 구체적 도메인에서 지식 증류의 근본적 병목을 재정의한다. 기존 지식 증류가 '용량 전이(capacity transfer)'에 집중했다면, 본 논문은 '형식 준수 안정성(format compliance stability)'을 동등한 병목 축으로 식별한다—소형 모델이 추론 지향 프롬프트를 따라 구조화된 출력을 신뢰성 있게 생성하지 못하는 문제가 지식 부족보다 더 치명적인 장애물임을 실증한다.

## 기존 Wiki와의 관계

### stabilized-knowledge-distillation의 구체적 정의 제공
기존 빈 페이지 상태였던 이 엔티티를 구체화한다: 교사 모델의 추론 능력을 학생 모델로 전이할 때, 학생의 출력 형식 준수성을 명시적으로 안정화하는 지식 증류 변형. 표준 KD가 '학생이 과제 형식을 따를 수 있다'는 암묵적 전제를 가진다면, 안정화 KD는 이 전제 자체가 성립하지 않는 설정을 다룬다.

### cross-language-code-clone-detection의 문제 정의
서로 다른 언어로 작성된 의미론적 동등 프로그램을 탐지하는 과제로, AST·토큰 중첩 등 표면 유사성 기반 특징이 근본적으로 실패하는 도메인. 본 논문은 이를 LLM 기반 의미론적 분석의 구체적 응용 사례로 위치시킨다.

### reasoning-prompt-compliance-gap의 실증적 근거
소형 모델이 지식 자체는 보유하더라도 다단계 추론 프롬프트의 구조적 요구(출력 형식, 추론 단계 분리 등)를 따르지 못하는 현상을 최초로 조작적 정의로 구체화한다.

## 다른 논문과의 연결

- **Turning the TIDE**가 아키텍처 간 지식 전이의 표현 공간 불일치를 다루었다면, 본 논문은 동일 아키텍처 내에서도 형식 준수성이라는 구조적 장벽이 존재함을 보여준다—TIDE의 문제가 '패러다임 간'이라면 본 논문의 문제는 '규모 간'이다.
- **Select to Think**가 SLM의 토큰 선택 전략으로 잠재적 능력을 끌어냈다면, 본 논문은 증류를 통해 그 능력을 영구적으로 고착화하는 보완 경로를 제공한다.
- **output-format-stability**이 [[sources/2026-05-05-standing-on-the-shoulders-of-giants-stabilized-kno.md|이 논문]]의 핵심 설계 목표로 구체화된다.

## 🔗 관련 논문

- Turning the TIDE: Cross-Architecture Distillation for Diffusion Large Models
- Select to Think: Unlocking SLM Potential with Local Sufficiency

## 🏷️ 엔티티

- [[entities/stabilized-knowledge-distillation.md|stabilized-knowledge-distillation]]
- [[entities/cross-language-code-clone-detection.md|cross-language-code-clone-detection]]
- [[entities/knowledge-distillation.md|knowledge-distillation]]
- [[entities/reasoning-prompt-compliance-gap.md|reasoning-prompt-compliance-gap]]
- [[entities/output-format-stability.md|output-format-stability]]
- [[entities/on-device-inference.md|on-device-inference]]
- [[entities/behavioral-stability-transfer.md|behavioral-stability-transfer]]

## 📐 개념

- [[concepts/format-compliance-bottleneck.md|format-compliance-bottleneck]]

---
_LLM 분석으로 생성됨_
