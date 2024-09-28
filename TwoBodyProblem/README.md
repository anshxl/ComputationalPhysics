# Two-Body Gravity Problem: Lagrangian Dynamics and Numerical Solution

## Introduction
This project explores the relative motion of two bodies interacting through gravitational attraction in a two-dimensional space using Lagrangian mechanics. The equations of motion are derived and solved numerically to analyze the resulting trajectories for various initial conditions.

## Problem Overview
The problem models the mutual gravitational pull between two masses, leading to orbital-like trajectories. The motion is restricted to two dimensions, and the center of mass (CoM) frame and relative coordinates are used to simplify the problem.

## Assumptions and Simplifications
- Both bodies are treated as point masses.
- The motion is restricted to two dimensions.
- No external forces act on the system.
- The center of mass (CoM) frame and relative coordinates are used.

## Lagrangian Mechanics
The Lagrangian \( L = T - V \) is constructed from the kinetic and potential energy of the system:
- **Kinetic Energy (T)**: The total kinetic energy is the sum of the kinetic energy of both masses, expressed in terms of the reduced mass \( \mu \) and the total mass \( M \).
- **Potential Energy (V)**: The potential energy is the gravitational potential energy between the two bodies.

## Euler-Lagrange Equations
Using the Euler-Lagrange formalism, the equations of motion for the relative coordinates \( r \) and \( \phi \) are derived:
- \( \ddot{r} = r \dot{\phi}^2 - \frac{Gm_1m_2}{\mu r^2} \)
- \( \ddot{\phi} = - \frac{2\dot{r}\dot{\phi}}{r} \)

## Numerical Solution
The second-order equations are converted into first-order equations for numerical solution using the following substitutions:
- \( v = \dot{r} \)
- \( \omega = \dot{\phi} \)

The equations are then solved using numerical integration methods.

## Usage Instructions
1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   ```
2. **Navigate to the project directory**:
   ```bash
   cd <project-directory>
   ```
3. **Install te required dependencies**:
   ```bash
   pip install numpy matplotlib scipy
   ```
4. **Run the Jupyter Notebook:**
   ```bash
   jupyter notebook WORKEDPROBLEM1.ipynb
   ```
   
**License**
This project is licensed under the MIT License.
