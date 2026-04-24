---
language: en
license: apache-2.0
license_link: https://huggingface.co/Qwen/Qwen3.5-35B-A3B/blob/main/LICENSE
pipeline_tag: text-generation
tags:
- mlx
library_name: mlx
base_model: Qwen/Qwen3.6-35B-A3B
---

> [!CAUTION]
> "FP16" is M1/M2 Apple Silicon only optimization that leads to a very noticeable prompt processing boost. For details and benchmarks see [jundot/omlx/issues/604](https://github.com/jundot/omlx/issues/604).
>
> Please use [deepsweet/Qwen3.6-35B-A3B-MLX-oQ4](https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-oQ4) if you have M3+ Apple Silicon.

> [!TIP]
> See Q and oQ KL divergence and RAM usage [comparison](https://github.com/jundot/omlx/discussions/945) and choose your poison.

This model was converted to MLX format from [Qwen/Qwen3.6-35B-A3B](https://huggingface.co/Qwen/Qwen3.6-35B-A3B) using [oMLX v0.36.0](https://github.com/jundot/omlx/releases/tag/v0.3.6).

Settings:

- Level: oQ4
- Sensitivity model: Qwen3.6-35B-A3B-MLX-MXFP4-FP16
- Text Only: yes
- Non-quant weight dtype: float16