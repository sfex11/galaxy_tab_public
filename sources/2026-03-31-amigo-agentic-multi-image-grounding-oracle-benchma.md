# AMIGO: Agentic Multi-Image Grounding Oracle Benchmark

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-31
**링크**: http://arxiv.org/abs/2603.28662v1

## 💡 핵심 인사이트

에이전틱 VLM 평가를 단일 턴 정답률에서 다중 턴 전략적 질문 생성과 정보 통합 능력 측정으로 전환함으로써, 실제 에이전트 배포 시나리오에 부합하는 평가 패러다임을 제시한다.

## 📖 분석

## AMIGO: Agentic Multi-Image Grounding Oracle Benchmark

AMIGO는 에이전틱 비전-언어 모델(VLM)의 **장기 호라이즌 다중 이미지 추론 능력**을 평가하기 위한 벤치마크이다. 기존 VLM 평가가 단일 이미지·단일 턴 정답 맞추기에 집중했던 한계를 지적하며, 시각적으로 유사한 이미지 갤러리에서 오라클이 비공개로 선택한 타겟 이미지를 식별하는 과제를 제안한다.

### 핵심 메커니즘
모델은 속성 기반 Yes/No/Unsure 질문을 엄격한 프로토콜 하에 순차적으로 던져 타겟을 좁혀간다. 이는 단순 시각 인식을 넘어 **전략적 질문 생성**, **다중 턴 정보 통합**, **불확실성 하 의사결정** 능력을 복합적으로 요구한다. 20 Questions 게임과 유사한 구조이나, 시각적 세밀함과 에이전틱 상호작용이 결합된 점이 차별화된다.

### 학술적 의의
AMIGO는 에이전틱 VLM 연구에서 중요한 빈 공간을 채운다. 기존 벤치마크들이 정적 능력(한 번의 입출력)을 측정했다면, AMIGO는 **동적 상호작용 루프 내에서의 추론 품질**을 측정한다. 이는 실제 에이전트 배포 시나리오(의료 진단 대화, 시각 검색 에이전트 등)에 더 가까운 평가 패러다임이다.

### Wiki 연결점
- [[agentic-vlm]] 개념과 직접 연결: 에이전틱 VLM의 다중 턴 추론 능력을 체계적으로 평가하는 최초의 벤치마크 중 하나
- [[visual-grounding]] 개념의 확장: 단일 이미지 그라운딩을 넘어 다중 이미지 간 비교·구별 그라운딩으로 발전
- [[theory-of-mind]]와 연관: 오라클의 응답 패턴을 추론하며 신념 상태를 업데이트하는 과정이 ToM 추론과 구조적 유사성을 가짐
- Act Wisely(메타인지 도구 사용) 논문과 상보적: AMIGO가 '무엇을 물어야 하는지 아는 능력'을 측정한다면, Act Wisely는 '도구를 언제 써야 하는지 아는 능력'을 다룸

## 🔗 관련 논문

- Act Wisely: Cultivating Meta-Cognitive Tool Use in Agentic M
- MARCUS: An agentic, multimodal vision-language model for car
- ClawBench: Can AI Agents Complete Everyday Online Tasks?
- Appear2Meaning: A Cross-Cultural Benchmark for Stru
- NavTrust: Benchmarking Trustworthiness for Embodied Navigati

## 🏷️ 엔티티

- [[entities/vlm.md|vlm]]
- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/agentic-vlm.md|agentic-vlm]]
- [[concepts/visual-grounding.md|visual-grounding]]
- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/multi-agent-system.md|multi-agent-system]]
- [[concepts/theory-of-mind.md|theory-of-mind]]

---
_LLM 분석으로 재생성됨_
