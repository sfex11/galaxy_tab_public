# Standing on the Shoulders of Giants: Stabilized Knowledge Distillation for Cross--Language Code Clone Detection

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-05
**링크**: http://arxiv.org/abs/2605.02860v1

## 💡 핵심 인사이트

지식 증류의 실제 병목은 능력 전이가 아니라 안정성 전이에 있으며, 소형 모델이 구조화된 출력을 신뢰성 있게 생성하도록 만드는 것이 도메인 특화 배포를 위한 핵심 전제 조건이다.

## 📖 분석

# Standing on the Shoulders of Giants: Stabilized Knowledge Distillation for Cross-Language Code Clone Detection

## 핵심 기여

본 논문은 지식 증류(Knowledge Distillation)의 목표를 '능력 전이'에서 '안정성 전이'로 확장한다. 대형 LLM이 교차 언어 코드 클론 탐지(X-CCD)에서 보여주는 의미론적 이해 능력을 소형 오픈소스 모델로 증류할 때, 단순히 정답률을 높이는 것을 넘어 **출력 형식 준수(output format compliance)와 추론 지시 따르기(prompt compliance)**를 동시에 안정화하는 기법을 제안한다.

## 기존 Wiki와의 관계

기존 [[knowledge-distillation]]은 아키텍처 패러다임 전환(자회귀↔확산)이나 파라미터 축소에 집중했으나, 본 논문은 증류 대상에 '행동 안정성'이라는 새로운 차원을 추가한다. 소형 모델이 의미론적 판단은 할 수 있으나 구조화된 출력을 신뢰성 있게 생성하지 못하는 현상을 문제화하고, 이를 증류 과정 자체에서 해결한다.

[[model-compression]]의 스코프에 '도메인 특화 행동 안정성 압축'을 추가한다. 탄소-정확도 트레이드오프(Carbon-Taxed Transformers)나 아키텍처 전환(TIDE)과 병렬적으로, 동일 아키텍처 내에서 대형→소형으로 안정성을 이전하는 실용적 경로를 제공한다.

[[on-device-inference]]의 배포 가능성을 구체화한다. 비용·프라이버시·재현성 문제로 대형 LLM을 블랙박스로 사용할 수 없는 환경에서, 증류된 소형 모델이 온디바이스에서 X-CCD를 수행할 수 있게 한다.

## 새로운 관점

증류의 근본적 전제인 '표현 공간의 동일성' 가정에 대한 실용적 회피 경로를 제시한다. 표현 공간이 다르더라도, 대형 모델의 **입출력 행동 패턴(특히 구조화된 출력 생성 패턴)**을 소형 모델이 모방하도록 증류하면 도메인 특화 배포가 가능하다는 실증이다.

## 연결점

- [[algorithm-system-translation-gap]]: 대형 모델의 '알고리즘 수준' 이해를 '시스템 수준' 배포 가능한 형태로 번역하는 구체적 사례
- [[execution-verification]]: 출력 형식 불안정성이 하류 검증 파이프라인을 무력화한다는 문제 인식을 공유
- [[marginal-distribution-ceiling]]: 소형 모델의 주변 분포 상한선을 증류로 높이려는 시도이나, 타겟 분포 무변경 원칙과는 다른 접근(소형 모델의 분포 자체를 변화시킴)

## 🔗 관련 논문

- sources/2026-05-01-turning-the-tide-cross-architecture-distillation-f.md
- sources/2026-04-30-carbon-taxed-transformers-a-green-compression-pipe.md
- sources/2026-05-01-select-to-think-unlocking-slm-potential-with-local.md
- sources/2026-05-05-generating-statistical-charts-with-validation-driv.md

## 🏷️ 엔티티

- [[entities/knowledge-distillation.md|knowledge-distillation]]
- [[entities/model-compression.md|model-compression]]
- [[entities/on-device-inference.md|on-device-inference]]
- [[entities/cross-language-code-clone-detection.md|cross-language-code-clone-detection]]
- [[entities/stabilized-knowledge-distillation.md|stabilized-knowledge-distillation]]

## 📐 개념

- [[concepts/cross-language-code-clone-detection.md|cross-language-code-clone-detection]]
- [[concepts/stabilized-knowledge-distillation.md|stabilized-knowledge-distillation]]
- [[concepts/output-format-stability.md|output-format-stability]]
- [[concepts/behavioral-stability-transfer.md|behavioral-stability-transfer]]
- [[concepts/reasoning-prompt-compliance-gap.md|reasoning-prompt-compliance-gap]]

---
_LLM 분석으로 생성됨_
