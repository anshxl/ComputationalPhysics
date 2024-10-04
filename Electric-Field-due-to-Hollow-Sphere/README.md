# Electric Field of a Charged Hollow Sphere

## Introduction
This project investigates the electric field of a uniformly charged hollow spherical shell. The goal is to analyze the electric field at various points in space both inside and outside the sphere using both analytical and numerical methods.

## System Description
The system consists of a hollow spherical shell with:
- Radius $R$
- Total charge $Q$
- Coulomb's constant $k = 8.99 \times 10^9 \, \frac{Nm^2}{C^2}$
- Radial distance $r$ from the center of the sphere

## Analytical Setup
The electric field is analyzed in two regions:
1. **Inside the Hollow Sphere $r \leq R$**: The electric field is zero.
2. **Outside the Hollow Sphere ($r > R$)**: The electric field is given by $E = \frac{kQ}{r^2}$.

## Numerical Methods
The numerical simulation involves:
1. Defining parameters.
2. Creating a grid of points in space.
3. Calculating the electric field at each point using the analytical expressions.
4. Visualizing the electric field lines.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
