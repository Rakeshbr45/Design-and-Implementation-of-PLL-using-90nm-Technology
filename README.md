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

# Block Diagram
![image](https://github.com/user-attachments/assets/b7105873-ee47-45d4-9986-954e0bcf849a)

# PLL design implementation using Cadence

#Phase Frequency Detector
![image](https://github.com/user-attachments/assets/103d863f-43ce-4775-9467-aea13a7e5eae)

Operation of PFD
![image](https://github.com/user-attachments/assets/1abbced6-cedd-4b02-b19c-e432e5b660dd)

Schematic Design
![image](https://github.com/user-attachments/assets/06c0e4af-49ef-45ac-8daf-e2f769fac37c)

# Charge Pump and Loop Filter
![image](https://github.com/user-attachments/assets/a00d498a-6a4c-497b-a3de-13fbf61fc12d)
![image](https://github.com/user-attachments/assets/76c03374-9fa8-43a9-8351-69b3be0d7b5c)

Schematic Design
![image](https://github.com/user-attachments/assets/7164799c-2b6a-4356-9523-93025a191a9d)

# Voltage Controlled Oscillator
![image](https://github.com/user-attachments/assets/24b032ea-89b0-42e5-9527-2d8b35ca08ce)

Schematic Design
![image](https://github.com/user-attachments/assets/fb3d19f3-d7bc-4be0-9f9a-44bfd1054bc4)

# Simulation Result
![image](https://github.com/user-attachments/assets/305a2be5-e6f7-4661-beb9-e69a235bb22f)

# VCO Output
![image](https://github.com/user-attachments/assets/0b61d8af-fb99-42f2-8fc8-cc38d1916459)

# PLL Schematic
![image](https://github.com/user-attachments/assets/748285d8-55b2-4a44-8a84-bdc8fd485669)









