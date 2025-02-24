# DSP-Lab
Section 1-1
In this section, a continuous-time sinusoidal wave is generated using the mathematical equation  The amplitude (A) is set to 5, the frequency (f) to 1 Hz, and the phase shift (ϕ) to zero. The signal is visualized using both plot (for a continuous representation) and stem (for a discrete-time representation), demonstrating the difference between continuous and sampled signals.

Section 1-2
To simulate real-world signal distortions, random noise is added to the generated sinusoidal wave. The noise is uniformly distributed in the range [−0.5,0.5]and is summed with the original signal to create a noisy waveform. The effect of noise is analyzed by plotting both the original and noisy signals, allowing for a visual comparison of the distortion introduced by the random fluctuations.

Section 1-3
A moving average filter is applied to the noisy sinusoidal signal to reduce high-frequency noise and smooth the waveform. The filter is implemented using convolution with a uniform kernel, where the window size determines the level of smoothing. The filtered signal is plotted alongside the noisy signal to illustrate the effectiveness of the moving average filter in noise reduction.

section 1-4
In this section, the moving average filter is implemented using the filter function instead of convolution. This method applies the filter recursively, making it more efficient for real-time processing. The same averaging kernel is used to smooth the noisy signal, and the filtered output is plotted to compare its performance with the previous convolution-based approach.

section 1-5
A discrete-time sinusoidal sequence is generated using a second-order difference equation. This method utilizes a recursive relation where each sample is computed based on previous values, avoiding the need for direct sine function evaluation. The system is implemented using the filter function with appropriately chosen coefficients, and the generated sequence is visualized using a stem plot to illustrate its discrete nature.
