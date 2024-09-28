# Duffing Oscillator Investigation

This repository contains a Jupyter Notebook that investigates the Duffing Equation, a second-order nonlinear ordinary differential equation describing the motion of a damped oscillator with a nonlinear restoring force.

## Description

The Duffing equation is expressed as:

$$
\frac{d^2x}{dt^2} + \delta \frac{dx}{dt} + \alpha x + \beta x^3 = \gamma \cos{\omega t}
$$

where:
- $x$ is the displacement,
- $t$ is time,
- $\delta$ is the damping coefficient,
- $\alpha$ is the linear stiffness coefficient,
- $\beta$ is the nonlinear stiffness coefficient,
- $\gamma$ is the amplitude of the driving force,
- $\gamma$ is the frequency of the driving force.

The notebook explores the behavior of the Duffing oscillator under various conditions and provides analytical insights into its dynamics.

## Installation

To run this notebook, you need to have Jupyter Notebook installed along with the necessary Python libraries. You can install the required libraries using:

```bash
pip install -r requirements.txt
