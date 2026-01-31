# HSI-VAR: Rethinking Hyperspectral Restoration through Spatial–Spectral Visual Autoregression</span><br>
![Language](https://img.shields.io/badge/language-python-red)

Contact: xmwang28@gmail.com

---
**Abstract:** Hyperspectral images (HSIs) capture richer spatial–spectral information beyond RGB, yet real-world HSIs often suffer from a composite mix of degradations, such as noise, blur, and missing bands.
Existing generative approaches for HSI restoration like diffusion models require hundreds of iterative steps, making them computationally impractical for high-dimensional HSIs.
While regression models tend to produce oversmoothed results, failing to preserve critical structural details.
We break this impasse by introducing HSI-VAR, rethinking HSI restoration as an autoregressive generation problem, where spectral and spatial dependencies can be progressively modeled rather than globally reconstructed.
HSI-VAR incorporates three key innovations: (1) Latent–condition alignment, which couples semantic consistency between latent priors and conditional embeddings for precise reconstruction; (2) Degradation-aware guidance, which uniquely encodes mixed degradations as linear combinations in the embedding space for automatic control, remarkably achieving a nearly $50\%$ reduction in computational cost at inference; (3) A spatial–spectral adaptation module that refines details across both domains in the decoding phase.
Extensive experiments on nine all-in-one HSI restoration benchmarks confirm HSI-VAR's state-of-the-art performance, achieving a 3.77 dB PSNR improvement on \textbf{\textit{ICVL}} and offering superior structure preservation with an inference speed-up of up to $95.5 \times$ compared with diffusion-based methods, making it a highly practical solution for real-world HSI restoration.
