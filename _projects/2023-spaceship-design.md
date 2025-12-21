---
layout: project
title: Spaceship Design
description: Just a spaceship that I designed
technologies: [SolidWorks, Machining]
---


In 2021, NASA asked me to design a spaceship...Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut nec accumsan leo. Pellentesque ornare orci enim, vitae vestibulum nibh rutrum in. Donec pharetra risus nec ipsum fringilla, et mattis tortor auctor. Duis tortor ante, posuere ut odio a, scelerisque interdum purus. Aenean faucibus luctus est, sed bibendum tellus. Nulla et magna urna. Morbi a ipsum sollicitudin, rhoncus risus volutpat, ultricies nunc. Quisque mollis finibus ante id imperdiet. Quisque vehicula elit sit amet felis facilisis fermentum.

**Heat Transfer Hot Side (heat lost):**
Q̇_h = ṁhcp(T_h,in  - Th, out) = (0.10 kg/s)(4180 J/kgk)(60 ℃-45 ℃) 
Q̇_h =6.27kW

Heat Transfer Cold Side:
Q̇<sub>c</sub> = ṁccp(Tc, in-Tc, out) = (0.10 kg/s)(4180 J/kgk)(34 ℃-20 ℃) 
Q̇_c =5.85 kW

This difference in heat gained and heat loss can be assumed to be from experimental heat loss, and general measurement uncertainties. 


Entropy Balance:
dS/dt=QTb+ṁinsin-ṁoutsout+Ṡgen
Ṡgen=ṁh(sh, out-sh, in)+ṁc(sc, out-sc, in)
Ṡgen=ṁccpln(Tc, outTc, in)+ṁhcpln(Th, outTh, in)=ṁccp[ln(Tc, outTc, in)+ln(Th, outTh, in)]
Ṡgen=(0.10 kg/s)[ln(34+273.1520+273.15)+ln(45+273.1560+273.15)]=0.26 W/K
Ṡgen> 0  confirming irreversibility in this system, as expected due to finite temperature differences


Real world Achievable Conditions?
Adiabatic: There will be some heat loss to surroundings, especially in lab setups without insulation.
Steady state: Can mostly be achieved after reservoir temperatures stabilize.
Kinetic energy changes: Negligible due to low flow velocities and small elevation changes.

