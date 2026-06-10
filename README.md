# Assignments

This repository contains two sets of computational economics assignments: Monte Carlo simulations for clustered standard errors and numerical solution of the Cournot duopoly game.

---

## File Descriptions

### `L3_Clustering_MonteCarlo.ipynb`
**Original baseline version**
- Implements Monte Carlo simulations to compare standard OLS standard errors and clustered standard errors
- Computes hypothesis test rejection rates under different data generating processes (DGPs)
- Provides the benchmark results for all subsequent standard error analyses

### `L3_Clustering_MonteCarlo_work1.ipynb`
**Extended cluster size analysis**
- Systematically varies the number of clusters in the simulation DGP
- Quantifies and compares rejection rates between clustered standard errors and White robust (WB) standard errors
- Evaluates how cluster count affects the finite-sample performance of different standard error estimators

### `assignment06_cournot.ipynb`
**Cournot Duopoly Equilibrium Solver**
- Implements three numerical methods to solve the nonlinear first-order conditions:
  - Hand-coded Newton-Raphson method with analytical Jacobian matrix
  - Fixed-point iteration on best-response functions
  - `scipy.optimize.fsolve` for result verification
- Analyzes the impact of government production subsidies on equilibrium quantities, prices and firm profits
- Includes convergence analysis and parameter sensitivity checks

---

## How to Run
1. Install required dependencies
2. Launch Jupyter Notebook
3. Open any `.ipynb` file and run all cells sequentially

## Dependencies
- `numpy`
- `scipy`
- `matplotlib`
- `jupyter`

## License
MIT License
