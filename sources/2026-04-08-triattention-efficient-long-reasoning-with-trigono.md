# TriAttention: Efficient Long Reasoning with Trigonometric KV Compression

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-04-08  
**링크**: http://arxiv.org/abs/2604.04921v1

## 핵심 요약

Extended reasoning in large language models (LLMs) creates severe KV cache memory bottlenecks. Leading KV cache compression methods estimate KV importance using attention scores from recent post-RoPE queries. However, queries rotate with position during RoPE, making representative queries very few, leading to poor top-key selection and unstable reasoning. To avoid this issue, we turn to the pre-RoPE space, where we observe that Q and K vectors are highly concentrated around fixed non-zero center...

---
_자동 생성됨_
