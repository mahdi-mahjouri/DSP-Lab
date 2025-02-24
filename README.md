# DSP Lab - Homework 1  

## Overview  
This repository contains MATLAB scripts for Digital Signal Processing (DSP) Lab Homework 1, covering fundamental signal processing concepts such as sinusoidal wave generation, noise addition, and filtering.  

## Sections  

### Section 1-1: Generating a Continuous-Time Sinusoidal Wave  
A continuous-time sinusoidal wave is generated using the mathematical equation:  
\[
x(t) = A \sin(2pi f t + \(\phi\))
\]
The amplitude (\( A \)) is set to 5, the frequency (\( f \)) to 1 Hz, and the phase shift (\( \phi \)) to zero. The signal is visualized using both **plot** (for a continuous representation) and **stem** (for a discrete-time representation), demonstrating the difference between continuous and sampled signals.  

### Section 1-2: Adding Random Noise  
To simulate real-world signal distortions, random noise is added to the generated sinusoidal wave. The noise is uniformly distributed in the range \([-0.5, 0.5]\) and is summed with the original signal to create a noisy waveform. The effect of noise is analyzed by plotting both the original and noisy signals, allowing for a visual comparison of the distortion introduced by the random fluctuations.  

### Section 1-3: Moving Average Filtering (Using `conv`)  
A moving average filter is applied to the noisy sinusoidal signal to reduce high-frequency noise and smooth the waveform. The filter is implemented using convolution with a uniform kernel, where the window size determines the level of smoothing. The filtered signal is plotted alongside the noisy signal to illustrate the effectiveness of the moving average filter in noise reduction.  

### Section 1-4: Moving Average Filtering (Using `filter`)  
In this section, the moving average filter is implemented using the `filter` function instead of convolution. This method applies the filter recursively, making it more efficient for real-time processing. The same averaging kernel is used to smooth the noisy signal, and the filtered output is plotted to compare its performance with the previous convolution-based approach.  

### Section 1-5: Sinusoidal Sequence Generation Using a Difference Equation  
A discrete-time sinusoidal sequence is generated using a second-order difference equation. This method utilizes a recursive relation where each sample is computed based on previous values, avoiding the need for direct sine function evaluation. The system is implemented using the `filter` function with appropriately chosen coefficients, and the generated sequence is visualized using a stem plot to illustrate its discrete nature.  


