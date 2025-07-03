# DDSMC Image experiments
We ran the image experiments by integrating DDSMC in the [DCPS code base](https://github.com/Badr-MOUFAD/dcps/). Therfore, we have here provided necessary code for doing this integration. So, to run DDSMC on images, you in priniciple need to do the following:
1. Clone and follow the instructions to install the DCPS codebase from <https://github.com/Badr-MOUFAD/dcps/>. 
1. Copy `../ddsmc` into `[DCPS directory]/src`.
1. Download the file `precond.py` from the [DAPS repository](https://github.com/zhangbingliang2019/DAPS/blob/legacy/model/precond.py) and add to `[DCPS directory]/src/ddsmc/ddsmc_image_utils`
1. Copy the required code in `posterior_samplers/cond_sampling_algos.py` to `[DCPS directory]/posterior_samplers/cond_sampling_algos.py`
1. Add an import of `ddsmc` from `posterior_samplers.cond_sampling_algos` in `[DCPS directory/demo_imges.py]`
1. Copy the imports, the additional arguments in Config, and the elif-statement in `[This directory]/demo_imges.py` into `[DCPS directory/demo_imges.py]`
1. Copy the configs into `[DCPS directory]/configs`

Now, you should be able to run DDSMC from within the DCPS codebase. NOTE: we here additionally provide the script `make_masks.py` which can be run in the DCPS directory to create the linear operators.

If using the DCPS codebase, please consider citing DCPS:
```
@inproceedings{
    janati2024divideandconquer,
    title={Divide-and-Conquer Posterior Sampling for Denoising Diffusion priors},
    author={Yazid Janati and Badr MOUFAD and Alain Oliviero Durmus and Eric Moulines and Jimmy Olsson},
    booktitle={The Thirty-eighth Annual Conference on Neural Information Processing Systems},
    year={2024},
    url={https://openreview.net/forum?id=BOrut7M2X7}
}
```