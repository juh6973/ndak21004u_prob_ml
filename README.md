# ndak21004u_prob_ml

## Setup

```bash
conda create -n ndak21004u python=3.12 -y
conda activate ndak21004u
pip install -r requirements.txt
python -m ipykernel install --user --name ndak21004u --display-name "Python (ndak21004u)"
```

Pick the `Python (ndak21004u)` kernel when opening the notebooks.

### Assignment 1: Bayesian linear regression

Run `assignment1/bayesian_linreg.ipynb` top to bottom (or `jupyter nbconvert --to notebook --execute --inplace assignment1/bayesian_linreg.ipynb`). It samples the toy datasets, computes the posterior over the weights and the posterior predictive, and saves the figures to `assignment1/figures/`.

### Assignment 1: VAE on MNIST

Run `assignment1/vae_mnist.ipynb` top to bottom. It downloads MNIST to `assignment1/data/`, trains a VAE with a 2D latent space (about 30 s on Apple MPS), plots the encoded test digits, and decodes a 15×15 grid of latent points. Figures are saved to `assignment1/figures/`. The device is picked automatically (cuda → mps → cpu); set `DEVICE=cpu` to override.
