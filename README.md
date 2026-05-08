# BJT-characterization-lab
Experimental analysis and characterization of an NPN Bipolar Junction Transistor (BC547B). Includes 4-quadrant characteristic curve measurements, quiescent point (Q-point) stabilization, and AC signal amplification analysis
# Bipolar Junction Transistor (BJT) Characterization Lab

This repository contains the experimental data, analysis, and circuit configurations for the characterization of a **BC547B NPN Transistor**. The project focuses on determining static parameters (DC) and evaluating dynamic performance (AC) under various biasing conditions.

## 🎯 Objectives
* Measure the **4-Quadrant Characteristic Curves** (Input, Transfer, and Output characteristics).
* Establish a Quiescent Operating Point (Q-Point) at $U_{BE} = 675\text{mV}$.
* Calculate the current gain ($\beta$) and compare it with datasheet specifications.
* Analyze signal amplification and observe large-signal distortion (clipping).

## 🛠️ Hardware Setup
* **Transistor:** BC547B (TO-92 package)
* **Equipment:** * Agilent 33210A Function Generator
    * Tektronix MDO3012 Oscilloscope
    * MetraHit 26S Multimeters
    * HPS Universal Lab Board
* **Key Components:** $1\text{k}\Omega$ Collector Resistor, $100\text{k}\Omega$ Base Resistor, $10\mu\text{F}$ coupling capacitors.

## 📊 Experimental Results

### 1. Static DC Analysis
The target Q-point was set at a base-emitter voltage of **675mV**. 
* **Measured $I_B$:** ~5.1μA
* **Measured $I_C$:** ~0.63mA
* **Calculated $\beta$ (hFE):** $\approx 123$

### 2. Transfer Characteristics (XY Mode)
Using the oscilloscope in XY mode, the transfer characteristic $I_C = f(U_{BE})$ was plotted. The resulting curve demonstrates the exponential relationship of the base-emitter junction and the "knee" voltage where the transistor begins to conduct heavily.

[Insert your 'bodeplot.jpeg' here to show the transfer curve]

### 3. Signal Clipping & Distortion
During AC analysis, the input amplitude was increased to observe the limits of the operating region.
* **Saturation:** Observed when the output signal "flattens" at the bottom.
* **Cutoff:** Observed when the base current is insufficient to maintain the linear region.

<img width="1600" height="1200" alt="BJT,wave" src="https://github.com/user-attachments/assets/e85c3ecb-aca4-411c-a729-7d808c3b4b81" />
<img width="1600" height="1200" alt="BJT,wave" src="https://github.com/user-attachments/assets/2377f42a-9fd6-4c5b-8297-a1e60129afe0" />
<img width="1200" height="1600" alt="Expected Result" src="https://github.com/user-attachments/assets/a8c6a720-d00e-469a-a4e0-9e665c11c791" />



## 🎓 Conclusion
The experiment verified the BC547B's performance within the manufacturer's "B" grouping for gain. The results highlight the importance of proper biasing to avoid signal distortion in amplification stages.
