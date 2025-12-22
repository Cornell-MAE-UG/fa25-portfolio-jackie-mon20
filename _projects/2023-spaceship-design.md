---
layout: project
title: Spaceship Design
description: Just a spaceship that I designed
technologies: [SolidWorks, Machining]
---

In 2021, NASA asked me to design a spaceship. This project focused on preliminary thermal analysis and heat transfer considerations for a conceptual spacecraft system. The goal was to evaluate energy balances and verify consistency with the second law of thermodynamics.

## Heat Transfer — Hot Side (Heat Lost)

The heat transfer rate on the hot side is calculated as:  

**Q̇<sub>h</sub> = ṁ<sub>h</sub> c<sub>p</sub> (T<sub>h,in</sub> − T<sub>h,out</sub>)**  

Substituting values:

**Q̇<sub>h</sub> = (0.10 kg/s)(4180 J/kg·K)(60 − 45) = 6.27 kW**

---

## Heat Transfer — Cold Side (Heat Gained)

The heat transfer rate on the cold side is:

**Q̇<sub>c</sub> = ṁ<sub>c</sub> c<sub>p</sub> (T<sub>c,in</sub> − T<sub>c,out</sub>)**  

Substituting values:

**Q̇<sub>c</sub> = (0.10 kg/s)(4180 J/kg·K)(34 − 20) = 5.85 kW**

The difference between heat lost on the hot side and heat gained on the cold side is attributed to experimental heat losses and general measurement uncertainty.

---

## Entropy Balance

The general entropy balance is:  

**dS/dt = Σ(Q̇ / T) + ṁ<sub>in</sub> s<sub>in</sub> − ṁ<sub>out</sub> s<sub>out</sub> + Ṡ<sub>gen</sub>**  

For this system:

**Ṡ<sub>gen</sub> = ṁ<sub>h</sub> c<sub>p</sub> ln(T<sub>h,out</sub> / T<sub>h,in</sub>) + ṁ<sub>c</sub> c<sub>p</sub> ln(T<sub>c,out</sub> / T<sub>c,in</sub>)**

Substituting numerical values (temperatures in Kelvin):

**Ṡ<sub>gen</sub> = (0.10 kg/s) [ ln((45 + 273.15)/(60 + 273.15)) + ln((34 + 273.15)/(20 + 273.15)) ] = 0.26 W/K**

Since **Ṡ<sub>gen</sub> > 0**, this confirms irreversibility in the system due to finite temperature differences during heat transfer.

---

## Real-World Achievable Conditions

- **Adiabatic:** Some heat loss to the surroundings is unavoidable, especially in laboratory-scale setups.  
- **Steady state:** Reasonably achieved after reservoir temperatures stabilize.  
- **Kinetic and potential energy changes:** Negligible due to low flow velocities and minimal elevation differences.
