# Linear Optimization (implemented with pyomo package)
This repo consists of some linear optimization problems that are implemented with a python package called pyomo (Python Optimization Modeling Objects) which is an AML (Algebric Modeling Language).
AMLs provide the ability to express optimization models with a high-level programming language, which is very important because without it, if we want to solve an optimization model with a specific solver, we have to express that model in a format that is acceptable for that solver and give it as an input to the solver, while writing the model with the solver format is difficult and time-consuming, especially for large-scale problems. In addition, different solvers sometimes use different formats for input, and if we want to use several different solvers in solving our model with to compare each other, it is necessary to prepare the input of each salver separately.
## package installation:
If you use `jupyter notebook`, run this command in `conda prompt`:
```
conda install pyomo 
```
aslo run this command to install `glpk` solver:
```
conda install –c conda-forge glpk
```
[If you use Google Colab, click on this link to see the installation guide of pyomo package and different solver](https://colab.research.google.com/github/jckantor/ND-Pyomo-Cookbook/blob/master/notebooks/01.02-Running-Pyomo-on-Google-Colab.ipynb#scrollTo=yTGBrqQO3vT2)
