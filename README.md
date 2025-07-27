# Option-Pricing-using-Cpp-MonteCarlo

## Project Overview

This project is a fully integrated, high-performance Monte Carlo simulation framework for European option pricing using the Black-Scholes model. The core pricing engine is written in modern **C++17**, employing **multithreading** to efficiently simulate thousands of trajectories per thread. 

The C++ engine is exposed to Python using **pybind11**, enabling seamless integration with **Python-based visualization and analysis workflows**. The interface supports pricing of both **Call and Put options**, computation of the full suite of **Greeks** (Delta, Gamma, Vega, Theta, Rho), and calculation of P&L relative to a user-defined market price.

A web-based interactive dashboard is built using **Streamlit**, allowing users to:

- Explore the behavior of option price and sensitivities across a grid of spot prices and volatilities
- Visualize results as **heatmaps** with intuitive color gradients (red for negative P&L, green for positive)
- Select individual Greeks to plot and analyze their movement with respect to input variables
- Record simulation metadata and results to a local **SQLite database** for inspection, reproducibility, or audit trails

This project demonstrates strong **quantitative software engineering**, with applications in derivatives pricing, trading strategy prototyping, and risk analysis. It combines the low-latency power of C++ with the analytical and visualization capabilities of Python.
