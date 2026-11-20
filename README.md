# ndak24002u_deep_learning

## Setup

```bash
pip install -r requirements.txt
```

### Weights & Biases

The MNIST notebook logs to W&B. Authenticate once per machine:

```bash
wandb login
```

To run without an account or network access, set `WANDB_MODE=offline` (runs are stored locally and can be synced later with `wandb sync`).

### Exercise 3: Deep vs wide networks

Run `assignment1/feedforwardAssignment.ipynb` top to bottom (or `jupyter nbconvert --to notebook --execute --inplace assignment1/feedforwardAssignment.ipynb`). Figures and the GIF are written to `assignment1/figures/`. The device is picked automatically (cuda → mps → cpu); set `DEVICE=cpu` to override.
