# TraceSafe: A Systematic Assessment of LLM Guardrails on Multi-Step Tool-Calling Trajectories

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-10
**링크**: http://arxiv.org/abs/2604.07223v1

## 💡 핵심 인사이트

LLM 에이전트의 안전성 취약점은 최종 출력이 아닌 다단계 도구 호출의 중간 실행 궤적에서 발생하며, 기존 가드레일은 이 영역에서 충분히 검증되지 않았다.

## 📖 분석

# TraceSafe: LLM 가드레일의 다단계 도구 호출 궤적 안전성 평가

## 개요
TraceSafe는 LLM이 정적 챗봇에서 자율 에이전트로 진화함에 따라, 최종 출력이 아닌 **중간 실행 궤적(intermediate execution traces)**에서의 안전성을 체계적으로 평가하는 최초의 벤치마크(TraceSafe-Bench)를 제안한다. 기존 안전성 가드레일은 자연어 응답에 대해서는 잘 검증되어 있으나, 다단계 도구 사용 궤적 내에서의 효과는 거의 탐구되지 않았다.

## 핵심 기여
- **TraceSafe-Bench**: 12개 위험 카테고리를 포괄하는 중간 궤적 안전성 평가 벤치마크
- 취약점 표면(vulnerability surface)이 최종 출력에서 중간 실행 단계로 이동한다는 관점 제시
- 멀티스텝 도구 호출 환경에서 기존 가드레일의 한계를 실증적으로 분석

## 기존 Wiki와의 관계
- **LLM Agent**: 본 논문은 LLM 에이전트의 안전성을 도구 호출 궤적 수준에서 평가하며, 에이전트 보안 연구의 새로운 차원을 제시한다. OpenClaw 보안 평가 및 CLAW-Eval과 함께 LLM 에이전트 안전성 연구의 핵심 축을 형성한다.
- **Multi-Agent System**: 다중 에이전트 환경에서 도구 호출 체인의 안전성 문제는 더욱 복잡해지며, 사회적 역학 기반 취약점 연구와도 연결된다.

## 관련 연구 연결
- [[concepts/post-hoc-guardrail-limitation.md|post hoc guardrail limitation]]
- CLAW-Eval(자율 에이전트 신뢰성 평가)과 상호보완적: CLAW-Eval이 전체적 신뢰성을 다룬다면, TraceSafe는 궤적 수준 안전성에 집중
- OpenClaw 보안 평가와 함께 에이전트 보안의 다층적 프레임워크 구성
- Social Dynamics 취약점 연구와 연결: 중간 단계 조작을 통한 공격 벡터 관점 공유

## 🔗 관련 논문

- 2026 04 09 claw eval toward trustworthy evaluation of autonom
- 2026 04 09 social dynamics as critical vulnerabilities that u
- 2026 04 09 who governs the machine a machine identity governa

## 🏷️ 엔티티

- [[entities/llm-agent.md|LLM Agent]]

## 📐 개념

- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/tool-use.md|tool-use]]

---
_LLM 분석으로 생성됨_
