# ndak24002u_deep_learning

## Setup

```bash
pip install -r requirements.txt
```

### Weights & Biases

The MNIST notebook logs to W&B. Put your API key (from https://wandb.ai/authorize) in a `.env` file in the repository root:

```
WANDB_API_KEY=your-key-here
```

The notebook loads it with `python-dotenv`, so no `wandb login` is needed. `.env` is git-ignored, so each group member keeps their own key.

### Exercise 3: Deep vs wide networks

Run `assignment1/feedforwardAssignment.ipynb` top to bottom (or `jupyter nbconvert --to notebook --execute --inplace assignment1/feedforwardAssignment.ipynb`). Figures and the GIF are written to `assignment1/figures/`. The device is picked automatically (cuda → mps → cpu); set `DEVICE=cpu` to override.

### Exercise 4: MLOps (MNIST + W&B)

With the `.env` key in place, run `assignment1/MNISTfeedforwardAssignment.ipynb` top to bottom. It downloads MNIST to `assignment1/data/`, trains the 42-unit baseline, runs a 20-run W&B sweep (about 10 min on CPU), and saves `mnist_baseline.png` and `mnist_sweep.png` to `assignment1/figures/`. Use `DEVICE=cpu` to override the device.
