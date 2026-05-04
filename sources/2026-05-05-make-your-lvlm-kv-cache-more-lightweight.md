# Make Your LVLM KV Cache More Lightweight

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-05
**링크**: http://arxiv.org/abs/2605.00789v1

## 💡 핵심 인사이트

LVLM에서 KV 캐시의 메모리 병목은 텍스트가 아닌 시각 토큰의 구조적 중복성에서 기인하며, 이 중복성은 텍스트 프롬프트를 가이드로 하여 선택적으로 제거할 수 있다.

## 📖 분석

# LightKV: LVLM의 시각 토큰 KV 캐시 경량화

## 정의
LightKV는 대형 비전-언어 모델(LVLM)에서 시각 토큰 임베딩 간의 중복성을 활용하여 KV 캐시 크기를 선택적으로 축소하는 추론 최적화 방법이다. 텍스트 프롬프트를 가이드로 삼아 중요한 시각 토큰만 KV 캐시에 유지함으로써, 프리필 단계에서 시각 토큰이 유발하는 GPU 메모리 과부하를 구조적으로 완화한다.

## 기존 Wiki와의 관계
기존 [[kv-cache-optimization]] 연구가 텍스트 도메인의 스키마 축적([[tools-tax]]), 계층적 메모리 구조([[hierarchical-kv-memory]])에 집중했다면, LightKV는 KV 캐시 최적화의 대상을 텍스트에서 **시각 토큰**으로 확장한다. [[token-pruning]]이 비디오 토큰이나 텍스트 토큰 선택에 적용되던 패러다임을, 프리필-디코딩 파이프라인에서 시각 임베딩의 구조적 중복성이라는 새로운 축으로 구체화한다.

## 핵심 기여
LVLM에서 KV 캐시가 LLM과 동일한 방식으로 채택될 때 발생하는 **모달리티 비대칭적 메모리 비용** 문제를 진단한다 — 시각 토큰이 프리필 단계에서 압도적으로 많은 수를 차지하며, 이 중 상당 부분이 중복 정보를 담고 있다는 실증. 텍스트 프롬프트가 시각 토큰의 중요도를 가이드한다는 발견은 [[token-selection-reasoning]]이 텍스트 내부 토큰에만 적용되던 원리를 시각-언어 간 관계로 확장한다.

## 다른 논문과의 연결점
[[tool-attention]]이 스키마 축적이 KV 캐시를 팽창시키는 상류 문제를 다뤘다면, LightKV는 시각 인코딩이 KV 캐시를 팽창시키는 입력 계층 문제를 다룬다. 두 접근은 에이전트 네이티브 서빙([[agent-native-serving]])에서 상호 보완적으로 적용될 수 있다 — 프리필 단계에서 시각 중복을 제거(LightKV)하고, 디코딩 단계에서 스키마 오버헤드를 제어(Tool Attention).

## 🔗 관련 논문

- 2026-05-01-unifying-sparse-attention-with-hierarchical-memory.md
- 2026-05-01-select-to-think-unlocking-slm-potential-with-local.md

## 🏷️ 엔티티

- [[entities/lightkv.md|lightkv]]
- [[entities/kv-cache-optimization.md|kv-cache-optimization]]
- [[entities/token-pruning.md|token-pruning]]
- [[entities/token-efficiency.md|token-efficiency]]
- [[entities/vlm.md|vlm]]

## 📐 개념

- [[concepts/vision-token-kv-cache-redundancy.md|vision-token-kv-cache-redundancy]]
- [[concepts/text-guided-vision-token-selection.md|text-guided-vision-token-selection]]
- [[concepts/modality-asymmetric-memory-cost.md|modality-asymmetric-memory-cost]]

---
_LLM 분석으로 생성됨_
