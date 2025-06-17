# Design-and-Implementation-of-PLL-using-90nm-Technology
PLL is a mixed signal circuit as its architecture involves both digital and analog signal  processing units. The present work focuses on the redesign of a PLL system using the  90 nm process technology (GPDK090 library) in CADENCE Virtuoso Analog Design  Environment
# About design and its components
A PLL is a closed-loop feedback system that sets fixed phase relationship between its output clock 
phase and the phase of a reference clock. A PLL is capable of tracking the phase changes that falls in 
this bandwidth of the PLL. A PLL also multiplies a low-frequency reference clock CKref to produce a 
high-frequency clock CKout this is known as clock synthesis.  
A PLL has a negative feedback control system circuit. The main objective of a PLL is to generate 
a signal in which the phase is the same as the phase of a reference signal. This is achieved after many 
iterations of comparison of the reference and feedback signals. In this lock mode the phase of the 
reference and feedback signal is zero. After this, the PLL continues to compare the two signals but 
since they are in lock mode, the PLL output is constant.  
In general, a PLL consists of five main blocks:  
1.Phase Detector or Phase Frequency Detector (PD or PFD)  
2.Charge Pump (CP)   
3.Low Pass Filter (LPF)   
4.Voltage Controlled Oscillator (VCO)  
The “Phase frequency Detector” (PFD) is one of the main parts in PLL circuits. It compares the 
phase and frequency difference between the reference clock and the feedback clock. Depending upon 
the phase and frequency deviation, it generates two output signals “UP” and “DOWN”. The “Charge 
Pump” (CP) circuit is used in the PLL to combine both the outputs of the PFD and give a single output. 
The output of the CP circuit is fed to a “Low Pass Filter” (LPF) to generate a DC control voltage. The 
phase and frequency of the “Voltage Controlled Oscillator” (VCO) output depends on the generated DC control voltage. If the PFD generates an “UP” 
signal, the error voltage at the output of LPF increases which in turn increase the VCO output signal 
frequency. On the contrary, if a “DOWN” signal is generated, the VCO output signal frequency 
decreases. The output of the VCO is then fed back to the PFD in order to recalculate the phase 
difference, and then we can create closed loop frequency control system.         
