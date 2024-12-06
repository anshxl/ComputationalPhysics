# Seismic Wave Propagation Simulation Using Ricker Wavelets

This project demonstrates a simulation of seismic wave propagation using the **Ricker wavelet** as the source function. The wave propagation is visualized on a 2D grid with variable wave speeds, incorporating realistic elements like absorbing boundaries and Gaussian noise for realism. The resulting animation illustrates how seismic waves travel through a medium with heterogeneity.

---

## Features
- **Wave Propagation Simulation**:
  - Uses a 2D grid to simulate the propagation of seismic waves.
  - Implements realistic wave speed variations to mimic geological heterogeneity.

- **Ricker Wavelet Source**:
  - The Ricker wavelet serves as the source time function, providing a realistic seismic signal.

- **Absorbing Boundaries**:
  - Reduces wave reflections at the grid edges for a more realistic simulation.

- **Gaussian Noise**:
  - Adds environmental or measurement noise for increased realism.

- **Visualization**:
  - Generates an animated GIF of the seismic wave propagation.

---

## Project Structure
The main code is organized into a Jupyter notebook containing:
1. **Ricker Wavelet Definition**:
   - Function to generate a Ricker wavelet based on the dominant frequency.
2. **Simulation Setup**:
   - Initialization of the 2D grid, wave speed map, and displacement fields.
3. **Wave Propagation**:
   - Function to update the wavefield using finite-difference approximations.
4. **Animation**:
   - Visualization of wave propagation over time, saved as a GIF.

---

## How It Works
1. **Grid and Medium Setup**:
   - A 2D grid is initialized with spatial resolution (`dx`, `dy`) and uniform wave speed.
   - A region of the grid has a lower wave speed to simulate geological variations.

2. **Source Function**:
   - A Ricker wavelet, centered at the grid's midpoint, represents the seismic source.

3. **Wave Propagation**:
   - Wavefield updates are performed iteratively using a finite-difference method for the wave equation.
   - Gaussian noise is added to simulate ambient disturbances.

4. **Boundary Conditions**:
   - Absorbing boundary conditions prevent artificial reflections from the grid edges.

5. **Animation**:
   - The wavefield is visualized using a `matplotlib` animation, which is saved as a GIF.

---

## Requirements
To run the project, ensure you have the following Python packages installed:
- `numpy`
- `matplotlib`
- `Pillow` (for saving GIFs)

You can install these dependencies with:
```bash
pip install numpy matplotlib pillow
```

---

## How to Run
1. Clone this repository or download the notebook file `SeismicWavePropogation.ipynb`.
2. Open the notebook in JupyterLab, Jupyter Notebook, or any compatible environment.
3. Run all cells to generate the wave propagation animation.

---

## Example Output
The simulation produces a GIF visualizing wave propagation. The waves originate at the source (center of the grid) and propagate outward, interacting with the heterogeneous medium and dissipating at the boundaries.

---

## Customization
- **Wave Speed Map**:
  - Modify the `c_map` variable to define custom geological variations.
- **Noise Level**:
  - Adjust the noise amplitude in the `update_realistic_wave` function.
- **Wavelet Frequency**:
  - Change the dominant frequency (`f_0`) to explore different wavelet characteristics.

---

## Acknowledgments
This project was inspired by real-world applications of wave propagation in seismic studies. The Ricker wavelet, commonly used in geophysics, provided a realistic foundation for modeling seismic sources.
