---
layout: project
title: Thermodynamics Portfolio
description: Thermodynamic Analysis of a Brazed Plate Heat Exchanger (SWEP B10Hx20)
image: /assets/images/function-graph.jpeg
---

### Overview

**Description:**  
The SWEP B10Hx20 brazed plate heat exchanger is a counter-flow heat exchanger used in HVAC systems, industrial process cooling, heat recovery systems, and refrigeration and heat pump loops. It consists of thin stainless-steel plates brazed together with copper, forming alternating hot and cold flow channels. The plate corrugations increase turbulence and heat transfer coefficients while maintaining a compact footprint.

**How it works:**  
Hot fluid enters one side of the exchanger while cold fluid enters from the opposite side, creating counter-flow operation. Heat is transferred by convection from the hot fluid to the plate, by conduction through the plate, and by convection from the plate to the cold fluid.

**Real-world relevance:**  
Similar heat exchangers are used in district heating plants, automotive thermal management systems, and industrial energy recovery, making this device highly relevant to mechanical and thermal systems.

**Assumptions:**  
- Steady state operation  
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

### Heat Transfer Hot Side (Heat Lost)

The heat transfer rate on the hot side is calculated as:

Q̇<sub>h</sub> = ṁ<sub>h</sub> c<sub>p</sub> (T<sub>h,in</sub> − T<sub>h,out</sub>)  

Q̇<sub>h</sub> = (0.10 kg/s)(4180 J/kg·K)(60 − 45)  

Q̇<sub>h</sub> = **6.27 kW**

---

### Heat Transfer Cold Side (Heat Gained)

The heat transfer rate on the cold side is calculated as:

Q̇<sub>c</sub> = ṁ<sub>c</sub> c<sub>p</sub> (T<sub>c,out</sub> − T<sub>c,in</sub>)  

Q̇<sub>c</sub> = (0.10 kg/s)(4180 J/kg·K)(34 − 20)  

Q̇<sub>c</sub> = **5.85 kW**

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

Ṡ<sub>gen</sub> = **0.26 W/K**

Since Ṡ<sub>gen</sub> > 0, this confirms irreversibility in the system due to finite temperature differences during heat transfer.

---

### Design / Operating Condition Change

If the heat exchanger were operated in **parallel flow** instead of counter-flow, both fluids would enter at the same end of the exchanger. This would cause the temperature difference between the two streams to decrease rapidly along the flow length.

As a result:
- The overall heat transfer rate would decrease  
- The exchanger effectiveness would be reduced  
- Entropy generation would increase  

This explains why compact brazed plate heat exchangers such as the SWEP B10Hx20 are typically designed for counter-flow operation.

---

### Real-World Achievable Conditions

- **Adiabatic behavior:** External heat losses are minimized but not completely eliminated in practice.  
- **Steady state:** Reasonably achieved once reservoir temperatures stabilize.  
- **Kinetic and potential energy changes:** Negligible due to low flow velocities and minimal elevation differences.  

---

### Sources

- SWEP International AB – *B10HX Brazed Plate Heat Exchanger Product Datasheet*   
- ASHRAE Handbook – HVAC Systems and Equipment