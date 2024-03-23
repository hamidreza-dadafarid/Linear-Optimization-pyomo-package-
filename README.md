# Linear Optimization (implemented with pyomo package)
This repo consists of some linear optimization problems that are implemented with a python package called pyomo (Python Optimization Modeling Objects) which is an AML (Algebric Modeling Language).
AMLs provide the ability to express optimization models with a high-level programming language, which is very important because without it, if we want to solve an optimization model with a specific solver, we have to express that model in a format that is acceptable for that solver and give it as an input to the solver, while writing the model with the solver format is difficult and time-consuming, especially for large-scale problems. In addition, different solvers sometimes use different formats for input, and if we want to use several different solvers in solving our model with to compare each other, it is necessary to prepare the input of each salver separately.
Commercial AMLs such as AIMMS, AMPL and GAMS provide the ability to express optimization models with a high-level programming language, but pyomo provides this ability through the Python programming language, which is a widely used programming language with many libraries and is capable
Although a number of packages such as PuLP, APLEpy, Openopt also provide the possibility of writing optimization models in Python. But each of these has the ability to model and solve a specific group of optimization problems, while pyomo has the ability to implement different types of optimization models, including:

* Linear programming
* Mixed integer linear programming
* Nonlinear programming
* Mixed integer nonlinear programming
* Mathematical programs with equilibrium constraint
* Generalized disjunctive programs
* Bi-level programs
* Stochastic programs
* Dynamic problems with differential algebraic equations

Pyomo does not solve the optimization models, but creates the appropriate input for the solvers and leaves the solving process to the solvers, and then reports the answer that the solver returns. It is possible to communicate with different servers in pyomo, although these servers must be installed first and activated if a license is needed. GLPK is an open source solver that can solve LP and MILP problems, and IPOPT is also used to solve nonlinear problems.
The following sites provide comprehensive information about the pyomo library:

[Pyomo website](http://www.pyomo.org)

[Pyomo’s open source software](https://github.com/Pyomo/pyomo)

https://pyomo.readthedocs.io/en/stable/working_models.html

## package installation:
If you use `jupyter notebook`, run this command in `conda prompt`:
```
conda install pyomo 
```
Aslo run this command to install `glpk solver`:
```
conda install –c conda-forge glpk
```
[If you use Google Colab, click on this link to see the installation guide of pyomo package and different solver](https://colab.research.google.com/github/jckantor/ND-Pyomo-Cookbook/blob/master/notebooks/01.02-Running-Pyomo-on-Google-Colab.ipynb#scrollTo=yTGBrqQO3vT2)
