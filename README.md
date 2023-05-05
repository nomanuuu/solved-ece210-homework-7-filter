Download Link: https://assignmentchef.com/product/solved-ece210-homework-7-filter
<br>
For each of the following scenarios, you will generate a filter, create magnitudephase plots for the filter, and apply the filter. First, we will generate a test vector x on which to apply the filters. Let x be the sum of sinusoids of all integer frequencies from 1Hz to 5kHz. Set t = [0,2], using an sampling frequency of 100kHz. I.e.,

50000

x = X sin(2πft), {0 ≤ t ≤ 2}

f=1

For each filter, follow these steps (you may want to define this in a function so you don’t have to repeat this code). Subplots recommended!

1.    Use the given specifications to produce the lowest-order filter which meets the specs. Either:

(a)    Use filterDesigner to generate a MATLAB function that returns a filter, and then call the function to create the filter object; or

(b)    Use the functions for designing and estimating the order of specific types of filters (e.g., cheby2ord, cheby2) to generate it without filterDesigner. Make sure all the parameters are correctly specified! Refer to the lecture example.

2.    Apply freqz on the filter object to produce a frequency-response plot. Similarly to in HW6, don’t use this to plot the frequency response: manually plot the frequency response, making sure you follow all the same instructions as in HW6 #2d.

3.    Apply the filter to the signal x, defined above.

4.    Plot the Fourier transform of the filtered signal using fft and plot. Refer to the lecture examples for the proper way to use FFT and obtain the proper scaling (use one of the two scaling methods mentioned).

Butterworth

Chebyshev Type I Chebyshev Type IIHPF

LPF

bandstop100kHz5dB

2dB

5dB50dB

40dB

50dBFstop = 10kHz,Fpass = 20kHz

Fstop = 35kHz,Fpass = 15kHz

Fstop = 15kHz,35kHz,Fpass = 5kHz,45kHzEllipticbandpass

5dB50dBFstop = 15kHz,35kHz,Fpass = 20kHz,30kHz

1