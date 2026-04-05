# Steerable Visual Representations

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-04-04  
**링크**: None

## 핵심 요약

**Steerable Visual Representations**는 DINOv2, MAE 같은 사전학습된 Vision Transformer의 범용 시각 표현에 텍스트를 통한 **조향 가능성(steerability)**을 부여하는 연구이다. 기존 ViT는 이미지의 가장 두드러진 시각 단서에만 집중하고, 멀티모달 LLM은 언어 중심 표현이라 순수 비전 태스크에서 성능이 떨어진다. 이를 해결하기 위해 **경량 크로스어텐션을 통해 텍스트를 시각 인코더 내부 레이어에 직접 주입하는 조기 융합(early fusion)** 전략을 제안한다. 이를 통해 시각 표현의 품질을 유지하면서도 사용자가 원하는 개념에 집중할 수 있는 조향 가능한 특징을 생성한다.

## 인사이트

1. CLIP처럼 텍스트와 비전을 후기 결합하는 대신, **시각 인코더 내부에 텍스트를 직접 주입하는 조기 융합**이 표현 품질 보존과 조향성을 동시에 달성하는 핵심이다.
2. 범용 시각 표현의 한계(가장 두드러진 단서에만 집중)와 멀티모달 LLM의 한계(언어 중심성)를 **하나의 프레임워크로 동시에 해결**할 수 있다.
3. 태스크별 전용 학습 없이도 이상 탐지, 개인화 객체 판별 등에서 **제로샷 일반화**가 가능하며, 전용 모델에 필적하는 성능을 보인다.

## 응용 가능성

1. **산업 품질 검사/이상 탐지**: 텍스트 프롬프트로 특정 결함 유형에 집중하도록 시각 표현을 조향하여, 별도 학습 없이 다양한 결함을 유연하게 탐지할 수 있다.
2. **개인화 이미지 검색/분류**: 사용자가 관심 있는 세부 속성(색상, 재질, 스타일 등)을 텍스트로 지정하여 해당 속성 중심의 시각 검색 및 분류를 수행할 수 있다.

## 추출된 엔티티

- Transformer

## 추출된 개념

_없음_

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-04-04-SteerableVisualRepresentations.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-04-03-universal-yoco-for-efficient-depth-scaling.md]] (공통 Entity: Transformer)
- [[sources/2026-03-27-avo-agentic-variation-operators-for-autonomous-evo.md]] (공통 Entity: Transformer)
