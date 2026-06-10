This repository contains two sets of computational economics assignments: Monte Carlo simulations for clustered standard errors and numerical solution of the Cournot duopoly game.
File Descriptions

1. L3_Clustering_MonteCarlo.ipynb
Original baseline version
Implements Monte Carlo simulations to evaluate the performance of standard OLS standard errors vs. clustered standard errors
Computes rejection rates for hypothesis tests under different data generating processes (DGPs)
Provides foundational results for standard error comparison

2. L3_Clustering_MonteCarlo_work1.ipynb
Extended analysis version
Systematically varies the number of clusters in the DGP
Compares rejection rates across clustered standard errors and White robust (WB) standard errors
Investigates how cluster size affects the finite-sample performance of different standard error estimators

3. assignment06_cournot.ipynb
Cournot Duopoly Equilibrium Solver
Implements three numerical methods to solve the nonlinear system of first-order conditions:
Hand-coded Newton-Raphson method with Jacobian matrix
Fixed-point iteration method (direct iteration on best-response functions)
Built-in scipy.optimize.fsolve function for verification
Analyzes the impact of government subsidies on equilibrium quantities, prices, and firm profits
Includes convergence analysis and sensitivity checks
