# FISTA for Linear Inverse Problems

## Overview

This project presents an implementation of the Fast Iterative
Shrinkage-Thresholding Algorithm (FISTA) for solving an
L1-regularized linear inverse problem.

The implementation also includes ISTA for comparison of
convergence performance.

## Problem Formulation

The optimization problem considered is:

minimize

    F(x) = 0.5 ||Ax - b||²₂ + λ||x||₁

## Algorithms

### ISTA
The Iterative Shrinkage-Thresholding Algorithm combines a
gradient-descent step with a soft-thresholding operation.

### FISTA
FISTA introduces an acceleration step to improve the convergence
behavior of ISTA.

## Implementation

The notebook includes:

- Soft-thresholding / proximal operator
- Objective-function calculation
- Lipschitz constant calculation
- ISTA implementation
- FISTA implementation
- Convergence checking
- Objective-value tracking
- Execution-time measurement
- ISTA vs FISTA comparison

## Experimental Results

The implemented experiment gives:

| Method | Final Objective |
|--------|-----------------:|
| ISTA   | 271.4532 |
| FISTA  | 140.6846 |

The notebook also records the convergence behavior and execution
time of the implemented algorithms. 1

## Tools & Libraries

- Python
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

## How to Run

1. Clone the repository.
2. Install the required libraries:

```bash
pip install -r requirements.txt
