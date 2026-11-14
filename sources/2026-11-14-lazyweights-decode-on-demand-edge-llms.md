# LazyWeights: Decode-on-Demand Edge LLMs

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-14
**링크**: http://arxiv.org/abs/2611.17108v1

## 💡 핵심 인사이트

배포 양자화 포맷의 코드 분포 비균등성을 낭비가 아닌 압축 기회로 전환하여, 손실 양자화 위에 무손실 엔트로피 코딩을 적층하고 메모리 계층 경계에서 온디맨드 해제함으로써, 엣지 배포 제약이 모델 교체가 아닌 표현 계층 설계 문제임을 보여준다.

## 📖 분석

# LazyWeights: Decode-on-Demand Edge LLMs

엣지 LLM 배포의 병목이 디바이스 등급에 따라 메모리 용량(4GB Jetson Nano)과 대역폭(8GB Orin Nano Super)으로 분리됨을 출발점으로 한다. 핵심 진단: GPTQ·AWQ·llama.cpp K/I-quant 같은 배포 양자화 포맷은 정수 코드가 균등하지 않음에도 모든 코드에 동일 비트를 배정하여 낭비가 발생한다.

## 기여 구조
1. **압축 가능 양자화**: GPTQ의 코드 배치를 재튜닝해 코드 분포를 비균등하게 만들어 압축률 상한을 끌어올림
2. **손실+무손실 합성**: 인터리브 레인 단위 무손실 Huffman 코딩을 양자화 위에 적층 — 손실 압축이 무손실 압축의 전제 조건이 되는 역전 구조
3. **온디맨드 디코딩**: DRAM-L2 사이 소형 유닛에서 가중치를 인출 시점에 복원

## Wiki 관계
- [[memory-hierarchy-native-inference]]: StrataFlux가 HBM 상한을 RAM/SSD 편입으로 완화했다면 본 논문은 계층 경계에서의 온디맨드 해제 연산을 추가한다. [[precision-escalation-on-demand]]와 '온디맨드 변환' 패턴을 공유
- [[massive-activation]]: 코드 분포 비균등성을 병목이 아닌 압축 기회로 역이용하는 반대 방향 사례
- [[on-device-inference]]: Select to Think(토큰 선택)·Carbon-Taxed(녹색 압축)에 이어 가중치 비트 경제학이라는 제3 축
- [[extreme-low-bit-quantization]]: 코드 비트 수가 아닌 실측 메모리 풋프린트가 평가 기준이 되어야 함을 시사

## 🔗 관련 논문

- StrataFlux: Memory-Hierarchy-Native Low-Bit LLM Inference
- Select to Think: Unlocking SLM Potential with Local Sufficie
- Carbon-Taxed Transformers: A Green Compression Pipeline for
- The SIMPLE Law for Energy Cost of LLM Inference

## 🏷️ 엔티티

- [[entities/lazyweights.md|lazyweights]]
- [[entities/model-compression.md|model-compression]]
- [[entities/on-device-inference.md|on-device-inference]]
- [[entities/memory-hierarchy-native-inference.md|memory-hierarchy-native-inference]]
- [[entities/massive-activation.md|massive-activation]]
- [[entities/extreme-low-bit-quantization.md|extreme-low-bit-quantization]]

## 📐 개념

- [[concepts/code-distribution-aware-quantization.md|code-distribution-aware-quantization]]
- [[concepts/entropy-coded-weights.md|entropy-coded-weights]]
- [[concepts/decode-on-demand-decompression.md|decode-on-demand-decompression]]
- [[concepts/lossy-lossless-composition.md|lossy-lossless-composition]]
- [[concepts/precision-escalation-on-demand.md|precision-escalation-on-demand]]
- [[concepts/decode-phase-gemv-serving-cost.md|decode-phase-gemv-serving-cost]]

---
_LLM 분석으로 생성됨_
