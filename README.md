# DiffusionUavLoc: Visually Prompted Diffusion for Cross-View UAV Localization

This repository contains the PyTorch implementation of the method proposed in the paper "DiffusionUavLoc: Visually Prompted Diffusion for Cross-View UAV Localization". The proposed framework addresses the challenge of cross-view UAV localization by combining geometry-driven image prompting and text-free diffusion models.

The code will be made publicly available after the paper review process is completed. We will upload it as soon as possible.

## Overview

DiffusionUavLoc is designed to handle the task of cross-view UAV localization, where UAV images (oblique perspectives) are matched against satellite images (near-nadir perspectives). The core idea of the method is to use a **text-free conditional diffusion model** that utilizes structural priors (e.g., edges, depth, semantic masks) to guide the synthesis of high-quality pseudo-satellite images. This enables efficient and stable retrieval-based localization without relying on textual descriptions or large-scale labeled data.

### Key Features:

* **Text-free conditional diffusion model**: Replaces textual prompts with visually derived image prompts for cross-view localization.
* **Geometric-prior orthophoto rendering**: Utilizes UAV imagery for rendering near-nadir pseudo-satellite images.
* **Structure-guided feature extraction**: Enhances feature extraction using multi-modal structural cues (e.g., edges, semantic masks, depth).
* **Unified retrieval**: Uses latent-space descriptors for efficient retrieval and matching.

### Datasets Used:

* **University-1652**: A multi-view dataset of 1,652 university buildings worldwide, supporting UAV-view target localization and navigation.
* **SUES-200**: A dataset for cross-view image matching with varying UAV altitudes, providing comprehensive localization data.

## Citation

If you use DiffusionUavLoc in your research, please cite our paper:

```
@article{liu2026diffusionuavloc,
  title={DiffusionUavLoc: Visually Prompted Diffusion for Cross-View UAV Localization},
  author={Liu, Tao and Ren, Kan and Chen, Qian},
  journal={IEEE Internet of Things Journal},
  year={2026},
  publisher={IEEE}
}
```

## Future Work

* **Weakly supervised end-to-end training**: To reduce dependency on manual annotations.
* **Cross-domain robustness**: Investigate better generalization methods across different seasons and cities.

