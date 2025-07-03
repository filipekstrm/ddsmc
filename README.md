# Decoupled Diffusion Sequential Monte Carlo
This repository is the official repository for the ICML 2025 paper [Solving Linear-Gaussian Bayesian Inverse Problems with Decoupled Diffusion Sequential Monte Carlo](https://arxiv.org/abs/2502.06379) by [Filip Ekström Kelvinius](https://filipekstrm.github.io/), [Zheng Zhao](https://zz.zabemon.com/), and [Fredrik Lindsten](https://lindsten.netlify.app/). See [Citation](#citation) for how to cite this work.

**_CURRENT STATUS:_**  The code currently only supports the GMM experiments and image experiments. We are working on providing clean code for the protein and binary MNIST experiments. Contact Filip in case you are interested in those experiments.

## Abstract DDSMC class
The directory [`ddsmc`](ddsmc) contains code for the general implementation of DDSMC. If you would like to implement DDSMC for your particular data type, you can implement a new class that inherits the DDSMC class in [`ddsmc/ddsmc_sampler.py`](ddsmc/ddsmc_sampler.py), and which then implements the abstract functions.

## Installation and usage
See the respective READMEs for information on how to install and run the corresponding experiments
## Citation
If using DDSMC, please cite our paper
```
@inproceedings{
      kelvinius2025solving,
      title={Solving Linear-Gaussian Bayesian Inverse Problems with Decoupled Diffusion Sequential Monte Carlo},
      author={Filip Ekstr{\"o}m Kelvinius and Zheng Zhao and Fredrik Lindsten},
      booktitle={Forty-second International Conference on Machine Learning},
      year={2025},
      url={https://openreview.net/forum?id=QRNpmG8XGd}
}
```

Remeber also to cite any other algorithms that you have used in the GMM experiment (see their corresponding README in `toy_data/[ALGORITHM]/README.md`), and to cite DCPS if you have been using the image experiments code (see [image README](image/README)).

## License
Code for the different implementations have sometimes been obtained and potentially modified from public repositories, and their licensing might therefore differ. Please read the corresponding README for whatever code you are using. We are thankful to all authors which made their code publicly available.