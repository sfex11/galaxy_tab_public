# AutoMegaKernel: A Statically-Checked Agent Harness for Self-Retargeting Megakernel Synthesis

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-06-10  
**링크**: http://arxiv.org/abs/2606.09682v1

## 핵심 요약

AutoMegaKernel (AMK) compiles a HuggingFace Llama-family model into a single persistent cooperative CUDA kernel that runs the whole forward pass in one launch, with no per-model hand-written CUDA. The contribution is the system, not raw speed.
  A frozen schedule-IR validator statically certifies deadlock-freedom and race-freedom via static graph checks (not a mechanized proof), so an unsafe agent-proposed schedule is rejected before launch: across 7,160 adversarial schedules (6,091 unsafe) it h...

## 인사이트

1. 추출 필요
2. 추출 필요
3. 추출 필요

## 응용 가능성

1. 추출 필요
2. 추출 필요

## 추출된 엔티티

_없음_

## 추출된 개념

_없음_

## 메모

_자동 생성됨_
