# Signals & Systems — Weekly Coding Exercises

My work on the weekly coding problems for the Signals & Systems course. Each week has a short Jupyter notebook whose tasks go with that week's problem set: the concepts from the pen-and-paper problems are implemented in Python and checked with assert cells.

## Structure

```
Signals-Systems/
├── ex01/
│   ├── 01d_coding.ipynb                  # original exercise notebook
│   ├── 01d_coding_solutions.ipynb        # reference solutions
│   └── 01_coding_implementation.ipynb    # my implementation
├── ex02/
│   ├── 02d_coding.ipynb
│   ├── 02d_coding_solutions.ipynb
│   └── 02d_coding_implementation.ipynb
├── ex03/
│   ├── 03d_coding.ipynb
│   ├── 03d_coding_solutions.ipynb
│   └── 03d_coding_implementation.ipynb
├── ex04/
│   ├── 04d_coding.ipynb
│   ├── 04d_coding_solutions.ipynb
│   └── 04d_coding_implementation.ipynb
└── README.md
```

Each week gets its own `exNN/` folder with the same layout.

## Weeks

| Week | Folder | Topics |
|------|--------|--------|
| 1 | [ex01](ex01/) | Discrete-time signals: shifting and time reversal with an explicit origin, impulse decomposition, testing systems for linearity and time invariance |
| 2 | [ex02](ex02/) | Convolution from scratch vs. `np.convolve`, step response and causality of FIR systems, BIBO stability via partial sums of \|h[k]\|, single (FIR) vs. feedback (IIR) echo |
| 3 | [ex03](ex03/) | State-space realizations: simulating $(A,B,C,D)$ and extracting the impulse response, $h[n]=CA^{n-1}B$ with matrices and invariance under a change of state coordinates, linearization of a nonlinear tank around an equilibrium |
| 4 | [ex04](ex04/) | Discretization: forward Euler vs. exact discretization via the matrix exponential of an augmented matrix, stability of Euler across the step-size threshold $T_s = 2/\|a\|$, reconstruction error of the zero-order hold |

## Setup

You need Python 3 with NumPy, Matplotlib and Jupyter.

```bash
pip install numpy matplotlib jupyter
```

Open a notebook in VS Code or Jupyter and select a kernel that has these packages installed. Then run the cells from top to bottom. Each task ends with a check cell that prints a "passed" message when the implementation is correct.

## Working approach

Before running a check cell, predict its output on paper, as the notebooks suggest. Then try the problem in the exercise or implementation notebook before looking at the solutions.
