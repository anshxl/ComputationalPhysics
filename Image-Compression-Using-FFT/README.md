# **Image Compression Using 2D FFT**

## **Overview**

This project demonstrates how to compress an image using the 2D Fast Fourier Transform (FFT). The FFT is a mathematical tool that transforms an image from the spatial domain into the frequency domain, enabling us to analyze and manipulate its frequency components for compression. By retaining only the most significant frequencies, we achieve a lossy compression technique while maintaining the overall structure of the image.

This project is conducted as part of a physics class to explore the mathematical and physical concepts behind Fourier analysis and its applications.

---

## **Key Features**
1. **Mathematical Foundations**: 
   - Detailed explanations of the 2D FFT, its inverse, and its relevance to image compression.
   - Parseval's theorem for energy conservation in the frequency domain.
   
2. **Frequency Domain Analysis**:
   - Visualize the magnitude spectrum of an image.
   - Filter frequency bands (low, medium, high) and analyze their contributions to the image.

3. **Compression**:
   - Apply frequency masks to retain specific frequency bands.
   - Reconstruct the image from filtered frequency components and evaluate the compression ratio and quality.

4. **Physics Connections**:
   - Insights into the decomposition of signals into sinusoidal components, analogous to wave analysis in physics.

---

## **Mathematics of 2D FFT**

The 2D FFT transforms an image \( f(x, y) \) from the spatial domain into the frequency domain \( F(u, v) \) using the following equation:

\[
F(u, v) = \sum_{x=0}^{M-1} \sum_{y=0}^{N-1} f(x, y) \cdot e^{-2\pi i \left( \frac{ux}{M} + \frac{vy}{N} \right)}
\]

The inverse transform reconstructs the image:

\[
f(x, y) = \frac{1}{MN} \sum_{u=0}^{M-1} \sum_{v=0}^{N-1} F(u, v) \cdot e^{2\pi i \left( \frac{ux}{M} + \frac{vy}{N} \right)}
\]

These equations decompose the image into a sum of sinusoidal basis functions.

---

## **Project Workflow**

### **1. Load and Visualize the Image**
- A sample grayscale image is used as the input.

### **2. Perform 2D FFT**
- Compute the frequency domain representation of the image using the 2D FFT.
- Visualize the magnitude spectrum to identify dominant frequency components.

### **3. Filter Frequencies**
- Apply masks to selectively retain low, medium, or high frequencies.
- Visualize the filtered frequency spectrum.

### **4. Reconstruct the Image**
- Use the inverse FFT to reconstruct the image from the filtered frequency components.
- Compare the reconstructed image with the original to evaluate compression quality.

### **5. Analyze Energy Contributions**
- Compute the energy contributions of low, medium, and high-frequency bands.
- Highlight the dominance of low frequencies in natural images.

### **6. Explore Compression Trade-offs**
- Experiment with different mask sizes to balance compression ratio and image quality.
- Plot Compression Ratio vs. Mean Squared Error (MSE) to visualize trade-offs.

---

## **Results**

### **Key Observations**:
1. Most of the image's energy is concentrated in the low-frequency components, representing smooth variations.
2. High frequencies contribute to fine details but make up a small fraction of the energy.
3. Increasing the mask size improves image quality but reduces compression efficiency.

### **Metrics**:
- **Compression Ratio**: Percentage of frequencies retained.
- **Mean Squared Error (MSE)**: Quantifies the difference between the original and reconstructed images.

---

## **Applications**
- **Image Compression**: Demonstrates the principles behind compression algorithms like JPEG.
- **Physics**: Connects Fourier analysis to wave decomposition and energy distribution in signals.
- **Signal Processing**: Explains the role of frequency filtering in noise reduction and signal enhancement.

---

## **Requirements**

### **Libraries Used**:
- `numpy`: For numerical computations.
- `scipy`: For FFT operations and image processing.
- `matplotlib`: For visualizations.
- `Pillow`: For loading and preprocessing images.

Install the required libraries using:

```bash
pip install numpy scipy matplotlib pillow
```

---

## **How to Run**

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/image-compression-fft.git
   cd image-compression-fft
   ```

2. Open the Jupyter notebook:
   ```bash
   jupyter notebook Image-Compression.ipynb
   ```

3. Run the cells sequentially to execute the project workflow.

---

## **References**
1. Demofox. *Frequency Domain Image Compression and Filtering*. (2020).  
   Available at: [https://blog.demofox.org/2020/11/04/frequency-domain-image-compression-and-filtering/](https://blog.demofox.org/2020/11/04/frequency-domain-image-compression-and-filtering/)

2. University of Edinburgh. *The Fourier Transform and Its Applications in Image Processing*.  
   Available at: [https://homepages.inf.ed.ac.uk/rbf/HIPR2/fourier.htm](https://homepages.inf.ed.ac.uk/rbf/HIPR2/fourier.htm)

3. SciPy Documentation. *Fast Fourier Transform (FFT)*.  
   Available at: [https://docs.scipy.org/doc/scipy/reference/fft.html](https://docs.scipy.org/doc/scipy/reference/fft.html)

---

## **Future Extensions**
1. Apply the method to color images by analyzing each color channel separately.
2. Experiment with advanced masks (e.g., Gaussian filters).
3. Explore applications like noise reduction, image denoising, or feature extraction.
