# Brownian Motion Simulation

This project simulates the random motion of particles, also known as Brownian motion, using Monte Carlo methods. The simulation is implemented in a Jupyter Notebook and visualized through interactive plots and animations.

## Features
- **1D and 2D Brownian Motion Simulations**:
  - Models the stochastic motion of particles in one and two dimensions.
  - Calculates Mean Squared Displacement (MSD) and compares it with theoretical predictions.

- **Interactive Animation**:
  - Visualizes 2D Brownian motion trajectories of particles starting from random initial positions.

- **Parameter Sensitivity Analysis**:
  - Explores the effects of time step size $( \Delta t )$ on MSD accuracy.
  - Investigates statistical properties such as displacement distributions.

## Structure of the Notebook
1. **Introduction**:
   - Overview of Brownian motion and its connection to stochastic processes and diffusion.
   - Mathematical formulation of Brownian motion.

2. **Simulation Code**:
   - Functions to simulate 1D and 2D Brownian motion.
   - Integration of random initial positions for particles in 2D.

3. **Analysis**:
   - Mean Squared Displacement (MSD) calculations and comparison with theoretical values.
   - Visualization of displacement distributions and parameter sensitivity.

4. **Visualization**:
   - Static and dynamic plots of particle trajectories.
   - Animated visualization of 2D Brownian motion, saved as a video file.

5. **Extra Features**:
   - Statistical validation of results.
   - Adjustable parameters for in-depth exploration.

## How to Run the Notebook
1. **Prerequisites**:
   - Python 3.x
   - Jupyter Notebook
   - Required Python libraries: `numpy`, `matplotlib`, `IPython`

## Output
- **1D and 2D Plots**:
  - Trajectories of particles over time.
  - Comparison of simulated and theoretical MSD.

- **Animation**:
  - A dynamic visualization of 2D Brownian motion, viewable inline or as a saved video file (`brownian_motion.mp4`).

## Customization
The notebook includes parameters to customize:
- Number of particles ($ N $).
- Total time steps ($ T $).
- Time step size ($ \Delta t $).
- Initial positions for 2D motion.


## References and Readings
1. [Oscar Mickelin's Brownian Motion Analysis](https://web.mit.edu/8.334/www/grades/projects/projects17/OscarMickelin/brownian.html)
2. J. Matson, ‘‘Crowd Forcing: Random Movement of Bacteria Drives Gears’’. Available at [Scientific American](https://www.scientificamerican.com/article/brownian-motion-bacteria/).
3. Feynman, ‘‘Feynman Lectures on Physics’’. Available at [Feynman Lectures](http://www.feynmanlectures.caltech.edu/I_41.html).
4. Central Limit Theorem. Available at [Wikipedia](https://en.wikipedia.org/wiki/Central_limit_theorem).

## License
This project is licensed under the MIT License.
