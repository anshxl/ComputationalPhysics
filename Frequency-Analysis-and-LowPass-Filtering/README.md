---
# Frequency Analysis and Low-Pass Filtering of a Randomized Harmonic Signal Using Fourier Methods

## Project Overview

This project applies Fourier Transform methods to analyze, filter, and reconstruct a complex, randomized harmonic signal. The signal is generated with three base frequencies (50 Hz, 120 Hz, and 250 Hz) and additional randomized harmonics, phase shifts, and noise to simulate a realistic audio waveform. By decomposing the signal into its frequency components, we gain insights into the underlying structure and create a low-pass filter to selectively remove high-frequency components. This exploration highlights the power of Fourier analysis in signal processing.

## Key Features

- **Signal Generation**: A randomized signal is created with specific base frequencies, harmonics, and noise. The signal is also playable to hear the original audio waveform.
- **Fourier Series Approximation**: Custom Fourier functions approximate the original signal, visualizing how well a Fourier series captures the waveform in the time domain.
- **Frequency Analysis**: We compute and plot the Fourier coefficients, identifying the dominant frequencies and visualizing the frequency spectrum through stem plots and spectrograms.
- **Low-Pass Filtering (Extra Credit)**: A custom low-pass filter removes high-frequency components, allowing us to reconstruct and analyze a filtered version of the signal both visually and audibly.

## Project Structure

- **Signal Generation**: Generates a signal composed of base frequencies with added randomized harmonics and Gaussian noise.
- **Fourier Approximation**: Uses custom Fourier functions to approximate the original signal with a Fourier series.
- **Frequency Analysis**: Plots the signal's frequency spectrum to identify dominant frequencies.
- **Low-Pass Filter**: Applies a low-pass filter to remove frequencies above a specified cutoff (200 Hz), then reconstructs the filtered signal.
- **Visualizations**: Plots the time-domain signal, frequency spectrum, and spectrograms for both original and filtered signals.

## How to Run the Project

1. **Requirements**: Install the necessary Python libraries, including `numpy`, `matplotlib`, and `sounddevice`.
   ```bash
   pip install numpy matplotlib sounddevice
   ```

2. **Notebook Execution**: Open the provided Jupyter notebook (`SimpleFourierAnalysis.ipynb`) and run each cell in sequence. The notebook contains code, explanations, and visualizations for each step of the analysis.

3. **Playing Audio**: The project uses the `sounddevice` library to play audio. Ensure your sound system is functional, and adjust the playback duration or amplitude as needed.

## Results and Observations

- **Original Signal**: The signal exhibits complex harmonic structure with clear peaks at base frequencies and harmonics.
- **Filtered Signal**: The low-pass filter effectively removes high-frequency noise, creating a smoother audio output that preserves the fundamental components.
- **Frequency Spectrum**: Visualizations show the dominant frequencies, highlighting the effects of filtering on the signal’s frequency content.

## Conclusion

This project demonstrates the utility of Fourier Transform methods in analyzing and manipulating complex signals. By breaking down a signal into its frequency components and applying a low-pass filter, we can selectively shape and understand the signal’s structure. This approach has broad applications in audio processing, communications, and other fields requiring frequency-based analysis.

---

