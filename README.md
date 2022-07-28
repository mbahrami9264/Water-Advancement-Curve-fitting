# Water-Advancement-Curve-fitting
This script uses the pyomo optimization library and ipopt solver to fit water advancement data based on the Y = X ^ r equation. This equation is used to model the advancement of water in border irrigation. X represents advancement time (min) and Y represents advancement length (m).
We suggest using Anaconda and Jupyter notebook
Instructions on how to install pyomo and ipopt solver are available at:
https://anaconda.org/conda-forge/pyomo
https://anaconda.org/conda-forge/ipopt

The data used for curve fitting was saved in the .dat format. An example data file can be find in the repository.

The optimization model was written in Python 3.10.4. For modelling and solving optimization problems, the Python Optimization Modeling Objects (Pyomo) library version 6.4.1 was used. Pyomo is an open-source package that was developed by Hart et al. (2011). Pyomo is used for mathematical modelling of optimization problem within Python. Abstract models are defined with their objective functions, constraints and boundaries, which will be communicated to a solver software package. Pyomo supports a wide range of problem types such as linear and nonlinear programming (Hart et al. 2017).
Since the curve fitting problem we wanted to solve is a nonlinear function, Interior Point OPTimizer (IPOPT) solver was used to find the optimal value of r. IPOPT is a nonlinear solver for continuous systems, developed by Wächter and Biegler (2006). IPOPT finds a local solution of the nonlinear model using an interior point line search filter method. The Python script for curve fitting was developed in a Jupyter Notebook using Anaconda.

# References
Wächter, A., & Biegler, L. T. (2006). On the implementation of an interior-point filter line-search algorithm for large-scale nonlinear programming. Mathematical programming, 106(1), 25-57.
Hart, W. E., Watson, J. P., & Woodruff, D. L. (2011). Pyomo: modeling and solving mathematical programs in Python. Mathematical Programming Computation, 3(3), 219-260.
Hart, W. E., Laird, C. D., Watson, J. P., Woodruff, D. L., Hackebeil, G. A., Nicholson, B. L., & Siirola, J. D. (2017). Pyomo-optimization modeling in python (Vol. 67, p. 277). Berlin: Springer.
