---
layout: project
title: Thermodynamics Portfolio
description: Thermodynamic Analysis of a Brazed Plate Heat Exchanger (SWEP B10Hx20)
image: /assets/images/function-graph.jpeg
---

### Overview:

**Description:** The SWEP B10Hx20 brazed plate heat exchanger is a  counter-flow heat exchanger used in HVAC systems, industrial process cooling, heat recovery systems, and refrigeration and heat pump loops. It consists of thin stainless-steel plates brazed together with copper, forming hot and cold flow channels that promote high heat transfer coefficients while maintaining a small footprint.

**How it works:** Hot fluid enters one side of the exchanger while cold fluid enters from the opposite side, creating counter-flow operation. Heat is transferred by convection from the hot fluid to the plate, by conduction through the plate,  and by convection from the plate to the cold fluid

**Real-world relevance:** Similar exchangers are used in district heating plants, automotive thermal management systems, and industrial energy recovery, which makes this device relevent to mechanical thermal systems.

**Assumptions:** 
Steady State;  Negligible kinetic energy and potential energy changes; No shaft work; Adiabatic externally (there is only heat transfer between the fluids)

Use control volume to analyze this thermodynamic system
Control Volume: Entire heat exchanger
Type: Steady-state, steady-flow control volume

---

### System Diagram

The figure below shows a control-volume diagram of the brazed plate heat exchanger operating in counter-flow. Mass flow rates and inlet and outlet temperatures are labeled for both the hot and cold fluid streams. Heat transfer occurs internally between the streams, with no shaft work interaction.

<p align="center">
  <img src="assets/images/old-radio.jpg" width="600">
</p>

---

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

---

### Heat Transfer Hot Side (Heat Lost)

The heat transfer rate on the hot side is calculated as:  

Q̇<sub>h</sub> = ṁ<sub>h</sub> c<sub>p</sub> (T<sub>h,in</sub> − T<sub>h,out</sub>)  

Q̇<sub>h</sub> = (0.10 kg/s)(4180 J/kg·K)(60 − 45) = **6.27 kW**

---

### Heat Transfer Cold Side (Heat Gained)

The heat transfer rate on the cold side is:

Q̇<sub>c</sub> = ṁ<sub>c</sub> c<sub>p</sub> (T<sub>c,out</sub> − T<sub>c,in</sub>)  

Q̇<sub>c</sub> = (0.10 kg/s)(4180 J/kg·K)(34 − 20) = **5.85 kW**

The difference between heat lost on the hot side and heat gained on the cold side is attributed to experimental heat losses and general measurement uncertainty.

---

### Entropy Balance

General entropy balance is:  

dS/dt = Σ(Q̇ / T) + Σṁ<sub>in</sub> s<sub>in</sub> − Σṁ<sub>out</sub> s<sub>out</sub> + Ṡ<sub>gen</sub>  

For this system:

Ṡ<sub>gen</sub> = ṁ<sub>h</sub> c<sub>p</sub> ln(T<sub>h,out</sub> / T<sub>h,in</sub>) + ṁ<sub>c</sub> c<sub>p</sub> ln(T<sub>c,out</sub> / T<sub>c,in</sub>)

Ṡ<sub>gen</sub> = (0.10 kg/s) [ ln((45 + 273.15)/(60 + 273.15)) + ln((34 + 273.15)/(20 + 273.15)) ] = **0.26 W/K**

Since Ṡ<sub>gen</sub> > 0, this confirms irreversibility in the system due to finite temperature differences during heat transfer.

---

### Real-World Achievable Conditions

- **Adiabatic:** Some heat loss to the surroundings is unavoidable, especially in laboratory-scale setups.  
- **Steady state:** Reasonably achieved after reservoir temperatures stabilize.  
- **Kinetic and potential energy changes:** Negligible due to low flow velocities and minimal elevation differences.

---

### Sources:

SWEP Heat Exchangers – Product Overview and Technical Notes

ASHRAE Handbook – HVAC Systems and Equipment
