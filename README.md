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

Run `assignment1/programming_exercises.ipynb` top to bottom (or `jupyter nbconvert --to notebook --execute --inplace assignment1/programming_exercises.ipynb`). It samples the toy datasets, computes the posterior over the weights and the posterior predictive, and saves the figures to `assignment1/figures/`.
