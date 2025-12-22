---
layout: project
title: Thermodynamics Portfolio
description: Thermodynamic Analysis of a Brazed Plate Heat Exchanger (SWEP B10Hx20)
image: /assets/images/function-graph.png
image2: /assets/images/old-radio.png
---

### Overview

**Description:**  
The SWEP B10Hx20 brazed plate heat exchanger is a counter-flow heat exchanger used in HVAC systems, industrial process cooling, heat recovery systems, and refrigeration and heat pump loops. It consists of thin stainless-steel plates brazed together with copper, forming alternating hot and cold flow channels.

**How it works:**  
Hot fluid enters one side of the exchanger while cold fluid enters from the opposite side, creating a counter-flow system. Heat is transferred by convection from the hot fluid to the plate, by conduction through the plate, and by convection from the plate to the cold fluid.

**Real-world relevance:**  
Similar heat exchangers are used in district heating plants, automotive thermal management systems, and industrial energy recovery, making this device highly relevant to mechanical and thermal systems.

**Assumptions:**  
- Steady state  
- Incompressible liquid water  
- Constant specific heat  
- Negligible kinetic and potential energy changes  
- No shaft work  
- Heat transfer occurs only between the two fluid streams 

**System definition:**  
Control Volume: Entire heat exchanger  
Type: Steady-state, steady-flow control volume  

---

### Data

| Parameter | Value |
|----------|-------|
| Hot Fluid | Water |
| Cold Fluid | Water |
| ṁ<sub>h</sub> | 0.10 kg/s |
| ṁ<sub>c</sub> | 0.10 kg/s |
| T<sub>h,in</sub> | 60 °C |
| T<sub>h,out</sub> | 45 °C |
| T<sub>c,in</sub> | 20 °C |
| T<sub>c,out</sub> | 34 °C |

---

### Challenging Adiabatic Assumption

**Heat Transfer Hot Side (Heat Lost)**

If we consider the CV to be just the hot fluid and its flow that is loosing Q̇<sub>h</sub>

Q̇<sub>h</sub> = ṁ<sub>h</sub> c<sub>p</sub> (T<sub>h,in</sub> − T<sub>h,out</sub>)  

Q̇<sub>h</sub> = (0.10 kg/s)(4180 J/kg·K)(60 − 45)  

**Q̇<sub>h</sub> = 6.27 kW**\


**Heat Transfer Cold Side (Heat Gained)**

If we consider the CV to be just the cold fluid and its flow that is gaining Q̇<sub>c</sub>

The heat transfer rate on the cold side is calculated as:

Q̇<sub>c</sub> = ṁ<sub>c</sub> c<sub>p</sub> (T<sub>c,out</sub> − T<sub>c,in</sub>)  

Q̇<sub>c</sub> = (0.10 kg/s)(4180 J/kg·K)(34 − 20)  

**Q̇<sub>c</sub> = 5.85 kW**

The difference between heat lost on the hot side and heat gained on the cold side is attributed to measurement uncertainty, property assumptions, and minor external heat losses.

---

### Entropy Balance

The general entropy balance for a control volume is:

dS/dt = Σ(Q̇ / T) + Σṁ<sub>in</sub> s<sub>in</sub> − Σṁ<sub>out</sub> s<sub>out</sub> + Ṡ<sub>gen</sub>  

Assuming incompressible liquid water with constant specific heat and negligible pressure drop, the entropy generation rate for this heat exchanger is:

Ṡ<sub>gen</sub> = ṁ<sub>h</sub> c<sub>p</sub> ln(T<sub>h,out</sub> / T<sub>h,in</sub>)  
     + ṁ<sub>c</sub> c<sub>p</sub> ln(T<sub>c,out</sub> / T<sub>c,in</sub>)  

Ṡ<sub>gen</sub> = (0.10)(4180)  
[ ln((45 + 273.15)/(60 + 273.15)) + ln((34 + 273.15)/(20 + 273.15)) ]  

**Ṡ<sub>gen</sub> = 0.26 W/K**

Since Ṡ<sub>gen</sub> > 0, this confirms irreversibility in the system due to finite temperature differences during heat transfer.

---

### Design Change Consideration

If instead the heat exchanger operated in parallel flow, not counter-flow, both fluids would enter at the same end of the exchanger. This would cause the temperature difference between the two streams to decrease rapidly along the flow length.

As a result:
- The overall heat transfer rate would decrease  
- The exchanger effectiveness would be reduced  
- Entropy generation would increase  

This explains why compact brazed plate heat exchangers such as the SWEP B10Hx20 are typically designed for counter-flow operation rather than parallel.

---

### Design Change Consideration (Quantitative Analysis)

If the heat exchanger were operated in parallel flow instead of counter-flow, both the hot and cold fluids would enter from the same end of the exchanger. To evaluate the impact of this change, the log mean temperature difference (LMTD) is compared for both configurations.

**Counter-flow LMTD:**  

ΔT₁ = T<sub>h,in</sub> − T<sub>c,out</sub> = 60 − 34 = 26 °C  
ΔT₂ = T<sub>h,out</sub> − T<sub>c,in</sub> = 45 − 20 = 25 °C  

ΔT<sub>lm,CF</sub> = (ΔT₁ − ΔT₂) / ln(ΔT₁ / ΔT₂)  

ΔT<sub>lm,CF</sub> ≈ 25.5 °C  

**Parallel-flow LMTD:**  

ΔT₁ = T<sub>h,in</sub> − T<sub>c,in</sub> = 60 − 20 = 40 °C  
ΔT₂ = T<sub>h,out</sub> − T<sub>c,out</sub> = 45 − 34 = 11 °C  

ΔT<sub>lm,PF</sub> = (40 − 11) / ln(40 / 11)  

ΔT<sub>lm,PF</sub> ≈ 22.5 °C  

Heat transfer rate is proportional to the LMTD:

Q̇ ∝ ΔT<sub>lm</sub>  

Q̇<sub>PF</sub> / Q̇<sub>CF</sub> ≈ 22.5 / 25.5 ≈ 0.88  

This shows that operating the heat exchanger in parallel flow reduces the heat transfer rate by about 12% compared to counter flow.

---

**Effectiveness Consideration:**  

The maximum possible heat transfer rate is:

Q̇<sub>max</sub> = ṁ<sub>min</sub> c<sub>p</sub> (T<sub>h,in</sub> − T<sub>c,in</sub>)  

Q̇<sub>max</sub> = (0.10)(4180)(60 − 20) = 16.7 kW  

For counter-flow operation:

ε<sub>CF</sub> = Q̇<sub>actual</sub> / Q̇<sub>max</sub>  
ε<sub>CF</sub> = 6.27 / 16.7 = 0.38  

Parallel-flow operation results in a lower heat transfer rate, so effectiveness decreases to:

ε<sub>PF</sub> ≈ 0.33  

---

**Entropy and Second-Law:**  

Parallel-flow operation leads the temperature difference between the hot and cold fluids to decrease signifigantly near the inlet, increasing irreversibility during heat transfer, causing:

- The driving temperature difference to reduce  
- Entropy generation to increases for a given heat transfer 
- Second-law efficiency is reduced  

---

**Conclusion:**  

Counter-flow operation provides higher heat transfer rates, greater effectiveness, and lower entropy generation compared to parallel-flow operation. This quantitative comparison explains why compact brazed plate heat exchangers such as the SWEP B10Hx20 are designed to operate in counter-flow configurations.

### Sources

- SWEP International AB – *B10HX Brazed Plate Heat Exchanger Product Datasheet*   
- ASHRAE Handbook – HVAC Systems and Equipment