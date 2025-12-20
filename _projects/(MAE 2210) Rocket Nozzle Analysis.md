---
layout: project
title: Rocket Nozzle Analysis
description: Thermodynamics Device Application
technologies: [N/A]
image: /assets/images/rocket-nozzle.png
---
**Model Type:** Space Shuttle Main Engine (SSME)/RS-25: De Laval Nozzle (Converging-Diverging)

<figure>
  <img src="{{ '/assets/images/sls-engine.jpg' | relative_url }}" alt="Rocket Nozzle" style="width: 100%; max-width: 600px;">
  <figcaption><em>Figure 1: RS-25 engine for SLS Artemis I mission to Moon. </em></figcaption>
</figure>

**Overview:** 
The RS-25 engine, originally developed as the Space Shuttle Main Engine (SSME), is one of the most advanced liquid-fueled rocket engines ever built, capable of producing over 2 million pounds of thrust by burning liquid hydrogen and liquid oxygen. Initially designed for the Space Shuttle program, where it powered the orbiter during launch and ascent, the RS-25 has been repurposed for NASA’s Space Launch System (SLS), providing propulsion for deep-space missions such as the Artemis program. A critical component of the RS-25 is its De Laval nozzle, a converging-diverging design that efficiently converts the high-pressure, high-temperature combustion gases into directed thrust. In the nozzle, subsonic gases in the converging section accelerate as the cross-sectional area decreases, reach sonic conditions at the throat, and then expand through the diverging section to supersonic speeds, producing high-velocity exhaust that propels the rocket. The flow physics are governed by conservation of mass, momentum, and energy, along with the ideal gas law, and assume an isentropic, quasi-one-dimensional flow. Differences between subsonic and supersonic flow regimes are central to nozzle performance, and thrust is maximized by minimizing entropy generation and avoiding shocks that convert mechanical energy into unusable heat.

In practical applications, the RS-25 engines were used in groups of three on Space Shuttle launches and are now mounted in groups of four on the SLS core stage. During Shuttle launches, the engines needed to operate at variable throttle settings to manage acceleration and orbital insertion safely, while the converging-diverging nozzle maintained near-optimal performance across the changing ambient pressures of ascent. On the SLS, the RS-25 engines provide primary lift-off thrust and continue to accelerate the vehicle through the lower atmosphere into near-vacuum conditions, critical for sending crewed missions or cargo to lunar orbit. The nozzle design is also essential for engine reusability and thrust modulation; it must withstand extreme thermal and mechanical loads repeatedly without flow separation or structural damage. Extensive ground testing at NASA’s Stennis Space Center validates the nozzle’s performance, ensuring that the flow reaches the correct Mach number distribution along its length and that combustion efficiency and thermal handling are optimized. The geometry of the De Laval nozzle is carefully tuned: subsonic flow accelerates in the converging section, sonic flow occurs at the throat, and supersonic flow expands through the diverging section, converting thermal and pressure energy into kinetic energy efficiently. Ideally, the nozzle expands the exhaust isentropically so that exit pressure matches ambient conditions, maximizing thrust. Any deviation from this—due to altitude changes or imperfect design—can reduce efficiency, highlighting the importance of the RS-25 nozzle’s precise engineering. In summary, the De Laval nozzle in the RS-25 engine is not only a cornerstone of high-thrust performance but also a carefully optimized system enabling both variable operation and reusability across the extreme conditions of modern spaceflight.

**Geometric Justification:** 
The geometry of the RS-25’s De Laval nozzle is critical to achieving optimal thrust and efficient propulsion. In the converging section, the fluid flow is subsonic, and as the cross-sectional area decreases, the gas accelerates, converting pressure energy into kinetic energy. At the throat—the narrowest part of the nozzle—the flow reaches sonic conditions (Mach 1), creating a natural transition point between subsonic and supersonic regimes. Beyond the throat, in the diverging section, the gases expand and accelerate further to supersonic velocities, continuing the conversion of thermal and pressure energy into directed kinetic energy. This geometric arrangement ensures that the engine can efficiently handle a wide range of operating conditions, from sea-level liftoff to near-vacuum in space. The design must also account for altitude variations, as an ideally expanded nozzle maximizes thrust only when the exit pressure matches ambient pressure. Deviations from ideal expansion—over-expanded or under-expanded flow—can generate shock waves or flow separation, reducing efficiency and thrust. In the RS-25, careful engineering of the nozzle contour, throat diameter, and expansion angle ensures that subsonic, sonic, and supersonic domains are correctly delineated, allowing reliable performance across throttle settings and multiple missions, while also supporting reusability of the engine components under extreme thermal and mechanical loads.

<figure>
  <img src="{{ '/assets/images/nozzle-im1.png' | relative_url }}" alt="Rocket Nozzle" style="width: 100%; max-width: 600px;">
  <figcaption><em>Figure 2: Thrust equation and diagram of rocket engine. </em></figcaption>
</figure>

**Mathematical Analysis:** 
The performance of the RS-25 nozzle can be analyzed mathematically using principles of fluid mechanics and thermodynamics. By combining the conservation of mass, momentum, and energy with the ideal gas law, and assuming an isentropic flow, the quasi-one-dimensional behavior of the exhaust gases can be described. In the converging section, for subsonic flow (Mach number M < 1), the continuity equation shows that decreasing area results in increasing velocity, while pressure and density decrease. At the throat, the Mach number reaches 1, and the flow properties satisfy the condition for choked flow. Beyond the throat, in the diverging section, supersonic expansion (M > 1) occurs, and the gas accelerates further as the cross-sectional area increases, while pressure, temperature, and density decrease. The ideal thrust of the nozzle is calculated using F = ṁ vₑ + (pₑ - pₐ) Aₑ where:
- ṁ = mass flow rate (kg/s)  
- vₑ = exhaust velocity (m/s)  
- pₑ = exit pressure (Pa)  
- pₐ = ambient pressure (Pa)  
- Aₑ = nozzle exit area (m²)

Thrust depends primarily on the mass flow rate and exhaust velocity, which are functions of the combustion chamber pressure, temperature, and nozzle geometry. Deviations from ideal expansion introduce additional terms accounting for shock losses or flow separation. This analysis is central to the RS-25, where precise nozzle contouring and throat sizing ensure the flow accelerates correctly through subsonic, sonic, and supersonic regimes, maximizing thrust while minimizing energy losses and maintaining engine integrity across multiple launches.

<figure>
  <img src="{{ '/assets/images/flow-relations.png' | relative_url }}" alt="Rocket Nozzle" style="width: 100%; max-width: 600px;">
  <figcaption><em>Figure 3: Mathematical flow relations for de Laval nozzle. </em></figcaption>
</figure>

<figure>
  <img src="{{ '/assets/images/nozzle-im3.png' | relative_url }}" alt="Rocket Nozzle" style="width: 100%; max-width: 600px;">
  <figcaption><em>Figure 4: Control volume for 1D flow. </em></figcaption>
</figure>

**Conceptual Applications to RS-25 Engine:**

calculation for expansion ratio - 77.5:1
Ue = 4460 m/s and 452 s^-1 in vacuum owing to a much higher combuster temperature (3300 K) and more favorable fluid properties (R = 375 J/kg-K; gamma = 1.2) stemming from combustion of liquid hydrogen and liquid oxygen
