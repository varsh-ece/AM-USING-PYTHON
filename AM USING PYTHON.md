## AM USING PYTHON

## FM
EXP NO: 4 GENERATION AND DETECTION OF AM 

## AIM: 
o implement and analyze frequency modulation (FM) using Python's NumPy and Matplotlib libraries.

## EQUIPMENTS REQUIRED

• Computer with i3 Processor • SCI LAB

## THEORY:

Theory of Amplitude Modulation (AM)
AM is an analog modulation technique where the amplitude of a high-frequency carrier wave is varied in proportion to the instantaneous amplitude of a low-frequency message signal (or baseband signal).

PROCEDURE

Install/Import Libraries: Ensure the necessary libraries, NumPy (np) for numerical calculation and Matplotlib (plt) for plotting, are imported. This is done by the first two lines of the code.

Define Parameters: Define the amplitudes (Am, Ac) and frequencies (Fm, Fc, Fs) for the message and carrier signals. These constants determine the characteristics of the generated signals.

Create Time Base: Generate a time vector (t) using np.arange(). This array represents the discrete time points over which the signals will be sampled and calculated.

Generate Signals: Use the defined parameters and the time base (t) to calculate the three required signal arrays: the message signal (m), the carrier signal (c), and the final AM signal (s).

Plot and Visualize: Use the plt.subplot() function to create a figure with three separate axes and plot the three generated signals (m, c, and s) in their respective positions for visual comparison. Finally, use plt.show() to display the generated graph.

Would you like to modify any of the parameters (like frequency or amplitude) to see how the AM


## Program:
```````````````````

import numpy as np
import matplotlib.pyplot as plt

Am = 3.5
Fm = 141
Ac = Am * 2
Fc = 1410
Fs = 14100
t = np.arange(0, 2 / Fm, 1 / Fs)

m = Am * np.cos(2 * np.pi * Fm * t)
c = Ac * np.cos(2 * np.pi * Fc * t)
s = (Ac + m) * np.cos(2 * np.pi * Fc * t)

plt.figure(figsize=(10, 8))

plt.subplot(3, 1, 1)
plt.plot(t, m)

plt.subplot(3, 1, 2)
plt.plot(t, c)

plt.subplot(3, 1, 3)
plt.plot(t, s)

plt.tight_layout()
plt.show()

``````````````````````````````

## Output Waveform

![WhatsApp Image 2025-10-22 at 18 28 25_012cbd34](https://github.com/user-attachments/assets/6a358935-f84c-445e-991a-fdfb1cf4c805)

Tabulation
![WhatsApp Image 2025-11-03 at 08 53 53_b2cf376c](https://github.com/user-attachments/assets/2586cea3-504c-4813-9952-ef428ec317e8)


Calculation
![WhatsApp Image 2025-11-03 at 08 53 53_2cfba46b](https://github.com/user-attachments/assets/9cac5d09-7235-49cd-84fe-bed48a315525)


RESULT:

Thus, the AMPLITUDE  modulation using python  is successfully done and the output is experimentally verified.
