---
layout: project
title: Spaceship Design
description: Just a spaceship that I designed
technologies: [SolidWorks, Machining]
---

In 2021, NASA asked me to design a spaceship. This project focused on preliminary thermal analysis and heat transfer considerations for a conceptual spacecraft system. The goal was to evaluate energy balances and verify consistency with the second law of thermodynamics.

## Heat Transfer — Hot Side (Heat Lost)

```text
Q̇_h = ṁ_h c_p (T_h,in − T_h,out)
Q̇_h = (0.10 kg/s)(4180 J/kg·K)(60 − 45)
Q̇_h = 6.27 kW
```

## Heat Transfer — Cold Side (Heat Gained)

```text
Q̇_c = ṁ_c c_p (T_c,in − T_c,out)
Q̇_c = (0.10 kg/s)(4180 J/kg·K)(34 − 20)
Q̇_c = 5.85 kW
```

The difference between heat lost on the hot side and heat gained on the cold side is attributed to experimental heat losses and general measurement uncertainty.

## Entropy Balance

```text
dS/dt = Σ(Q̇ / T) + ṁ_in s_in − ṁ_out s_out + Ṡ_gen
```

```text
Ṡ_gen = ṁ_h c_p ln(T_h,out / T_h,in) + ṁ_c c_p ln(T_c,out / T_c,in)
```

```text
Ṡ_gen = (0.10 kg/s)[ln((45 + 273.15)/(60 + 273.15)) + ln((34 + 273.15)/(20 + 273.15))]
Ṡ_gen = 0.26 W/K
```

```text
Ṡ_gen > 0
```

This confirms irreversibility in the system due to finite temperature differences during heat transfer.

## Real-World Achievable Conditions

- **Adiabatic:** Some heat loss to the surroundings is unavoidable, especially in laboratory-scale setups.
- **Steady state:** Reasonably achieved after reservoir temperatures stabilize.
- **Kinetic and potential energy changes:** Negligible due to low flow velocities and minimal elevation differences.
