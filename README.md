# Attenuation Measurement 2.5 GB & 10 GB
# Attenuation-Limited Fiber Length

## Objective
- Calculate the attenuation-limited fiber length based on the power budget equation.  
- Simulate the resulting system and verify that it meets performance objectives.

---

## Theory
The **power budget equation** states that the power budget in a transmission system must equal the sum of all power losses plus the power margin.  

The power budget is the difference between the transmitter output power and the receiver sensitivity in dBm:

\[
P_T - S_R = A \cdot L_F + L_C + L_A + M
\]

Where:
- **PT** = transmitter output power (dBm)  
- **SR** = receiver sensitivity (dBm)  
- **A** = fiber attenuation (dB/km)  
- **LF** = fiber length (km)  
- **LC** = coupling loss (dB)  
- **LA** = additional known losses (dB)  
- **M** = power margin (dB)  

In this exercise, all parameters are given except the fiber length, which must be determined.  

The **receiver sensitivity** is defined as the minimum power required to achieve a BER of \(10^{-9}\), corresponding to a Q factor of 6.  
- Receiver sensitivity depends on the bit rate.  
- Fiber attenuation depends on the operating wavelength.  

---

## Pre-lab Calculations
Using the power budget equation and the parameters below, determine the attenuation-limited fiber length:

- **Transmitter output power:** 0 dBm  
- **Operating wavelength:** 1550 nm  
- **Bit rate:** 2.5 Gb/s  
- **Receiver sensitivity:** -30 dBm  
- **Fiber attenuation:** 0.19 dB/km  
- **Number of connectors:** 2  
- **Loss per connector:** 0.5 dB  
- **Additional known losses:** 0 dB  
- **Power margin:** 6 dB  

---

## Layout
- The system has been created using **OptiSystem** and exported as an **OptiPerformer** file.  
- Two versions exist: one for **2.5 Gb/s** and one for **10 Gb/s**.  
- Work with the **2.5 Gb/s** version first.  
- An optical attenuator represents connector loss and system margin.  
- Adjust parameters according to the table above.  
- Dispersion and nonlinear effects in the fiber are disabled.  
- To set the receiver sensitivity to -30 dBm for 2.5 Gb/s, set the **thermal noise parameter** in the receiver to **8.97e-24 W/Hz**.  
- Visualizer components are included to obtain necessary simulation data.  

---

## Simulation
1. Run the simulation and record:
   - **Optical power levels (dBm):**
     - Both ends of fiber  
     - Receiver input  
   - **BER analysis:**
     - BER  
     - Q factor  
     - Eye diagram  

2. Set the fiber length to **125% of the calculated pre-lab value** and repeat the simulation and data recording.  

---
## TABULATION OF 2.5GB

![2 5 GB](https://github.com/user-attachments/assets/d855c726-e0c3-441e-a4f6-4b62c9d286db)

## LOW NOISE FOR 2.5GB
<img width="969" height="728" alt="2 5GB LOW - NOISE" src="https://github.com/user-attachments/assets/641e1a0d-e4ed-4c27-8e1d-ebc57ceacbb7" />
## HIGH NOISE FOR 2.5GB
<img width="965" height="732" alt="2 5GB HIGH - NOISE" src="https://github.com/user-attachments/assets/376b9d64-e12f-4e1f-93eb-c808778d639d" />

## TABULATION OF 10GB

![10 GB](https://github.com/user-attachments/assets/9bd0ba93-54d0-4eab-8834-845b7167e461)

## LOW NOISE FOR 10GB
<img width="969" height="737" alt="10GB LOW - NOISE" src="https://github.com/user-attachments/assets/58c5eb01-f727-4b9e-9a81-96958f303601" />
## HIGH NOISE FOR 10GB
<img width="968" height="734" alt="10GB HIGH - NOISE" src="https://github.com/user-attachments/assets/fab55ecf-bf6e-46fa-9872-b345fdf7cfd3" />


## Analysis and Report
Compare simulation results with pre-lab calculations and record observations.  

Your report should contain:
- **Cover Page**
  - Title of the lab  
  - Course name and number  
  - Your name  

- **Pre-lab Calculations**  

- **Screenshots** of layout and results (including eye diagrams)  

- **Summary Table** for each simulation:
  | Fiber Length (km) | Received Power (dBm) | Q Factor | BER |
  |-------------------|-----------------------|----------|-----|
  

- **Written Summary** of observations and explanations of differences.



## Result

Thus the Attenuation of 10GB and 2.5GB was observed and calculated.
