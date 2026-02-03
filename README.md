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
## Tabulation for 2.5GB and 10 GB
![WhatsApp Image 2026-02-03 at 8 26 31 PM](https://github.com/user-attachments/assets/f9b86a46-f447-43ea-a2c3-f37f715070e1)

![WhatsApp Image 2026-02-03 at 8 26 42 PM](https://github.com/user-attachments/assets/c2871071-fa90-4cd8-aed4-bf84498822e6)


## High Noise for 2.5 GB
<img width="1920" height="1080" alt="Screenshot (10)" src="https://github.com/user-attachments/assets/9dc191e5-c286-46dd-82a8-fb3b151629dc" />

## Low Noise for 2.5 GB
<img width="1920" height="1080" alt="Screenshot (11)" src="https://github.com/user-attachments/assets/47c8ddb6-b83f-4eb9-a4c4-880cf6ab40ff" />

## High Noise for 10 GB
<img width="1920" height="1080" alt="Screenshot (12)" src="https://github.com/user-attachments/assets/ff0feead-dd0b-4208-b152-ee5a658727b7" />

## Low Noise for 10 GB
<img width="1920" height="1080" alt="Screenshot (13)" src="https://github.com/user-attachments/assets/472545bd-2f3d-4925-96e7-aa8b25b80b0c" />

## Analysis and Report
Compare simulation results with pre-lab calculations and record observations.  
## Description
 Attenuation measurement at 2.5 Gbps and 10 Gbps evaluates the optical power loss in a fiber due to absorption, scattering, and connection losses. This measured attenuation determines the attenuation-limited fiber length, which is the maximum distance the signal can travel while still maintaining sufficient power at the receiver for reliable communication.

## Result :
Thus the attenuation-limited fiber length based on the power budget equation is successfully simulated and verified.

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
