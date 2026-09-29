---
layout: page
title: FluxServe
description: A lightweight, high-performance serving engine for diffusion language models.
github: https://github.com/FLX-OSS/FluxServe
importance: 1
---

[FluxServe](https://github.com/FLX-OSS/FluxServe) is an open-source serving engine built specifically
for **diffusion language models (dLLMs)**, aiming at low-latency, high-throughput inference on both
single- and multi-GPU setups. It is released under the MIT license.

Most serving stacks are designed around autoregressive LLMs, whose decoding pattern differs from
iterative diffusion decoding. FluxServe targets that gap directly.

## Highlights

- **Block-causal attention** implemented natively for autoregressive diffusion decoding
- **Dynamic request scheduler** with fine-grained, block-level request management
- **Variable-length prefill and block-decode** as first-class operations
- **Multi-GPU serving** with tensor, data, and expert parallelism
- Built on **FlashInfer** and **FlashAttention**, with a C++ control plane and Python execution
- Model support for **LLaDA2.X**, **Diffusion-Gemma**, and **Nemotron-Labs-Diffusion**
- Tuned for **H100, H200, B200, and GH200** GPUs

## My contributions

I integrate new dLLM architectures into the serving framework, contributing model support and
runtime.
