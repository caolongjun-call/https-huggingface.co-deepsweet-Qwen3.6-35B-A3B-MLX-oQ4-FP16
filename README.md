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

This model was converted to MLX format from [Qwen/Qwen3.6-35B-A3B](https://huggingface.co/Qwen/Qwen3.6-35B-A3B) using [oMLX v0.3.6](https://github.com/jundot/omlx/releases/tag/v0.3.6).

## Settings

- Level: oQ4
- Sensitivity model: Qwen3.6-35B-A3B-MLX-Q8
- Text Only: yes
- Non-quant weight dtype: float16

## What is "oQ"?

See ["oQ: oMLX Universal Dynamic Quantization"](https://github.com/jundot/omlx/blob/main/docs/oQ_Quantization.md) and ["Q and oQ KL Divergence and RAM usage comparison"](https://github.com/jundot/omlx/discussions/945) for details.

## What is "FP16"?

"FP16" is M1/M2 Apple Silicon only optimization that leads to a very noticeable prompt processing boost. See [jundot/omlx/issues/604](https://github.com/jundot/omlx/issues/604) for details.

Use [deepsweet/Qwen3.6-35B-A3B-MLX-oQ4](https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-oQ4) if you have M3+ Apple Silicon.

## Changelog

- 25.04.2026: re-quantize using affine Q8 sensitivity model