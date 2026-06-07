# EXP.No: 6: SIMULATION OF AUTOCORRELATION AND PSD USING SCILAB 

# AIM:
Write a program for Autocorrelation and PSD of signals in SCILAB and verify Wiener-Khinchin relation.
# EQUIPMENTS Needed

•	Computer with i3 Processor

•	SCI LAB
# THEORY:
The Wiener-Khinchin theorem states that the power spectral density of a wide sense stationary random process is the Fourier transform of the corresponding autocorrelation function.
<img width="582" height="91" alt="image" src="https://github.com/user-attachments/assets/ec98ecd0-56fd-4e4b-ab09-add2f7d8a651" />
# Algorithm
1.	Load or Define the Signal: Input your time-domain signal.
2.	Compute Autocorrelation: Calculate the autocorrelation function of the signal.
3.	 Compute Power Spectral Density (PSD): Estimate the PSD of the signal, either directly using a method like Welch’s periodogram or by using the Fourier transform of the autocorrelation.
4.	 	Plot Results: Visualize the autocorrelation function and PSD.
# PROCEDURE

•	Refer Algorithms and write code for the experiment.
•	Open SCILAB in System
•	Type your code in New Editor
•	Save the file
•	Execute the code
•	If any Error, correct it in code and execute again
•	Verify the generated waveform using Tabulation and Model Waveform
# PROGRAM:
```
t=0:0.01:2*3.14;
x=sin(2*t);
subplot(3,2,1);
plot(x);
au=xcorr(x,x);
subplot(3,2,2);
plot(au);
v=fft(au);
subplot(3,2,3);
plot(abs(v));
fw=fft(x);
subplot(3,2,4);
plot(fw);
fw2=(abs(fw)).^2;
subplot(3,2,5);
plot(fw2);
```
# OUTPUT:
<img width="765" height="725" alt="image" src="https://github.com/user-attachments/assets/18473478-28ff-4e97-b392-3ef1bfa5c9cb" />


<img width="1516" height="1600" alt="WhatsApp Image 2026-06-07 at 7 48 23 PM" src="https://github.com/user-attachments/assets/bac9c73a-abfd-433a-af95-11c414f6aac0" />



# RESULT :
Thus the Autocorrelation and PSD are executed in Scilab and output is verified.


