# AMIGO: Agentic Multi-Image Grounding Oracle Benchmark

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-01
**링크**: http://arxiv.org/abs/2603.28662v1

## 💡 핵심 인사이트

단일 이미지·단일 턴 평가를 넘어, 시각적으로 유사한 다중 이미지 갤러리에서 순차적 질문 전략을 통해 타겟을 식별하는 장기 지평 벤치마크를 최초로 제안하여 에이전틱 VLM의 능동적 추론 능력을 체계적으로 측정할 수 있게 했다.

## 📖 분석

## AMIGO: Agentic Multi-Image Grounding Oracle Benchmark

AMIGO는 에이전틱 비전-언어 모델(VLM)의 **다중 이미지, 다중 턴 그라운딩 능력**을 평가하는 장기 지평(long-horizon) 벤치마크이다. 기존 VLM 평가가 단일 이미지·단일 턴 정답 맞추기에 머물렀다면, AMIGO는 시각적으로 유사한 이미지 갤러리에서 오라클이 숨긴 타겟 이미지를 **순차적 Yes/No/Unsure 질문**을 통해 식별하는 과제를 설계했다. 이는 에이전트가 속성 기반 질문 전략을 세우고, 응답에 따라 후보를 점진적으로 좁혀가는 **능동적 추론(active inference)** 능력을 요구한다.

### 기존 연구와의 연결

**agentic-vlm** 개념과 직접적으로 연결된다. MARCUS가 의료 영역에서 에이전틱 VLM의 실용성을 보여줬다면, AMIGO는 에이전틱 VLM의 **시각적 변별력과 전략적 질문 생성 능력**을 체계적으로 측정하는 벤치마크를 제공한다. 또한 Act Wisely의 메타인지적 도구 사용 연구와 맥을 같이하는데, 질문 순서를 최적화하려면 모델이 자신의 불확실성을 인식하고 정보 이득이 큰 질문을 선택해야 하기 때문이다.

**visual-grounding** 개념의 확장으로도 볼 수 있다. 기존 visual grounding이 단일 이미지 내 객체 위치 특정에 집중했다면, AMIGO는 이를 **다중 이미지 간 식별**로 확장하여 더 미세한 시각적 차이를 포착하는 능력을 평가한다. ClawBench가 웹 환경에서의 에이전트 과제 완수를 평가한 것처럼, AMIGO는 시각 도메인에서의 장기 에이전틱 상호작용 평가를 다룬다.

엄격한 프로토콜(strict protocol) 하의 평가라는 점에서 llm-benchmark 계열의 최근 추세—통제된 조건에서의 체계적 능력 측정—를 따르고 있다.

## 🔗 관련 논문

- Act Wisely: Cultivating Meta-Cognitive Tool Use in Agentic M
- MARCUS: An agentic, multimodal vision-language model for car
- ClawBench: Can AI Agents Complete Everyday Online Tasks?
- Appear2Meaning: A Cross-Cultural Benchmark for Stru
- TraceSafe: A Systematic Assessment of LLM Guardrails on Mult

## 🏷️ 엔티티

- [[entities/vlm.md|vlm]]
- [[entities/mllm.md|mllm]]

## 📐 개념

- [[concepts/agentic-vlm.md|agentic-vlm]]
- [[concepts/visual-grounding.md|visual-grounding]]
- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/vision-language-model.md|vision-language-model]]
- [[concepts/multi-agent-system.md|multi-agent-system]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[concepts/paired-route-benchmark.md|paired route benchmark]]

---
**관련**: [[concepts/image-grounding.md|image grounding]]

---
**관련**: [[concepts/executable-benchmark.md|executable benchmark]]

---
**관련**: [[concepts/dynamic-benchmark.md|dynamic benchmark]]

---
**관련**: [[entities/gui-grounding.md|gui grounding]]
