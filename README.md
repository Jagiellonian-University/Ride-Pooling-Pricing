# Ride Pooling Pricing

We study a ride-sharing service with the variation of Dial-a-Ride, where each request specifies not only the source, destination, and travel time but also the revenue that is earned to serve the request. The goal is to serve requests and maximize the overall profit of the platform. A key challenge of such a platform is to satisfy the monetary constraints: riders will not pay more for the detours that occurred on the ride; drivers will make a profit for all detours due to ridesharing. The design of a pricing mechanism for such a platform is a fundamental problem, as it involves a complex mixture of economics and engineering, and how to optimally offer a pricing for revenue maximization has not been well studied yet. However, most of the state-of-the-art approaches focus on minimizing the travel distance of drivers, and new request is assigned to those who can fit the request in his schedule with the least increase in travel time. We argue that by minimizing the travel distance of driver is not always equal to the shorter trips for riders. To this end, we devise a fair pricing model for the dynamic ride-sharing service. Our cloud-based model find a shared ride while satisfying the monetary constraints for the rider to pay less as compared to non-shared ride and guarantee drivers to earn more with the increase of overall profit of ride-sharing platforms. We also provide experimental results, and our simulations in MaaSSIM support our theoretical findings and demonstrate that our algorithms perform well under settings that reflect realistic dial-a-ride systems. From the experiments, we observe that the total profit obtained by our proposed pricing model is feasible up to X\%  and runs X times faster than action-based approach; and outperforms in terms of service rate and profitability.

# Installation
This module require ExMAS and MaaSSim. 

## Building Environment (Miniconda & OSMNX)

```
language: python
python:
 - "3.7"
install:
- Miniconda (You need to configure your system with https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)

Creating a conda environment with osmnx:
 - conda info -a
 - conda config --prepend channels conda-forge
 - conda create -n ox --strict-channel-priority osmnx
 - conda activate ox
 ```
 
 ## Installing Packages 
 
 Clone this directory (cd Ride-Pooling-Pricing)
 ```
 pip install -r requirements-ExMAS.txt
 ```
 ```
 pip install -r requirements-MaaSSim.txt
```

## Installing ExMAS

```
pip install git+https://github.com/RafalKucharskiPK/ExMAS.git
```

## Installing MaaSSim

```
pip install git+https://github.com/RafalKucharskiPK/MaaSSim.git
```

### Documentation

* [Quickstart tutorial](https://github.com/Jagiellonian-University/Ride-Pooling-Pricing/blob/main/PricingModel.ipynb)


----
Usman Akhtar, Jagiellonian-University, 2022 email: usman.akhtar@uj.edu.pl








