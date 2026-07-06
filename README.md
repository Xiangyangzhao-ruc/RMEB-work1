# RMEB-work1

## Assignments
This repository contains computational economics assignments for the RMEB course, including three main components: Monte Carlo simulations for clustered standard errors, numerical solution of the Cournot duopoly game, and the final assignment with complete replication materials.

### `final assignment/`
Final course empirical replication assignment, built on the classic paper from *Quarterly Journal of Economics* about no-fault divorce reform and divorce rates in the United States (Friedberg, 1998). This folder delivers a fully reproducible research workflow with three core components:
- `assignment01_final_version.ipynb`: Executable Jupyter notebook with the complete empirical analysis pipeline, including data cleaning and preprocessing, two-way fixed effects model estimation, robustness checks, and heterogeneity analysis. It replicates all core regression results and key figures from the original study, and can be run sequentially to generate full empirical outputs.
- `Report.pdf`: Formal replication report. It systematically covers the research background and literature basis, empirical identification strategy and econometric specification, data source and variable definitions, comparison between replicated results and original findings, as well as extended analysis and discussion.
- `DivorceData(QJE).zip`: Raw dataset package. It contains state-level panel data on divorce rates and corresponding socioeconomic variables across the United States, which is exactly the core data used in the original QJE paper and supports full replication of the entire analysis.

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
