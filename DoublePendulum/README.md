# Double Pendulum Simulation
## Project Description
This project simulates the dynamics of a double pendulum system, which consists of two point masses connected by rigid rods. The first mass is connected to a pivot point, and the second mass is connected to the first mass. The system exhibits two degrees of freedom, represented by the angles $\theta_1$ (angle of the first rod from the vertical) and $\theta_2$ (angle of the second rod from the vertical). The double pendulum is a classic example of a chaotic system, where small changes in initial conditions can lead to drastically different outcomes.

## Objectives
Investigate the chaotic dynamics of the double pendulum.
Analyze the stability of the system at its equilibrium points and examine how trajectories evolve over time in the phase space.
Use numerical integration to explore the system’s time evolution.

## System Description
**Variables**
$\theta_1$: Angle of the first pendulum.
$\theta2$: Angle of the second pendulum.
$\dot{\theta_1}, \dot{\theta_2}$: Angular velocities of the first and second pendulums.
Parameters
$m_1, m_2$: Masses of the two pendulums.
$L_1, L_2$: Lengths of the rods.
$g$: Gravitational acceleration.

## Plan
**Phase Space Analysis**
Create a phase portrait with angular velocities $\dot{\theta_1}$ and $\dot{\theta_2}$ plotted against angles $\theta_1$ and $\theta_2$.
Identify and label any fixed points (e.g., both pendulums in vertical or horizontal positions).

**Stability of Fixed Points**
Calculate the fixed points where $\theta_1$ and $\theta_2$ do not change over time (e.g., when both pendulums are perfectly aligned in the vertical down or up position).
Analyze the stability by linearizing the system near the fixed points and calculating eigenvalues of the Jacobian matrix at these points. Stable, unstable, and saddle points will be characterized.

**Numerical Integration**
Use a numerical method (e.g., Runge-Kutta) to integrate the system of ODEs and find trajectories over time for given initial conditions.
Plot the resulting trajectories in the phase space to visualize chaotic behavior.

## Equations of Motion
The equations of motion for the double pendulum system, derived from the Euler-Lagrange equations, are:

$$
(m_1 + m_2) L_1^2 \ddot{\theta}_1 + m_2 L_1 L_2 \left( -\sin(\theta_1 - \theta_2) (\dot{\theta}_1 - \dot{\theta}_2) \dot{\theta}_2 + \dot{\theta}_1 \ddot{\theta}_2 \right) + (m_1 + m_2) g L_1 \sin \theta_1 = 0
$$

$$
m_2 L_2^2 \ddot{\theta}_2 + m_2 L_1 L_2 \left( \dot{\theta}_1 (-\sin(\theta_1 - \theta_2)(\dot{\theta}_1 - \dot{\theta}_2)) + \dot{\theta}_2 \ddot{\theta}_1 \right) - m_2 g L_2 \sin \theta_2 = 0
$$

## Functions
The project includes functions to compute the phase portrait and calculate the trajectories for both pendulums. The inspiration for this code comes from the in-class activity done on September 10, 2024.

## Usage
Install Dependencies: Ensure you have numpy and scipy installed.
Run the Simulation: Execute the Jupyter Notebook to simulate the double pendulum and visualize the phase portraits and trajectories.
