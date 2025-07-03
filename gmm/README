# Gaussian Mixture Model

## Installation
To install an environment for running the GMM code, start by creating a virtual environment with Python 3.12, e.g., using conda as 
```
conda create -n ddsmc python=3.12
```
Activate the environment and then install the requirements and the ddsmc package with pip
```
pip install -r requirements.txt
pip install -e .
```

## Usage
Code for the Gaussian mixture model (GMM) experiments can be found in `toy_data/`. A minimal example for running an experiment is (after navigating to `toy_data/`)
```
python toy_gaussian.py --algo ALGO --num_samples NUM_SAMPLES --dim_x DIM_X --dim_y DIM_Y --num_steps NUM_STEPS
```
where `ALGO` is your preferred algo: `ddsmc, tds, mcgdiff, ddrm, dcps, or daps` (not case-sensitive). The different algorithms might also have some (optional) arguments. Run `python toy_gaussian.py -h` or see the source code for information on arguments. **Note that some arguments have defaults and no warnings will be displayed if not explicitly setting an argument with a default.**

## LICENSE
The script `toy_gaussian.py` was modified from the [MCGDiff repository](https://github.com/gabrielvc/mcg_diff/blob/1a3cdd22c971ca13ce06a48eaaa00d2a6602b5c1/scripts/viz_gaussian.py). The original work is under a GPL 3.0 License, and hence the modifications are also under this license, which can be found in [LICENSE](LICENSE).