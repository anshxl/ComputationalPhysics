# Coupled Pendulum System with Damping: A Normal Mode Analysis

This repository contains a Jupyter Notebook that explores the dynamics of a coupled pendulum system with three pendulums linked by springs and influenced by gravity. The goal of this project is to analyze the **normal modes** of oscillation for the system and to investigate the effects of adding a **dissipative (damping) term** on mode selection and synchronization.

## Project Overview

The notebook systematically covers the following:

1. **System Setup and Derivation of Equations of Motion**:
   - We set up a system of three identical pendulums with spring couplings and derive the equations of motion using **Lagrangian mechanics**.
   - The equations of motion are expressed in matrix form to facilitate normal mode analysis.

2. **Normal Mode Analysis**:
   - By calculating the **eigenvalues and eigenvectors** of the system’s coefficient matrix, we identify the normal modes and their corresponding frequencies.
   - Each normal mode represents a unique pattern of oscillation with a distinct frequency, showing how the pendulums move in sync or out of phase depending on the mode.

3. **Numerical Solution of the System**:
   - Using SciPy’s `solve_ivp`, we numerically solve the system’s differential equations for a given set of initial conditions.
   - We visualize the time evolution of each pendulum’s angular displacement, which highlights how the initial conditions determine the interplay of modes.

4. **Damping and Mode Selection**:
   - We add a damping term to each equation of motion to simulate energy loss over time.
   - With damping, the system gradually settles into the **lowest-frequency mode**, demonstrating how dissipative effects lead to synchronization in coupled systems.

## Key Findings

1. **Normal Mode Patterns**:
   - We identified three distinct normal modes, each with a specific frequency and oscillation pattern. The modes range from independent motion of outer pendulums to synchronized motion of all pendulums.
   
2. **Effect of Random Initial Conditions**:
   - Without damping, random initial conditions lead to a superposition of all three modes, resulting in complex, quasi-periodic motion.

3. **Damping and Synchronization**:
   - Adding a small damping coefficient drives the system toward the lowest-frequency mode, resulting in synchronized oscillation. This shows how dissipative forces help coupled oscillatory systems achieve coherence over time.

## Running the Notebook

To explore the project further:
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/coupled-pendulum-damping.git
   ```
2. Install required dependencies (e.g., `numpy`, `scipy`, `matplotlib`, `sympy`).
3. Open the notebook in Jupyter and run each cell to reproduce the results.

## Future Directions

Future work on this system could involve exploring **nonlinear effects** or varying the damping coefficient to study the onset of synchronization in more detail. Additionally, larger coupled systems or different initial conditions could reveal further insights into the dynamics of oscillatory networks.
