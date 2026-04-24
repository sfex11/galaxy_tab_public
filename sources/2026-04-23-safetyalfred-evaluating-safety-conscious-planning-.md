# SafetyALFRED: Evaluating Safety-Conscious Planning of Multimodal Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-23
**링크**: http://arxiv.org/abs/2604.19638v1

## 💡 핵심 인사이트

위험을 '인식'하는 것과 위험을 '회피 계획에 반영'하는 것은 별개의 능력이며, disembodied QA 기반 안전 평가는 체화 에이전트의 실제 안전성을 체계적으로 과대평가한다.

## 📖 분석

# SafetyALFRED: 안전 인식 계획의 체화 평가

## 정의
ALFRED 체화 에이전트 벤치마크에 6개 범주의 실제 주방 위험 요소를 증강하여, MLLM이 체화 환경에서 위험을 **사후 인식이 아닌 사전 계획 단계에서 능동적으로 회피**하는 능력을 평가하는 벤치마크.

## 기존 Wiki와의 관계

### sandbox-liveworld-gap의 새로운 축 추가
기존 Wiki에서 ClawBench가 샌드박스-라이브 격차를 웹 태스크 도메인에서 실증했다면, SafetyALFRED는 **안전성 평가 방법론 자체의 격차**를 노출한다. disembodied QA에서 위험을 '인식'하는 능력과, 체화 환경에서 위험을 '회피 계획에 반영'하는 능력은 별개의 능력이며, 전자가 후자를 보장하지 않는다.

### closed-loop-evaluation과의 연결
Fail2Drive가 자율주행에서 정적 평가와 폐루프 평가의 격차를 보였듯, SafetyALFRED는 안전성 도메인에서 동일한 패턴을 확인한다: 11개 SOTA 모델 중 QA 기반 안전 평가에서는 높은 점수를 받지만 체화 계획에서는 위험을 무시하는 모델이 다수 존재.

### MLLM/VLM 합성 분석에의 기여
기존 VLM 합성(26편)에서 공간 추론이 가장 두꺼운 연구 축이었으나, SafetyALFRED는 **공간 추론이 안전 계획으로 어떻게 변환되는지**를 평가한다. 공간적 위험 인지(perception)와 행동 계획(planning) 사이의 간극을 정량화하는 프레임워크를 제공.

### ai-safety: 평가 방법론의 근본적 문제
기존 ai-safety 개념이 주로 텍스트 생성 수준의 안전성(jailbreak, 출력 필터링)에 집중했다면, SafetyALFRED는 안전성을 **환경 내 행동 계획**으로 확장한다. 이는 thought-action-separation, trajectory-opacity 등 기존 Wiki 개념들이 체화 도메인에서 어떻게 구체화되는지를 보여주는 실증적 근거가 된다.

## 🔗 관련 논문

- navtrust-benchmarking-trustworthiness-for-embodied-navi
- fail2drive-benchmarking-closed-loop-driving-genera
- clawbench-can-ai-agents-complete-everyday-online-t
- agentvln-towards-agentic-vision-and-language-navig

## 🏷️ 엔티티

- [[entities/safetyalfred.md|safetyalfred]]
- [[entities/mllm.md|mllm]]
- [[entities/vlm.md|vlm]]
- [[entities/embodied-ai.md|embodied-ai]]
- [[entities/llm-agent.md|llm-agent]]
- [[entities/ai-safety.md|ai-safety]]
- [[entities/agentic-vlm.md|agentic-vlm]]

## 📐 개념

- [[concepts/proactive-safety-planning.md|proactive-safety-planning]]
- [[concepts/disembodied-vs-embodied-safety-evaluation.md|disembodied-vs-embodied-safety-evaluation]]
- [[concepts/hazard-avoidance-planning.md|hazard-avoidance-planning]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-04-22-using-large-language-models-for-embodied-planning-]]: 둘 다 LLM 기반 체화 에이전트의 안전성 평가를 다루며, 하나는 DESPITE 벤치마크로 계획의 체계적 위험을, 다른 하나는 SafetyALFRED로 주방 환경에서의 사전 회피 능력을 평가한다.
- → [[sources/2026-04-24-interval-pomdp-shielding-for-imperfect-perception-]]: 둘 다 자율/체화 에이전트의 안전성을 다루며, 하나는 불완전 인지 하에서 형식적 증명 가능한 실드링을, 다른 하나는 벤치마크를 통해 안전 인식 계획 능력을 실증적으로 평가한다.
