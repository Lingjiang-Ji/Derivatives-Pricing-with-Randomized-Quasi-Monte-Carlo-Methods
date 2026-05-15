# Derivatives-Pricing-with-Randomized-Quasi-Monte-Carlo-Methods

## Overview

This project implements Monte Carlo (MC) and Randomized Quasi-Monte Carlo (RQMC) methods for derivative pricing and numerical integration.

The research focuses on convergence behavior, payoff continuity, variance reduction, and pricing efficiency under stochastic simulation frameworks.

## Research Objectives
Implement Monte Carlo simulation for derivative pricing

Explore Randomized Quasi-Monte Carlo (RQMC) methods

Compare convergence rates and variance reduction effects

Analyze payoff continuity and numerical stability

Evaluate pricing efficiency under different simulation settings

## Methodology
Simulation Framework

Geometric Brownian Motion

Path simulation

Stochastic process discretization

Numerical integration techniques

Pricing Methods

Standard Monte Carlo

Sobol sequence sampling

Randomized Quasi-Monte Carlo (RQMC)

Variance reduction analysis

Evaluation Metrics

## Key Findings
- Quasi-Monte Carlo consistently reduced RMSE relative to standard Monte Carlo across European call, digital call, and Asian call pricing experiments.
- The variance reduction effect was strongest for the European call and Asian call payoffs, with variance reduction factors reaching above 50 at larger sample sizes.

- For the digital call, QMC still improved variance, but the gain was more limited, with variance reduction factors around 2–3 due to payoff discontinuity.
- QMC produced lower absolute bias in most settings, especially for the Asian call, where the bias decreased substantially as sample size increased.
- Standard Monte Carlo showed the expected convergence pattern, but required much larger sample sizes to approach the same error level achieved by QMC.
- QMC had higher runtime per replication, especially at larger sample sizes, creating a trade-off between computational cost and estimator accuracy.

## Variance Reduction Summary

| Payoff | n = 256 | n = 512 | n = 1024 | n = 2048 | n = 4096 | n = 8192 | n = 16384 |
|:---|---:|---:|---:|---:|---:|---:|---:|
| European Call | 12.72 | 11.61 | 23.55 | 33.84 | 55.81 | 46.01 | 52.12 |
| Digital Call | 2.07 | 2.72 | 2.50 | 3.14 | 3.15 | 2.94 | 2.84 |
| Asian Call | 14.96 | 19.03 | 42.73 | 45.33 | 35.99 | 41.16 | 52.05 |

## Results Visualization

### RMSE Comparison

(images/RMSE_eu.png)

(images/RMSE_dig.png)

(images/RMSE_as.png)

### Absolute Bias Comparison

(images/ab_eu.png)

(images/ab_dig.png)

(images/ab_as.png)

### Variance Reduction

(images/vrf.png)

### Reduction and Runtime Comparison
(images/all.png)

## Skills Demonstrated

Computational Finance

Derivatives Pricing

Stochastic Simulation

Numerical Methods

Monte Carlo Methods

Randomized Quasi-Monte Carlo

Python Scientific Computing
Pricing error
Convergence speed
Variance comparison
Numerical stability
