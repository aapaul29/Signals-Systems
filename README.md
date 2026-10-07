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


## Setup

You need Python 3 with NumPy, Matplotlib and Jupyter.

```bash
pip install numpy matplotlib jupyter
```

Open a notebook in VS Code or Jupyter and select a kernel that has these packages installed. Then run the cells from top to bottom. Each task ends with a check cell that prints a "passed" message when the implementation is correct.

## Working approach

Before running a check cell, predict its output on paper, as the notebooks suggest. Then try the problem in the exercise or implementation notebook before looking at the solutions.
