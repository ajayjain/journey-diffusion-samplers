# Journey to the BAOAB-limit: finding effective MCMC samplers for score-based models

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17kesyBVqubV_Zzchf2XoR-7MHk5jxTuo?usp=sharing)

This repository will have code to reproduce CIFAR10 experiments for the paper "Journey to the BAOAB-limit: finding effective MCMC samplers for score-based models". Find videos and a Colab notebook for text-to-image sampling at https://ajayj.com/journey. Our full code is coming soon!

## Abstract
Diffusion and score-based generative models have achieved remarkable sample quality on difficult image synthesis tasks. Many works have proposed samplers for pretrained diffusion models, including ancestral samplers, SDE and ODE integrators and annealed MCMC approaches. So far, the best sample quality has been achieved with samplers that use time-conditional score functions and move between several noise levels. However, estimating an accurate score function at many noise levels can be challenging and requires an architecture that is more expressive than would be needed for a single noise level. In this work, we explore MCMC sampling algorithms that operate at a single noise level, yet synthesize images with acceptable sample quality on the CIFAR-10 dataset. We show that while näive application of Langevin dynamics and a related noise-denoise sampler produces poor samples, methods built on integrators of underdamped Langevin dynamics using splitting methods can perform well. Further, by combining MCMC methods with existing multiscale samplers, we begin to approach competitive sample quality without using scores at large noise levels.

## Citation

```
@article{jain2022journey,
  author = {Jain, Ajay and Poole, Ben},
  title = {Journey to the BAOAB-limit: finding effective MCMC samplers for score-based models},
  journal = {Workshop on Score-Based Methods at NeurIPS},
  year = {2022},
}
```
