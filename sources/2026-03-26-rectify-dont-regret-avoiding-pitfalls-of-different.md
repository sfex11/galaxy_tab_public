# Rectify, Don't Regret: Avoiding Pitfalls of Differentiable Simulation in Trajectory Prediction

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-03-26  
**링크**: http://arxiv.org/abs/2603.23393v1

## 핵심 요약

Current open-loop trajectory models struggle in real-world autonomous driving because minor initial deviations often cascade into compounding errors, pushing the agent into out-of-distribution states. While fully differentiable closed-loop simulators attempt to address this, they suffer from shortcut learning: the loss gradients flow backward through induced state inputs, inadvertently leaking future ground truth information directly into the model's own previous predictions. The model exploits ...

---
_자동 생성됨_
