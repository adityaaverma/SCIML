# Scientific Machine Learning Mini Project

This project demonstrates the power of **Scientific Machine Learning (SciML)** by combining classical **differential equation models** with modern **neural networks**. The focus is on modeling the **Lotka–Volterra predator-prey system** using **Universal Differential Equations (UDEs)** in Julia.

---

## 📌 Project Overview
- Implemented the **Lotka–Volterra predator-prey model** with known population dynamics.
- Introduced a **neural network (Lux.jl)** to approximate the *unknown interaction terms* in the dynamics.
- Leveraged **Universal Differential Equations (UDEs)** to hybridize mechanistic modeling and data-driven learning.
- Performed parameter optimization using:
  - **ADAM optimizer** for initial training.
  - **LBFGS optimizer** for fine-tuning and convergence.
- Evaluated results with:
  - Loss curves (ADAM vs. LBFGS).
  - Comparison of predicted vs. ground-truth trajectories.
  - Error plots for learned interactions.

---

## 🛠️ Tech Stack
- **Programming Language:** Julia
- **Libraries:**
  - [OrdinaryDiffEq.jl](https://github.com/SciML/OrdinaryDiffEq.jl) – ODE solvers
  - [ModelingToolkit.jl](https://github.com/SciML/ModelingToolkit.jl) – symbolic modeling
  - [DataDrivenDiffEq.jl](https://github.com/SciML/DataDrivenDiffEq.jl) – data-driven modeling
  - [SciMLSensitivity.jl](https://github.com/SciML/SciMLSensitivity.jl) – sensitivity analysis
  - [Lux.jl](https://github.com/avik-pal/Lux.jl) – neural networks
  - [Optimization.jl](https://github.com/SciML/Optimization.jl) – optimization framework

---

## 🚀 Results
- Successfully trained the hybrid UDE to approximate missing system dynamics.
- Reduced training loss from **1e-1 → 1e-4** through two-stage optimization.
- Demonstrated that UDEs can capture nonlinear interactions more effectively than purely mechanistic or purely data-driven models.

---

## 📊 Visualizations
- **Training Loss Curves:** Comparison between ADAM and LBFGS optimizers.
- **Trajectory Plots:** Ground truth vs. neural approximation.
- **Error Analysis:** L2-error between predicted and true interactions.

---

## 📂 Project Structure
