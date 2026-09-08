# Early-stage epidemic modelling and parameter estimation

A piece of coursework from the University of Bristol module *Mathematical Modelling in Biology, Medicine and Public Health*.

## Overview

This analysis investigates the early dynamics of an epidemic using a mechanistic mathematical model.

The computational component fits the model to supplied time-series data, estimates identifiable combinations of epidemiological parameters and compares the mechanistic representation with simpler empirical alternatives.

## Analysis

The R implementation:

- Defines the analytical form of the epidemic-growth model
- Uses a log-linear approximation to obtain starting parameter values
- Fits the model using nonlinear least squares
- Uses the Levenberg-Marquardt algorithm through `minpack.lm`
- Recovers identifiable combinations of epidemiological parameters
- Examines fitted values and residuals
- Fits an alternative exponential model
- Fits quadratic, cubic and quartic polynomial models
- Compares models using residual sum of squares and residual diagnostics

The parameterisation relates the fitted eigenvalues to combinations involving transmission, progression and recovery rates.

## Repository structure

- `Coursework_1.pdf` — coursework brief
- `CW1_4iii_4iv.Rmd` — R implementation for Questions 4(iii) and 4(iv)
- `CW1_4iii_4iv.pdf` — rendered analysis
- `data.csv` — supplied data

## Tools

R, nonlinear least squares, `minpack.lm`, linear regression and residual analysis.
