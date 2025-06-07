# RC Circuit Modeling and Analysis – ME 351

## Overview
This project involved modeling and analyzing an RC (Resistor-Capacitor) circuit subject to a rectangular pulse input. The switch initiates charging and discharging phases based on the pulse duration. Two scenarios were evaluated to observe transient behavior.

## Objective
- Model a first-order RC circuit
- Simulate voltage across the capacitor (Vc) when subjected to a rectangular pulse
- Compare system response for pulse durations t₁ = 2τ and t₁ = 4τ
- Visualize and analyze transient responses using MATLAB and Simscape

## Circuit Description
- Voltage Source (Vs): 10V
- Time Constant (RC or τ): 10s
- Initial capacitor voltage: 0V (fully discharged)
- Pulse durations: 
  - Case 1: t₁ = 2τ = 20s
  - Case 2: t₁ = 4τ = 40s

## Methodology
- Solved differential equations for capacitor charging and discharging:
  - Charging: Vc(t) = Vs(1 - e^(-t/RC))
  - Discharging: Vc(t) = Vc(t₁)e^(-(t - t₁)/RC)
- Plotted Vc vs normalized time (t/τ) for both cases
- Used MATLAB for simulation and visualization
- Modeled in Simscape to validate analytical results

## Results
- **Case 1 (t₁ = 2τ):** Capacitor charges ~86.5% of Vs before discharging
- **Case 2 (t₁ = 4τ):** Capacitor charges ~98.2% of Vs before discharging
- Discharge phase followed expected exponential decay behavior
- Visual plots demonstrated time constant effects clearly

## Tools Used
- MATLAB for simulation, plotting, and data analysis
- Simscape for visual circuit modeling and dynamic simulation

## Authors
- Abbas Hussain and team, Spring 2024
- Course: ENME 351 – First Order Differential Equations
- Instructor: Department of Mechanical Engineering, George Mason University

