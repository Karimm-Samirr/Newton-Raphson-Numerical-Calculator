# Newton–Raphson Method — Numerical Root Finding Calculator

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/YOUR_REPO_NAME/blob/main/Newton_Raphson_Calculator.ipynb)

**Course:** Differential Equations and Numerical Analysis

## Overview
An interactive Python calculator implementing the **Newton–Raphson numerical method** to approximate roots of non-linear equations $f(x) = 0$. The notebook automatically computes symbolic derivatives using `SymPy`, evaluates convergence conditions, generates step-by-step iteration tables, and plots the function alongside its tangent lines.

## Features
- **Automatic Differentiation:** Computes $f'(x)$ and $f''(x)$ symbolically via `SymPy`.
- **Convergence Check:** Evaluates the theoretical convergence condition $\left|\frac{f(x)f''(x)}{[f'(x)]^2}\right| < 1$ at $x_0$ and the final approximation.
- **Error & Edge-Case Handling:** Detects division by zero ($f'(x_i) \approx 0$), undefined domain values, and divergence.
- **Visualization:** Plots $f(x)$, initial guess $x_0$, iteration points, tangent lines, and the final root using `Matplotlib`.
- **Built-in Validation:** Tested against known analytical and numerical roots ($x^2 - 4$, $x^3 - x - 2$, and $\cos(x) - x$).

## How to Run
1. Click the **Open in Colab** badge at the top of this page.
2. In Colab, select **Runtime → Run all** from the top menu.
3. Modify the input parameters (`function_text`, `x0_text`, `tol_text`, `max_iter_text`) in **Section 5** to solve custom equations.