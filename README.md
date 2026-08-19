# Reservoir as a Dynamical System: A Tutorial Review

This repository contains the Python code and Jupyter notebooks supplementing the review article:

Contact person: Sarika Jalan (sarikajalan9@gmail.com)

Note: If you are using any of the above codes, please cite doi: inserted later

**Reservoir as a Dynamical System: A Tutorial Review**  
*(DOI to be inserted later)*

---

## Overview

This tutorial review explores Reservoir Computing (RC) through the lens of nonlinear dynamics. It acts as both a theoretical introduction and a practical implementation guide, explaining how reservoirs achieve accurate predictions and reconstruct complex behaviors. 

Together with the accompanying article, these notebooks serve as a beginner-friendly supplement to bridge nonlinear dynamics theory and hands-on machine learning implementation.

### Key Features
* **Self-Contained Notebooks:** Each notebook runs completely independently for ease of use.
* **Integrated Explanations:** Detailed markdown cells precede the code wherever required in every notebook, walking through the underlying concepts.

---

## Notebook Structure

The repository is divided into fundamental nonlinear dynamics concepts (01–05) and their direct application to Reservoir Computing architectures (06–08):

* **`01_Jacobian_eigenvalues.ipynb`**  
  Detects bifurcations in a 2D map by tracking Jacobian eigenvalues as they cross the unit circle (Neimark–Sacker bifurcation), marking the transition from a stable fixed point to an invariant closed curve.

* **`02_Bifurcations_crisis.ipynb`**  
  Generates bifurcation diagrams for both discrete (Logistic map) and continuous (Lorenz system) dynamical systems.

* **`03_FTLE.ipynb`**  
  Computes Finite-Time Lyapunov Exponents (FTLEs) and plots their distributions to quantify local stability variations across different dynamical regimes.

* **`04_scaling_transient_times.ipynb`**  
  Demonstrates power-law scaling of average chaotic transient lifetimes as trajectories linger near the remnant ("ghost") of an attractor destroyed by a boundary crisis.

* **`05_delay_coordinate_embedding.ipynb`**  
  Applies Takens' delay coordinate embedding to a single scalar variable from the Lorenz system, demonstrating that the full attractor topology can be reconstructed from 1D observations.

* **`06_RC_crisis.ipynb`**  
  Trains a Reservoir Computing model on the Logistic map and diagnoses its crisis mechanisms using the dynamical techniques introduced in previous notebooks.

* **`07_RC_FTLE.ipynb`**  
  Plots FTLE distributions for an RC model trained on the Logistic map to analyze the dynamical regimes of the reservoir's reconstructed attractor.

* **`08_RC_Jacobian_eigvals.ipynb`**  
  Trains an RC model on the Stuart–Landau oscillator and tracks its Jacobian eigenvalues to probe dynamical phase transitions inside the trained reservoir.

---

## Dependencies

The notebooks require Python along with the following packages:

* [NumPy](https://numpy.org/)
* [Matplotlib](https://matplotlib.org/)
* [NetworkX](https://github.com/networkx/networkx)
* [Directional Fibers](https://github.com/garrettkatz/directional-fibers)

---


