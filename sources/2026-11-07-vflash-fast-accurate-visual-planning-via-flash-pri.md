# VFlash: Fast, Accurate Visual Planning via Flash Primitive Decoding

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-07
**링크**: http://arxiv.org/abs/2611.08449v1

## 💡 핵심 인사이트

출력 구조가 사전에 알려진 태스크에서는 토큰 단위 자기회귀 생성이 구조적 낭비이며, 프리미티브의 기하 구조 사전 지식이 제약이 아니라 디코딩 프리미티브 자체의 재정의로 기능한다.

## 📖 분석

VFlash는 물리 AI(로봇공학·자율주행)의 시각 계획을 위한 가속·고정확 디코딩 방법이다. 점·바운딩 박스·궤적 같은 시각 프리미티브가 공간적 목표와 예상 동작을 표현할 수 있음에도, 자기회귀 VLM은 이를 좌표 토큰 단위로 생성하여 예측이 풍부할수록 비용이 증가한다([[autoregressive-generation]], [[token-efficiency]]). VFlash는 프리미티브의 알려진 구조를 활용하는 Flash Primitive Decoding으로 이 병목을 제거한다.

Wiki 관점에서 이 논문은 세 간선을 연다. 첫째, [[template-constrained-decoding]](TeCoD)의 구조적 사례 확장이다. 제약의 근원이 외부 도메인 지식이 아니라 출력 형식 자체의 기하 구조에 있으며, 구조 지식이 출력 공간 축소([[output-space-pruning]])와 가속·정확도 향상을 동시에 실현함을 보여준다. 둘째, [[latent-aligned-planning]]이 연속 행동-이산 토큰 간극을 잠재 정렬로 봉합했다면, VFlash는 동일 간극을 프리미티브 단위 병렬 생성([[parallel-decoding]], [[non-autoregressive-language-modeling]])으로 우회하는 제2 경로를 제공한다. 셋째, [[latent-visual-reasoning]](VideoLVR)이 입력 측 잠재 주입으로 접지를 유지했다면, VFlash는 출력 측 구조 활용으로 토큰 예산을 절감하여 시각 접지의 입력-출력 양면 설계를 완성한다.

핵심 통찰: 출력 구조가 사전에 알려진 태스크에서 토큰 단위 자기회귀는 구조적 낭비이며, 기하 구조 사전 지식은 제약이 아니라 디코딩 프리미티브([[decoder-primitive-redefinition]]) 자체의 재정의로 기능한다.

## 🔗 관련 논문

- Continuous Actions from Discrete Minds: Latent-Aligned Planning for En
- VideoLVR: Latent Visual Reasoning over Grounded Video Evidence
- Q&A on Any Spreadsheet Requires Interpreting Its Grid Struct

## 🏷️ 엔티티

- [[entities/vflash.md|vflash]]
- [[entities/visual-grounding.md|visual-grounding]]
- [[entities/textual-coordinate-grounding.md|textual-coordinate-grounding]]
- [[entities/action-tokenization.md|action-tokenization]]
- [[entities/latent-aligned-planning.md|latent-aligned-planning]]

## 📐 개념

- [[concepts/structure-informed-decoding.md|structure-informed-decoding]]
- [[concepts/primitive-level-generation.md|primitive-level-generation]]
- [[concepts/visual-planning.md|visual-planning]]
- [[concepts/decoder-primitive-redefinition.md|decoder-primitive-redefinition]]
- [[concepts/token-efficiency.md|token-efficiency]]

---
_LLM 분석으로 생성됨_
