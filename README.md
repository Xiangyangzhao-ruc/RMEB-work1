# RMEB-work1

## Assignments
This repository contains computational economics assignments for the RMEB course, including three main components: Monte Carlo simulations for clustered standard errors, numerical solution of the Cournot duopoly game, and the final assignment with complete replication materials.

## File Descriptions
`final assignment/`
Final course assignment with full reproducible materials
- Contains the executable Jupyter notebook for core empirical analysis and computational tasks
- Includes the complete replication report detailing methodology, empirical results and discussion
- Attaches raw original datasets to support full replication of the assignment

`L3_Clustering_MonteCarlo.ipynb`
- Original baseline version
- Implements Monte Carlo simulations to compare standard OLS standard errors and clustered standard errors
- Computes hypothesis test rejection rates under different data generating processes (DGPs)
- Provides the benchmark results for all subsequent standard error analyses

`L3_Clustering_MonteCarlo_work 1.ipynb`
- Extended cluster size analysis
- Systematically varies the number of clusters in the simulation DGP
- Quantifies and compares rejection rates between clustered standard errors and White robust (WB) standard errors
- Evaluates how cluster count affects the finite-sample performance of different standard error estimators

`assignment06_cournot.ipynb`
- Cournot Duopoly Equilibrium Solver
- Implements three numerical methods to solve the nonlinear first-order conditions:
  - Hand-coded Newton-Raphson method with analytical Jacobian matrix
  - Fixed-point iteration on best-response functions
  - `scipy.optimize.fsolve` for result verification
- Analyzes the impact of government production subsidies on equilibrium quantities, prices and firm profits
- Includes convergence analysis and parameter sensitivity checks

## How to Run
1. Install required dependencies
2. Launch Jupyter Notebook
3. Open any `.ipynb` file and run all cells sequentially

## License
MIT License
