# Joint Learning of Pose Regression and Denoising Diffusion with Score Scaling Sampling for Category-level 6D Pose Estimation

**ICCV 2025**

[Seunghyun Lee](https://github.com/sseunghyun) · [Tae-Kyun Kim](https://sites.google.com/view/tkkim/home)

Korea Advanced Institute of Science and Technology (KAIST)

[![Paper](https://img.shields.io/badge/Paper-arXiv-green)](https://arxiv.org/abs/2510.04125)
[![ICCV 2025](https://img.shields.io/badge/ICCV-2025-blue)](https://openaccess.thecvf.com/content/ICCV2025/html/Lee_Joint_Learning_of_Pose_Regression_and_Denoising_Diffusion_with_Score_ICCV_2025_paper.html)

---

## Overview

> **TL;DR:** We propose a joint learning strategy combining direct pose regression with diffusion score matching, along with a time-dependent score scaling guidance, achieving state-of-the-art category-level 6D pose estimation with single-sample inference — no additional evaluation network required.

This repository is the official PyTorch implementation of our ICCV 2025 paper. Our work builds upon [GenPose](https://github.com/Jiyao06/GenPose) (NeurIPS 2023).

**Key contributions:**
- **Joint Learning**: Pre-trains the encoder with direct pose regression, then jointly trains with the diffusion denoising head — significantly accelerating training convergence (~1.5× speedup) while improving accuracy.
- **Score Scaling Guidance**: A time-dependent exponential score scaling strategy that guides samples toward high-density regions, enabling reliable single-sample inference without any additional pose evaluation network.

---

## Citation

If you find our work useful in your research, please consider citing:

```bibtex
@InProceedings{Lee_2025_ICCV,
  author    = {Lee, Seunghyun and Kim, Tae-Kyun},
  title     = {Joint Learning of Pose Regression and Denoising Diffusion with Score Scaling Sampling for Category-level 6D Pose Estimation},
  booktitle = {Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV)}, 
  month     = {October},
  year      = {2025},
  pages     = {5757-5768}
}
```

---

## Code

Code will be released soon.

---

## Acknowledgements

This work builds upon [GenPose](https://github.com/Jiyao06/GenPose). We thank the authors for their excellent work and open-source implementation.

This work was supported by NST grant (CRC 21011, MSIT), IITP grant (RS-2023-00228996, RS-2024-00459749, RS-2025-25443318, RS-2025-25441313, MSIT) and KOCCA grant (RS-2024-00442308, MCST).
