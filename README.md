[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/xcarl1/Awesome-Self-Supervised-Micro-Image-Denoise/graphs/commit-activity)
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/xcarl1/Awesome-Self-Supervised-Micro-Image-Denoise)
<img alt="GitHub watchers" src="https://img.shields.io/github/watchers/xcarl1/Awesome-Self-Supervised-Micro-Image-Denoise?style=social"> <img alt="GitHub stars" src="https://img.shields.io/github/stars/xcarl1/Awesome-Self-Supervised-Micro-Image-Denoise?style=social"> <img alt="GitHub forks" src="https://img.shields.io/github/forks/xcarl1/Awesome-Self-Supervised-Micro-Image-Denoise?style=social">

# Awesome Self-Supervised Micro-Image Denoise

A curated list of self-supervised denoising methods for microscopy imaging. We categorize existing methods into four distinct classes based on their underlying assumptions and sampling strategies.

## 📖 Taxonomy

We organize all current microscopic self-supervised methods into the following four categories:

1.  **Blind-Spot Frame Based**
    * *Mechanism*: Masks pixels in the center frame (or removes the frame entirely) and predicts them using unmasked pixels from the same frame or adjacent frames.

2.  **Blind-Spot Convolution Based**
    * *Mechanism*: Modifies the network structure (e.g., masked convolution) so that the prediction for a specific pixel depends only on its spatial neighbors, excluding the pixel itself.

3.  **Neighboring Frame Based**
    * *Mechanism*: Predicts even frames using odd frames (or vice versa), assuming high temporal similarity between adjacent frames.

4.  **Spatial Sampling Based**
    * *Mechanism*: Exploits spatial redundancy, assuming high similarity between neighboring pixels (e.g., via subsampling).

---

## 1. Blind-Spot Frame Based
> **Core Idea:** Temporal masking and prediction.

- **DeepInterpolation: Removing independent noise in systems neuroscience data using DeepInterpolation**
  - *Nature Methods 2021*
  - [[Paper](https://www.nature.com/articles/s41592-021-01285-2)] [[Code](https://github.com/AllenInstitute/deepinterpolation)]

- **DeepVID: High-speed low-light in vivo two-photon voltage imaging of large neuronal populations**
  - *Nature Methods 2023*
  - [[Paper](https://www.nature.com/articles/s41592-023-01820-3)] [[Code](https://github.com/bu-cisl/DeepVID)]

- **DeepVID v2: Self-supervised denoising with decoupled spatiotemporal enhancement for low-photon voltage imaging**
  - *bioRxiv 2024*
  - [[Paper](https://www.biorxiv.org/content/10.1101/2024.05.16.594448)] [[Code](https://github.com/bu-cisl/DeepVIDv2)]

- **TeD: Self-supervised denoising of dynamic fluorescence images via temporal gradient-empowered deep learning**
  - *Photonix 2025*
  - [[Paper](https://www.photonix.cn/en/article/doi/10.1186/s43074-025-00173-8)]

## 2. Blind-Spot Convolution Based
> **Core Idea:** Structural masking (BS-Conv).

- **DeepSeMi: Bio-friendly long-term subcellular dynamic recording by self-supervised image enhancement microscopy**
  - *Nature Methods 2023*
  - [[Paper](https://www.nature.com/articles/s41592-023-02058-9)] [[Code](https://github.com/GuoxunZhang-THU/DeepSeMi)]

- **SUPPORT: Statistically unbiased prediction enables accurate denoising of voltage imaging data**
  - *Nature Methods 2023*
  - [[Paper](https://www.nature.com/articles/s41592-023-02005-8)] [[Code](https://github.com/NICALab/SUPPORT)]

## 3. Neighboring Frame Based
> **Core Idea:** Frame interpolation / Odd-Even prediction.

- **DeepCAD: Real-time denoising enables high-sensitivity fluorescence time-lapse imaging beyond the shot-noise limit**
  - *Nature Methods 2021*
  - [[Paper](https://www.nature.com/articles/s41592-021-01225-0)] [[Code](https://github.com/cabooster/DeepCAD)]

- **DeepCAD-RT: Real-time denoising enables high-sensitivity fluorescence time-lapse imaging beyond the shot-noise limit**
  - *Nature Biotechnology 2023*
  - [[Paper](https://www.nature.com/articles/s41587-022-01450-8)] [[Code](https://github.com/cabooster/DeepCAD-RT?tab=readme-ov-file)]

## 4. Spatial Sampling Based
> **Core Idea:** Spatial redundancy / Subsampling.

- **FAST: Real-time self-supervised denoising for highspeed fluorescence neural imaging**
  - *Nature Communications 2025*
  - [[Paper](https://www.nature.com/articles/s41467-025-64681-8)] [[Code](https://github.com/FDU-donglab/FAST)]

- **SN2N: Self-inspired learning for denoising live-cell super-resolution**
  - *Nature Methods 2024*
  - [[Paper](https://www.nature.com/articles/s41592-024-02400-9)] [[Code](https://github.com/WeisongZhao/SN2N/)]

- **SDRTrans: Spatial redundancy transformer for self-supervised fluorescence image denoising**
  - *Nature Computational Science 2023*
  - [[Paper](https://www.nature.com/articles/s43588-023-00568-2)] [[Code](https://github.com/cabooster/SRDTrans)]

---

## Contribution

Feel free to create a pull request or open an issue to add new papers or fix existing entries.
