# info-tutorato

Hands-on PyTorch and deep-learning notebooks that complement the history-and-theory lectures for economics students.

The course pairs theoretical PDF lectures with practical Jupyter notebooks. Notebooks are written to run out-of-the-box on **Google Colab** (which pre-installs PyTorch, NumPy, and matplotlib).

## Course contents

| #   | Material                                                             | Topic                                               |
| --- | -------------------------------------------------------------------- | --------------------------------------------------- |
| 0   | [`notebooks/0-torch-beginners.ipynb`](notebooks/0-torch-beginners.ipynb) | PyTorch from scratch: a thorough tensor tour |
| 1   | `lectures/1-1943.pdf`                                                | McCulloch–Pitts neurons (1943)                      |
| 2   | `lectures/2-1951-1969.pdf`                                           | Hebb, Rosenblatt's perceptron, the AI winter        |
| 3   | `lectures/3-architecture-and-training.pdf`                           | Multi-layer networks                                |
| 4   | `lectures/4-1847-1960-GD+SGD.pdf`                                    | Gradient descent and SGD                            |
| x   | `lectures/x-1986-2015-adam.pdf`                                      | Backpropagation, momentum, Adam                     |

## Running the notebooks

### On Google Colab (recommended for students)

1. Go to <https://colab.research.google.com>.
2. `File → Upload notebook` and select the `.ipynb` file from the `notebooks/` folder.
3. `Runtime → Run all`.

No installation needed — Colab ships with `torch`, `numpy`, and `matplotlib`.

### Locally with [uv](https://docs.astral.sh/uv/)

```bash
uv sync
uv run jupyter lab
```

### Locally with pip

```bash
python -m venv .venv
source .venv/bin/activate
pip install torch numpy matplotlib jupyter ipykernel
jupyter lab
```

Then open any notebook under `notebooks/` and run the cells.
