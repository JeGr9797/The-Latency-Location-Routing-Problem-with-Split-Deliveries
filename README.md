# The Latency Location Routing Problem with Split Deliveries
This repository contains the instances, as well as the codes of the mathematical formulation and the metaheuristic used for the article "The Latency Location Routing Problem with Split Deliveries: Mathematical Formulation and Metaheuristic Algorithm".

In order to solve the poblem using the Iterated Local Search (ILS) metaheuristic numpy and pandas libraries are required.

## Install the library numpy

```
   pip install numpy
```

## Install the library pandas

```
   pip install pandas
```

In order to solve the matemathical model, it is necesary to have Decision Optimization Modeling for Python (DOcplex) and a cplex license.

## Install the library DOcplex

```
   pip install docplex
```

## The contents of the folders are as follows:
- Instances folder: contains .py scripts with data for all the instances (one instance per script). 
- Solution_methods folder: contains .ipynb scripts with the mathematical programming formulation and the ILS implementation.
- Experiment results folder: contains both the results of the exact methods (.xlsx) and the results of the ILS (.xlsx).
  - Regarding the ILS results, the structure of the solution is as follows:
    - Instance ID: the current instance.
    - Open_depots: the current open depots.
    - Splits: indicates if splits occurred in the current instance.
    - Routes: the routes generated for each vehicle.
    - Utilization_percentage: the percentage of capacity utilization for each vehicle.
    - Cost: solution cost for the current instance.
    - Time: solution time in seconds for the current instance.
