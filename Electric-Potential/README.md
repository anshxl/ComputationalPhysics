# Electric Potential in a Rectangular Box

## Introduction
This project investigates the electric potential in a rectangular box with sinusoidal boundary conditions. The goal is to analyze the potential distribution using both analytical and numerical methods.

## System Description
The system consists of a rectangular box with:
- Width $a$
- Height $b$
- Amplitude of the sinusoidal potential $V_0$
- Number of Fourier terms to sum $ \text{terms} $
- Resolution of the grid $ \text{steps} $

## Analytical Setup
The electric potential is calculated using a Fourier series expansion. The potential at each point $(x, y)$ is given by:
$$V(x, y) = \frac{4V_0}{\pi} \sum_{2n+1}^{\infty}\frac{\sinh(\frac{n\pi x}{a})\sin(\frac{n\pi y}{a})}{n \sinh(\frac{n\pi b}{a})}$$


## Numerical Methods
The numerical simulation involves:
1. Defining parameters.
2. Creating a grid of points in space.
3. Calculating the electric potential at each point using the Fourier series expansion.
4. Visualizing the potential distribution using a 3D surface plot.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
