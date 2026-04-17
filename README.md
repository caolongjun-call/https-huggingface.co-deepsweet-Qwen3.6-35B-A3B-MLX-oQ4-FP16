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

This model was converted to MLX format from [Qwen/Qwen3.6-35B-A3B](https://huggingface.co/Qwen/Qwen3.6-35B-A3B) using:

- [oMLX v0.36.0](https://github.com/jundot/omlx/releases/tag/v0.3.6)
- specific optimization for M1/M2 Apple Silicon performance, see [jundot/omlx/issues/604](https://github.com/jundot/omlx/issues/604) for more details and benchmarks
- fully [fixed](https://huggingface.co/froggeric/Qwen3.5-35B-A3B-Uncensored-FernflowerAI-MLX-8bit/blob/main/chat_template.README.md) `chat_template.jinja` by [@froggeric](https://huggingface.co/froggeric)

Settings:

- Level: oQ4
- Sensitivity model: Qwen3.6-35B-A3B-MLX-MXFP4-FP16
- Text Only: yes
- Non-quant weight dtype: float16