# Signals & Systems — Weekly Coding Exercises

My work on the weekly coding problems for the Signals & Systems course. Each week has a short Jupyter notebook whose tasks go with that week's problem set: the concepts from the pen-and-paper problems are implemented in Python and checked with assert cells.

## Structure

```
Signals-Systems/
├── ex01/
│   ├── 01d_coding.ipynb                 # original exercise notebook
│   ├── 01d_coding_solutions.ipynb       # reference solutions
│   └── 01_coding_implementation.ipynb   # my implementation
└── README.md
```

Each week gets its own `exNN/` folder with the same layout.

## Weeks

| Week | Folder | Topics |
|------|--------|--------|
| 1 | [ex01](ex01/) | Discrete-time signals: shifting and time reversal with an explicit origin, impulse decomposition, testing systems for linearity and time invariance |

### Week 1 tasks

- **C1: Shift and reverse** (P3, P4): represent a signal as values plus an origin index, then implement `delay` for $x[n-k]$ and `reverse` for $x[-n]$, and plot the results as stem plots.
- **C2: Impulse decomposition** (P2): rebuild a signal as a sum of scaled, shifted impulses $\sum_k x[k]\,\delta[n-k]$ and check it against the directly defined signal.
- **C3: Linearity and time invariance** (P6, P10): write numerical tests using random inputs and apply them to $y[n] = u[n]\,s[n]$ (linear, not time-invariant) and $y[n] = u[n] + 1$ (time-invariant, not linear).

## Setup

You need Python 3 with NumPy, Matplotlib and Jupyter.

```bash
pip install numpy matplotlib jupyter
```

Open a notebook in VS Code or Jupyter and select a kernel that has these packages installed. Then run the cells from top to bottom. Each task ends with a check cell that prints a "passed" message when the implementation is correct.

## Working approach

Before running a check cell, predict its output on paper, as the notebooks suggest. Then try the problem in the exercise or implementation notebook before looking at the solutions.
