# DenseAR

### Next-Dense-Stride Prediction for Multimodal Autoregressive Visual Modeling

Chicago Y. Park<sup>1,*</sup>, Jialin Mao<sup>2</sup>, Xiaojian Xu<sup>2</sup>, Taha Kass-Hout<sup>2</sup>, Ulugbek S. Kamilov<sup>1</sup>, Cao Xiao<sup>2</sup>

<sup>1</sup>University of Wisconsin–Madison &nbsp;&nbsp; <sup>2</sup>GE HealthCare

<sup>*</sup>This work was done during an internship at GE HealthCare.

[**Paper (arXiv)**](https://arxiv.org/abs/2607.09892) · [**Project Page**](https://uw-cig.github.io/densear_page/)

---

## 🚧 Code — Coming Soon

The full training and inference code for **DenseAR** is being cleaned up for release and will be published in this repository. **Star ⭐ / watch 👀 this repo** to be notified when it lands.

---

## Overview

**DenseAR** reformulates autoregressive image generation as coarse-to-fine **next-dense-stride prediction** on a compact single-scale latent grid. Traversing the grid with progressively denser strides captures the transition from global structure to fine detail — avoiding both the slow inference of raster-order autoregression (DenseAR decodes multiple tokens in parallel) and the long multi-resolution sequences of multi-scale approaches.

On brain MRI, a single DenseAR model unifies cross-modal translation, modality-conditioned generation, and tumor segmentation. On natural images, DenseAR improves class-conditional ImageNet generation over single-grid and multi-scale-tokenizer baselines.

### Highlights

- **Next-dense-stride prediction** — coarse-to-fine generation on a compact single-scale latent grid.
- **Fast** — decodes multiple tokens per step in parallel, avoiding slow raster-order autoregression.
- **Compact** — no long multi-resolution token sequences as in multi-scale (VAR) models.
- **Unified** — one backbone for MRI cross-modal translation, modality-conditioned generation, and tumor segmentation.
- **Strong** — comparable to task-specific methods on brain MRI and improved class-conditional ImageNet (FID/IS) over single-grid and multi-scale baselines.

## Release Checklist

- [ ] Training code
- [ ] Inference / sampling code
- [ ] Pretrained checkpoints
- [ ] Data preprocessing scripts

## Citation

If you find this work useful, please consider citing:

```bibtex
@article{park2026DenseAR,
  title   = {Next-Dense-Stride Prediction for Multimodal Autoregressive Visual Modeling},
  author  = {Park, Chicago Y. and Mao, Jialin and Xu, Xiaojian and Kass-Hout, Taha and Kamilov, Ulugbek S. and Xiao, Cao},
  journal = {arXiv:2607.09892},
  year    = {2026}
}
```

## Contact

For questions, please reach out to Chicago Y. Park (`chicago.park@wisc.edu`).
