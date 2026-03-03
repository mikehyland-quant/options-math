# options-math

Python implementations of core option pricing models, volatility surface frameworks, and supporting mathematical utilities.

This repository contains modular tools for pricing, implied volatility extraction, and volatility surface construction across multiple model frameworks.

The goal is not academic replication, but practical implementation consistent with trading desk usage.

---

## Overview

The repository covers:

- Closed-form option pricing
- Greeks and sensitivity analysis
- Implied volatility inversion
- Volatility skew modeling
- Stochastic volatility frameworks
- Parametric volatility surface construction

Models are implemented with clarity and numerical stability in mind, and are structured for use in trading or research environments.

---

## Repository Contents

### Core Pricing & Math

- **Options_Math_Algebra**
  - Foundational algebra and mathematical identities used in pricing derivations.

- **Options_Math_Black_Scholes**
  - Black–Scholes pricing (calls & puts)
  - Greeks (Delta, Gamma, Vega, Theta, Rho)
  - Implied volatility solver
  - Forward pricing framework

- **Options_Math_Helpers**
  - Parent class
  - Numerical utilities
  - Root-finding tools
  - Normal distribution functions
  - Volatility conversions

---

### Volatility Surface & Skew Models

- **Options_Skew_SABR**
  - SABR implied volatility approximation
  - Parameter calibration logic
  - Smile dynamics

- **Options_Skew_Heston** - SOON
  - Stochastic volatility framework
  - Characteristic function-based pricing
  - Volatility skew implications

- **Options_Skew_SVI** - SOON
  - Stochastic Volatility Inspired (SVI) parameterization
  - Arbitrage constraints
  - Surface fitting considerations

- **Options_Skew_Wow_Alpha**
  - Volatility surface parameterization inspired by proprietary market-making frameworks
  - Forward-vol decomposition logic
  - Surface smoothing techniques

---

## Design Philosophy

This codebase emphasizes:

- Clean mathematical implementation
- Practical calibration workflows
- Stability under edge-case inputs
- Explicit separation between pricing and surface construction
- Readability for desk-level review

The focus is on understanding *why* models behave as they do — not merely calling a library function.

---

## Applications

These tools support:

- Options market-making analytics
- Vol surface construction
- Risk management & hedging analysis
- Relative value volatility trades
- Structured product pricing
- Academic exploration of model dynamics

---

## Technical Notes

- Python + NumPy
- Closed-form and semi-analytic solutions
- Numerical solvers for implied vol and calibration
- Modular structure for integration into larger trading frameworks

---

## Context

This repository reflects practical derivatives experience across:

- Equity options
- Interest rate derivatives
- Crypto options
- Volatility surface modeling
- Forward-vol decomposition

The implementations align with methodologies used in professional trading environments.
This code performs options math including Black Scholes pricing and greeks, volatility back-solving, and parameterized skew generation.

