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
