---
language: en
license: apache-2.0
license_link: https://huggingface.co/Qwen/Qwen3.6-35B-A3B/blob/main/LICENSE
pipeline_tag: text-generation
tags:
- mlx
library_name: mlx
base_model: Qwen/Qwen3.6-35B-A3B
---

This model was converted to MLX format and quantized from [Qwen3.6-35B-A3B](https://huggingface.co/Qwen/Qwen3.6-35B-A3B) using [oMLX](https://github.com/jundot/omlx).

## What is "oQ"?

See ["oQ: oMLX Universal Dynamic Quantization"](https://github.com/jundot/omlx/blob/main/docs/oQ_Quantization.md) for details.

## Quantizations

| Text-Only     | Vision-Language  | Text-Only FP16     | Vision-Language FP16  |
|---------------|------------------|--------------------|-----------------------|
| [MLX-oQ8][01] | [MLX-VL-oQ8][05] | [MLX-oQ8-FP16][09] | [MLX-VL-oQ8-FP16][13] |
| [MLX-oQ6][02] | [MLX-VL-oQ6][06] | [MLX-oQ6-FP16][10] | [MLX-VL-oQ6-FP16][14] |
| [MLX-oQ5][03] | [MLX-VL-oQ5][07] | [MLX-oQ5-FP16][11] | [MLX-VL-oQ5-FP16][15] |
| [MLX-oQ4][04] | [MLX-VL-oQ4][08] | [MLX-oQ4-FP16][12] | [MLX-VL-oQ4-FP16][16] |

See ["Evaluation of various MLX quantizations"](https://github.com/deepsweet/mlx-eval/blob/main/results/README.md) for details:

![Qwen3.6-35B-A3B KLD/RAM chart](https://raw.githubusercontent.com/deepsweet/mlx-eval/main/results/Qwen3.6-35B-A3B.svg)

## What is "VL"?

"VL" is Vision-Language, meaning quantization preserves the original model's multimodality.

No "VL" means quantization is Text-Only.

## What is "FP16"?

"FP16" is an M1/M2 Apple Silicon tweak that delivers a very noticeable prompt processing boost, because older M-series lack native BF16 hardware support. See ["Metal FP32 Vs BF16 Vs FP16 benchmark"](https://github.com/deepsweet/metal-fp32-bf16-fp16) for details.

No "FP16" means quantization is better suited for M3+ Apple Silicon.

[01]: https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-oQ8
[02]: https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-oQ6
[03]: https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-oQ5
[04]: https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-oQ4
[05]: https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-VL-oQ8
[06]: https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-VL-oQ6
[07]: https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-VL-oQ5
[08]: https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-VL-oQ4
[09]: https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-oQ8-FP16
[10]: https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-oQ6-FP16
[11]: https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-oQ5-FP16
[12]: https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-oQ4-FP16
[13]: https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-VL-oQ8-FP16
[14]: https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-VL-oQ6-FP16
[15]: https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-VL-oQ5-FP16
[16]: https://huggingface.co/deepsweet/Qwen3.6-35B-A3B-MLX-VL-oQ4-FP16