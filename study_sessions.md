## Upcoming

- Comparing LTX 2.5 Diffusion Decoder to its Convolutional Decoder in both results & code
- [FixAnything](https://fix-anything.github.io/) - Wan I2V conditioned on point clouds & gaussians to produce new camera moves

## Past

#### [Wednesday 02.09.26] PiD paper review, Vista4D, LTX 2.5 diffusion decoder
- Reviewed [Pixel Diffusion paper](https://arxiv.org/abs/2605.23902) from Nvidia
  - [NTK-Aware scaling](https://www.reddit.com/r/LocalLLaMA/comments/14lz7j5/ntkaware_scaled_rope_allows_llama_models_to_have/)
  - Uses distillation
  - Based on [PixelDiT](https://arxiv.org/abs/2511.20645)
  - Allows decoding early via their sigma-aware gating mechanism
  - Improves FLUX.1, FLUX.2, SD3, and some Representational AutoEncoder (RAE)-based methods which use DINOv2 encodings
- Recap of interesting papers e.g. [Vista4D](https://arxiv.org/abs/2604.21915), [Reshoot Anything](https://arxiv.org/abs/2604.21776)
- Began looking through codebase for [LTX 2.5 Diffusion decoder](https://github.com/Lightricks/LTX-2/blob/main/packages/ltx-core/src/ltx_core/model/video_vae/diffusion_video_decoder.py#L72)

#### [Tuesday 25.08.26] Distillation, LTX
- LTX architecture overview in ComfyUI and [node-based webpage](https://plasmax.github.io/mlearn/visualizations/ltx25graph.html)
- Practical session looking at distillation in notebook & colab, using two moons & a simple 2D checkerboard example

#### [Tuesday 18.08.26] Normalized Attention Guidance
- Attempted to reproduce [NAG](https://arxiv.org/abs/2505.21179) on the lightweight Nitro-E model inside [colab](https://colab.research.google.com/drive/16HkHCdJg0m5k_oTowi5yyLXQe3xYI5mc?usp=sharing).
- Normalized Attention Guidance moves the conditional & unconditional steering closer to where the text embeddings come in, rather than running the full vector prediction twice and then balancing with CFG (Classifier-Free Guidance).

#### [Thursday 13.08.26] Rectified Flow
- Applied [ReFlow](https://arxiv.org/abs/2209.03003) to our simple [two moons colab](https://colab.research.google.com/drive/1pZ6lqkELdrFNHwJdRLRbC8KAvUqLJYTN?usp=sharing)

#### [Tuesday 04.08.26] MNIST Classifier
- Trained a basic [MNIST Classifier in colab](https://colab.research.google.com/drive/1xDr2p00olS6rPpR4QSayjH1eFS3-eUYG?usp=sharing), inspired by Adam Harley's [awesome visualization](https://adamharley.com/nn_vis/cnn/2d.html).

#### [Tuesday 28.07.26] Zero-initialize convolutional layers
- Looked at why the last layer on vector prediction networks is often zero-initialized.

...


#### [Sunday 18.01.2026] Attention is all we need