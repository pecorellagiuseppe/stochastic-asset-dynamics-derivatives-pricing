# Stochastic Asset Dynamics and Derivatives Pricing

**Quantitative Financial Modeling | Sapienza University of Rome | Group Project (2026)**

## Project Overview

This project explores the mathematical foundations of stochastic asset dynamics and derivatives pricing, combining theoretical derivations with numerical simulations in Python.

The theoretical analysis focuses on Itô's Lemma, the derivation of the Black–Scholes partial differential equation (PDE) through delta hedging, and the Merton extension for assets paying continuous dividends.

The computational component illustrates Geometric Brownian Motion (GBM), numerical applications of Itô's Lemma, and the mean-reverting behavior of the Ornstein–Uhlenbeck (OU) process.

## Objectives

- Study stochastic processes and apply Itô's Lemma to financial asset dynamics.
- Derive the Black–Scholes PDE using a delta-hedged portfolio and no-arbitrage arguments.
- Extend the Black–Scholes framework to continuously dividend-paying assets.
- Simulate Geometric Brownian Motion using Python.
- Explore Itô's Lemma through numerical simulations.
- Model mean reversion using the Ornstein–Uhlenbeck process.

## Mathematical Framework

### 1. Geometric Brownian Motion

Geometric Brownian Motion models the stochastic evolution of an asset price:

```math
dS_t = \mu S_t\,dt + \sigma S_t\,dW_t
```

where:

- **μ** represents the expected return.
- **σ** represents volatility.
- **W** is a standard Brownian motion.

### 2. Black–Scholes PDE

By applying Itô's Lemma and constructing a dynamically delta-hedged portfolio, the Black–Scholes PDE for a non-dividend-paying asset is obtained:

```math
\frac{\partial V}{\partial t} + \frac{1}{2}\sigma^2 S^2\frac{\partial^2 V}{\partial S^2} + rS\frac{\partial V}{\partial S} - rV = 0
```

where **V** is the derivative value, **S** is the underlying asset price, and **r** is the risk-free interest rate.

### 3. Merton Extension

For an underlying asset paying a continuous dividend yield **q**, the pricing PDE becomes:

```math
\frac{\partial V}{\partial t} + \frac{1}{2}\sigma^2 S^2\frac{\partial^2 V}{\partial S^2} + (r-q)S\frac{\partial V}{\partial S} - rV = 0
```

This extension accounts for the effect of continuous dividend payments on derivatives pricing.

### 4. Ornstein–Uhlenbeck Process

The Ornstein–Uhlenbeck process describes stochastic dynamics with mean reversion:

```math
dX_t = \kappa(\theta-X_t)\,dt + \sigma\,dW_t
```

where:

- **κ** represents the speed of mean reversion.
- **θ** represents the long-run mean.
- **σ** represents volatility.

## Python Implementation

The Jupyter notebook includes:

- Simulation and visualization of GBM paths.
- Numerical exploration of Itô's Lemma.
- Simulation of Ornstein–Uhlenbeck paths.
- Visualization of stochastic behavior and mean reversion.

**Technologies:** Python, NumPy, Matplotlib, Jupyter Notebook.

## Repository Structure

| File | Description |
| --- | --- |
| [stochastic_simulations.ipynb](stochastic_simulations.ipynb) | Python simulations of GBM, Itô's Lemma, and the OU process. |
| [stochastic_asset_dynamics_report.pdf](stochastic_asset_dynamics_report.pdf) | Theoretical report containing mathematical derivations and financial interpretation. |
| [derivatives_pricing_presentation.pdf](derivatives_pricing_presentation.pdf) | Presentation summarizing the theoretical framework and computational results. |

## How to Run

Install the required Python packages:

```bash
pip install numpy matplotlib notebook
```

Launch the notebook:

```bash
jupyter notebook stochastic_simulations.ipynb
```

## Skills and Methods

**Python | Quantitative Finance | Stochastic Calculus | Stochastic Differential Equations | Black–Scholes | Derivatives Pricing | Numerical Simulation | Financial Modeling**

## Authors

This project was developed as part of the **Quantitative Financial Modeling** course at **Sapienza University of Rome**.

**Contributors:**

- Leonardo Satoru Alosi
- Sahar JafariDoust
- Giuseppe Pecorella
- Amina Migdanova
- Sebastiano Rocchi

This repository documents collaborative academic work and is intended for educational purposes.  
