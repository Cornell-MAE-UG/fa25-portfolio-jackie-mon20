---
layout: project
title: Thermodynamics Portfolio
description: Thermodynamic Analysis of a Brazed Plate Heat Exchanger (SWEP B10Hx20)
image: /assets/images/function-graph.jpeg
---

### Overview

**Description:** The SWEP B10Hx20 brazed plate heat exchanger is a counter-flow heat exchanger used in HVAC systems, industrial process cooling, heat recovery systems, and refrigeration and heat pump loops. It consists of thin stainless-steel plates brazed together with copper, forming hot and cold flow channels that promote high heat transfer coefficients while maintaining a small footprint.

**How it works:** Hot fluid enters one side of the exchanger while cold fluid enters from the opposite side, creating counter-flow operation. Heat is transferred by convection from the hot fluid to the plate, by conduction through the plate, and by convection from the plate to the cold fluid.

**Real-world relevance:** Similar exchangers are used in district heating plants, automotive thermal management systems, and industrial energy recovery, making this device relevant to mechanical thermal systems.

**Assumptions:**  
Steady State; Negligible kinetic energy and potential energy changes; No shaft work; Heat transfer occurs only between the fluids.

Control Volume: Entire heat exchanger  
Type: Steady-state, steady-flow control volume

<hr>

### System Diagram

The figure below shows a control-volume diagram of the brazed plate heat exchanger operating in counter-flow. Mass flow rates and inlet and outlet temperatures are labeled for both the hot and cold fluid streams. Heat transfer occurs internally between the streams, with no shaft work interaction.

<p align="center">
  <img src="C:\Users\monah\fa25-portfolio-jackie-mon20\assets\images\old-radio.jpg" width="600">
</p>

<hr>

### Data

| Parameter | Value |
|----------|-------|
| Hot Fluid | Water |
| Cold Fluid | Water |
| m_h | 0.10 kg/s |
| m_c | 0.10 kg/s |
| T_h,in | 60 °C |
| T_h,out | 45 °C |
| T_c,in | 20 °C |
| T_c,out | 34 °C |

<hr>

### Heat Transfer Hot Side (Heat Lost)

The heat transfer rate on the hot side is calculated as:  

Q̇_h = m_h c_p (T_h,in − T_h,out)  

Q̇_h = (0.10 kg/s)(4180 J/kg·K)(60 − 45) = **6.27 kW**

<hr>

### Heat Transfer Cold Side (Heat Gained)

Q̇_c = m_c c_p (T_c,out − T_c,in)  

Q̇_c = (0.10 kg/s)(4180 J/kg·K)(34 − 20) = **5.85 kW**

The difference between heat lost on the hot side and heat gained on the cold side is attributed to experimental heat losses and general measurement uncertainty.

<hr>

### Entropy Balance

dS/dt = Σ(Q̇ / T) + Σ ṁ_in s_in − Σ ṁ_out s_out + Ṡ_gen  

Ṡ_gen = m_h c_p ln(T_h,out / T_h,in) + m_c c_p ln(T_c,out / T_c,in)  

Ṡ_gen = (0.10 kg/s) [ ln((45+273.15)/(60+273.15)) + ln((34+273.15)/(20+273.15)) ] = **0.26 W/K**

Since Ṡ_gen > 0, this confirms irreversibility due to finite temperature differences during heat transfer.

<hr>

### Real-World Achievable Conditions

- **Adiabatic:** Some heat loss to the surroundings is unavoidable  
- **Steady state:** Achieved after reservoir temperatures stabilize  
- **Kinetic and potential energy changes:** Negligible

<hr>

### Sources

- SWEP Heat Exchangers – Product Overview and Technical Notes  
- ASHRAE Handbook – HVAC Systems and Equipment
