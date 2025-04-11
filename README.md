# DSP Lab - Homework 1  

## Overview  
This repository contains MATLAB scripts for Digital Signal Processing (DSP) Lab Homework 1, covering fundamental signal processing concepts such as sinusoidal wave generation, noise addition, and filtering.  

## Sections  

### Section 1-1: Generating a Continuous-Time Sinusoidal Wave  
A continuous-time sinusoidal wave is generated using the mathematical equation:  

x(t) = A sin(2pi f t + phi)

The amplitude A  is set to 5, the frequency f to 1 Hz, and the phase shift phi to zero. The signal is visualized using both **plot** (for a continuous representation) and **stem** (for a discrete-time representation), demonstrating the difference between continuous and sampled signals.  

### Section 1-2: Adding Random Noise  
To simulate real-world signal distortions, random noise is added to the generated sinusoidal wave. The noise is uniformly distributed in the range [-0.5, 0.5] and is summed with the original signal to create a noisy waveform. The effect of noise is analyzed by plotting both the original and noisy signals, allowing for a visual comparison of the distortion introduced by the random fluctuations.  

### Section 1-3: Moving Average Filtering (Using `conv`)  
A moving average filter is applied to the noisy sinusoidal signal to reduce high-frequency noise and smooth the waveform. The filter is implemented using convolution with a uniform kernel, where the window size determines the level of smoothing. The filtered signal is plotted alongside the noisy signal to illustrate the effectiveness of the moving average filter in noise reduction.  

### Section 1-4: Moving Average Filtering (Using `filter`)  
In this section, the moving average filter is implemented using the `filter` function instead of convolution. This method applies the filter recursively, making it more efficient for real-time processing. The same averaging kernel is used to smooth the noisy signal, and the filtered output is plotted to compare its performance with the previous convolution-based approach.  

### Section 1-5: Sinusoidal Sequence Generation Using a Difference Equation  
A discrete-time sinusoidal sequence is generated using a second-order difference equation. This method utilizes a recursive relation where each sample is computed based on previous values, avoiding the need for direct sine function evaluation. The system is implemented using the `filter` function with appropriately chosen coefficients, and the generated sequence is visualized using a stem plot to illustrate its discrete nature.  
### Section 1-6: Sampling of Multi-Frequency Signal
A composite analog signal consisting of three cosine waves at 1 kHz, 4 kHz, and 6 kHz is generated at a high sampling rate (1 MHz) to represent a continuous signal. The signal is then sampled at 5 kHz, which is below the Nyquist rate for the highest frequency component (6 kHz), causing aliasing. Both the original and sampled signals are plotted to visually demonstrate the effects of undersampling on signal reconstruction.

### Section 1-7: Frequency-Domain Analysis of Aliasing
In this section, a squared sinc function is analyzed in the frequency domain to study the effects of sampling at different rates (20, 10, 5, and 4 Hz). Using the Fourier Transform, the spectra of both the continuous signal and its sampled versions are plotted for comparison. As the sampling frequency decreases, overlapping of spectral components becomes evident, clearly demonstrating the phenomenon of aliasing.

### Section 1-8: Effect of Sampling Ratio on Signal and Spectrum
In this section, the impact of different sampling ratios (0.5, 1.5, and 3 times the original frequency) on the time-domain and frequency-domain representations of a sinc function is analyzed. The original signal is sampled at these different rates, and both the time-domain signals and their corresponding frequency spectra are plotted for comparison. As the sampling ratio changes, the spectra demonstrate variations in aliasing and frequency content.

### Section 1-9: Filter Bank Processing
In this section, a signal composed of multiple frequency components is analyzed and processed using a filter bank, consisting of analysis and synthesis filters. The signal is first filtered and downsampled, followed by scaling and upsampling before being reconstructed. The original and reconstructed signals are compared in the frequency domain, showing the effects of the filter bank processing and its impact on the signal spectrum.

## Project Repository
Check out the project repository: [DSP-Lab](https://github.com/mahdi-mahjouri/DSP-Lab)

