<p align="center">

  <h1 align="center">Accelerating Score-based Generative Models for High-Resolution Image Synthesis</h1>
  <p align="center">
    <a href="">Hengyuan Ma</a>
    ·
    <a href="http://www.robots.ox.ac.uk/~lz/">Li Zhang</a>
    ·
    <a href="https://xiatian-zhu.github.io">Xiatian Zhu</a>
    ·
    <a href="https://zjfheart.github.io/">Jingfeng Zhang</a>
    ·
    <a href="https://www.dcs.warwick.ac.uk/~feng/">Jianfeng Feng</a>

  </p>
  <h3 align="center"><a href="">Paper</a> | <a href="https://github.com/fudan-zvg/TDAS">Project Page</a></h3>
  <div align="center"></div>
  </p>

<p align="center">
  <a href="">
    <img src="./image/demo.pdf" alt="Logo" width="95%">
  </a>
</p>

<p align="center">
Score-based generative models (SGMs) have recently emerged as a promising class of generative models. The key idea is to produce high-quality images by recurrently adding Gaussian noises and gradients to a Gaussian sample until converging to the target distribution, a.k.a.  the diffusion sampling. To ensure stability of convergence in sampling and generation quality, however, this sequential sampling process has to take a small step size and many sampling iterations (e.g., 2000). Several acceleration methods have been proposed with focus on low-resolution generation. In this work, we consider the acceleration of high-resolution generation with SGMs, a more challenging yet more important problem. We prove theoretically that this slow convergence drawback is primarily due to the ignorance of the target distribution. Further, we introduce a novel Target Distribution Aware Sampling (TDAS) method by leveraging the structural priors in space and frequency domains. Extensive experiments on CIFAR-10, CelebA, LSUN, and FFHQ datasets validate that TDAS can consistently accelerate state-of-the-art SGMs, particularly on more challenging high resolution 1024x1024 image generation tasks by up to 18.4x, whilst largely maintaining the synthesis quality. With fewer sampling iterations, TDAS can still generate good quality images. In contrast, the existing methods degrade drastically or even fails completely. 
</p>


If you find our paper useful, please cite
```bibtex
@article{Ma2022AccelerateSGM,
  author    = {Ma, Hengyuan and Zhang, Li and Zhu, Xiatian and Zhang, Jingfeng and Feng, Jianfeng},
  title     = {Accelerating Score-based Generative Models for High-Resolution Image Synthesis},
  journal   = {arXiv prepreint},
  year      = {2022},
}
```