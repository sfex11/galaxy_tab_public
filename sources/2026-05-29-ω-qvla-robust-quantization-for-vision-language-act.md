# Ω-QVLA: Robust Quantization for Vision-Language-Action Models via Composite Rotation and Per-step Scaling

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-05-29  
**링크**: http://arxiv.org/abs/2605.28803v1

## 핵심 요약

Vision-Language-Action (VLA) models unify perception, reasoning, and control within a single policy, yet their multi-billion-parameter backbones and diffusion-based action heads make on-device deployment prohibitively expensive. Prior quantization efforts offer only partial solutions, compressing the LLM backbone while leaving the DiT action head at full precision, or resorting to mixed-precision schemes, driven by the belief that uniformly quantizing the action head is inherently unstable. We c...

---
_자동 생성될_

## 🔗 교차 참조

- → [[sources/2026-05-28-mobilemoe-scaling-on-device-mixture-of-experts]]: 거대 모델의 엣지 디바이스 배포를 가능하게 한다는 공통 목표 아래, 전자는 서브 bilion 규모의 MoE 아키텍처로, 후자는 복합 회전 및 스케일링 기반 양자화로 각각 효율성을 극대화합니다.
