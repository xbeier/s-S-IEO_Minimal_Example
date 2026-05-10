# Minimal Example: Supervised Learning of Replenishment Decisions

This repository contains a minimal working example for the code accompanying the scientific article **"Supervised Learning of Optimal Replenishment Decisions"** (Bubak, Fleischmann, Stuckenschmidt, 2026).

The example illustrates how supervised learning can be used to learn period-dependent `(s, S)` replenishment policy parameters for a stochastic dynamic inventory problem under non-stationary demand. Instead of forecasting future demand distributions and repeatedly solving the inventory problem, the approach learns a direct mapping from observable features to replenishment policy parameters.

## Contents

- `Minimal Example.ipynb`  
  Jupyter notebook demonstrating the full workflow.

- `Minimal_Example.py`  
  Utility functions for computing bounds and generating `(s, S)` labels.

- `data.csv`  
  Example demand and feature data.

- `data_labelled.csv`, `data_train.csv`, `data_test.csv`  
  Generated labelled, training, and test data used in the example.

## Workflow

The notebook covers the following steps:

1. Load the example data.
2. Compute approximate optimal `(s, S)` labels.
3. Train a supervised regression model to predict policy parameters.
4. Evaluate the resulting replenishment policy on a test period.

## Requirements

The example uses Python 3.9.23 and common scientific-computing libraries, including:

- `numpy` 1.26.0
- `pandas` 2.3.2
- `scipy` 1.13.1
- `scikit-learn` 1.0.2
- `matplotlib` 3.9.4
