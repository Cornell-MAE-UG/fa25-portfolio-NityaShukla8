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
The RS-25 engine, originally developed as the Space Shuttle Main Engine (SSME), is one of the most advanced liquid-fueled rocket engines ever built, capable of producing over 2 million pounds of thrust by burning liquid hydrogen and liquid oxygen. Initially designed for the Space Shuttle program, where it powered the orbiter during launch and ascent, the RS-25 has been repurposed for NASA’s Space Launch System (SLS), providing propulsion for deep-space missions such as the Artemis program. A critical component of the RS-25 is its De Laval nozzle, a converging-diverging design that efficiently converts the high-pressure, high-temperature combustion gases into directed thrust. In the nozzle, subsonic gases in the converging section accelerate as the cross-sectional area decreases, reach sonic conditions at the throat, and then expand through the diverging section to supersonic speeds, producing high-velocity exhaust that propels the rocket. The flow physics are governed by conservation of mass, momentum, and energy, along with the ideal gas law, and isentropic, quasi-one-dimensional flow. Differences between subsonic and supersonic flow regimes are central to nozzle performance. Thrust is maximized by minimizing entropy generation and avoiding shocks that convert mechanical energy into unusable heat.

The RS-25 engines were used in groups of three on Space Shuttle launches and are now mounted in groups of four on the SLS core stage. On the Shuttle, the engines operated at variable throttle settings to control acceleration and ensure safe orbital insertion. The converging-diverging nozzle maintained near-optimal performance despite changing ambient pressures during ascent. On the SLS, the RS-25 engines provide primary lift-off thrust and continue to accelerate the vehicle from the lower atmosphere into near-vacuum conditions. The nozzle design is also essential for engine reusability and thrust modulation; it must withstand extreme thermal and mechanical loads repeatedly without flow separation or structural damage. Extensive ground testing at NASA’s Space Center validates the nozzle’s performance, ensuring that the flow reaches the correct Mach number distribution along its length and that combustion efficiency and thermal handling are optimized. The geometry of the De Laval nozzle is carefully tuned: subsonic flow accelerates in the converging section, sonic flow occurs at the throat, and supersonic flow expands through the diverging section, converting thermal and pressure energy into kinetic energy efficiently. Ideally, the nozzle expands the exhaust isentropically so that exit pressure matches ambient conditions, maximizing thrust. Any deviation from this—due to altitude changes or imperfect design—can reduce efficiency, highlighting the importance of the RS-25 nozzle’s precise engineering.

**Geometric Justification:** 
The geometry of the RS-25’s De Laval nozzle is critical to achieving optimal thrust and efficient propulsion. In the converging section, the fluid flow is subsonic, and as the cross-sectional area decreases, the gas accelerates, converting pressure energy into kinetic energy. At the throat—the narrowest part of the nozzle—the flow reaches sonic conditions (Mach 1), creating a natural transition point between subsonic and supersonic regimes. Beyond the throat, in the diverging section, the gases expand and accelerate further to supersonic velocities, continuing the conversion of thermal and pressure energy into directed kinetic energy. This geometric arrangement ensures that the engine can efficiently handle a wide range of operating conditions, from sea-level liftoff to near-vacuum in space. The design must also account for altitude variations, as an ideally expanded nozzle maximizes thrust only when the exit pressure matches ambient pressure. Deviations from ideal expansion—over-expanded or under-expanded flow—can generate shock waves or flow separation, reducing efficiency and thrust. In the RS-25, careful engineering of the nozzle contour, throat diameter, and expansion angle ensures that subsonic, sonic, and supersonic domains are correctly delineated, allowing reliable performance across throttle settings, while also supporting reusability of the engine components under extreme thermal and mechanical loads.

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

Thrust depends primarily on the mass flow rate and exhaust velocity, which are functions of the combustion chamber pressure, temperature, and nozzle geometry. Deviations from ideal expansion introduce additional terms accounting for shock losses or flow separation. This analysis is central to the RS-25, where precise nozzle contouring and throat sizing ensure the flow accelerates correctly through subsonic, sonic, and supersonic regimes.

<figure>
  <img src="{{ '/assets/images/flow-relations.png' | relative_url }}" alt="Rocket Nozzle" style="width: 100%; max-width: 600px;">
  <figcaption><em>Figure 3: Mathematical flow relations for de Laval nozzle. </em></figcaption>
</figure>

<figure>
  <img src="{{ '/assets/images/nozzle-im3.png' | relative_url }}" alt="Rocket Nozzle" style="width: 100%; max-width: 600px;">
  <figcaption><em>Figure 4: Control volume for 1D flow. </em></figcaption>
</figure>

**Mathematical Applications to RS-25 Engine:**

(1) Given / Assumed Engine Properties
<ul>
  <li>Combustion temperature: T<sub>c</sub> = 3300 K – typical hydrogen-oxygen combustion temperature</li>
  <li>Gas constant: R = 375 J/kg·K – specific to RS-25 exhaust gas mixture</li>
  <li>Ratio of specific heats: γ = 1.2 – represents high-temperature combustion gas behavior</li>
  <li>Chamber pressure: p<sub>c</sub> – very high, sets energy available; not needed for vacuum calculation</li>
  <li>Nozzle expansion ratio: ε = A<sub>e</sub>/A<sub>t</sub> = 77.5 – RS-25 nozzle geometry optimized for vacuum acceleration</li>
  <li>Ambient pressure in vacuum: p<sub>a</sub> ≈ 0 Pa – simplifies thrust calculation in space</li>
</ul>

(2) Ideal Exhaust Velocity from Isentropic Expansion
<p>The exhaust velocity for an ideal gas expanding through a de Laval nozzle is given by:</p>
<p>v<sub>e</sub> = √[2 γ R T<sub>c</sub> / (γ - 1) * (1 - (p<sub>e</sub>/p<sub>c</sub>)^((γ-1)/γ))]</p>

<p>In vacuum, p<sub>e</sub> ≈ 0, so the bracket term ≈ 1:</p>
<p>v<sub>e,vac</sub> ≈ √(2 γ R T<sub>c</sub> / (γ - 1))</p>

<p>Plug in the RS-25 numbers:</p>
<ul>
  <li>2 × γ = 2 × 1.2 = 2.4</li>
  <li>2.4 × R = 2.4 × 375 = 900</li>
  <li>900 × T<sub>c</sub> = 900 × 3300 = 2,970,000</li>
  <li>Divide by (γ - 1) = 0.2 → 2,970,000 / 0.2 = 14,850,000</li>
  <li>Take square root: v<sub>e,vac</sub> ≈ 3853 m/s</li>
</ul>
<p>Note: The actual RS-25 vacuum velocity is 4460 m/s due to real gas effects and nozzle efficiency.</p>

(3) Exit Pressure from Expansion Ratio
<p>Using isentropic expansion:</p>
<p>p<sub>e</sub>/p<sub>c</sub> = (A<sub>t</sub>/A<sub>e</sub>)^(γ/(γ-1)) = ε^(-γ/(γ-1))</p>
<ul>
  <li>γ/(γ-1) = 1.2 / 0.2 = 6</li>
  <li>p<sub>e</sub>/p<sub>c</sub> = 77.5<sup>-6</sup> ≈ 3.3 × 10<sup>-12</sup> ≈ 0</li>
</ul>
<p>Confirms effectively zero exit pressure in vacuum.</p>

(4) Steady-State Thermodynamic Analysis
<p>Treat the nozzle as a steady-flow device:<p>
<p>ṁ (h<sub>c</sub> + v<sub>c</sub>²/2 + g z<sub>c</sub>) + Q̇ - Ẇ<sub>s</sub> = ṁ (h<sub>e</sub> + v<sub>e</sub>²/2 + g z<sub>e</sub>)</p>
<p>Simplifying for an adiabatic, horizontal nozzle with negligible chamber velocity and potential energy:</p>
<p>h<sub>c</sub> ≈ h<sub>e</sub> + v<sub>e</sub>²/2</p>
<p>Using h = c<sub>p</sub> T for an ideal gas:</p>
<p>v<sub>e</sub> = √(2 c<sub>p</sub> (T<sub>c</sub> - T<sub>e</sub>)) = √(2 γ R / (γ - 1) (T<sub>c</sub> - T<sub>e</sub>))</p>
<p>With T<sub>e</sub> ≈ 0 in vacuum, this reduces to the previous isentropic result.</p>

(5) Mass Flow Rate and Thrust
<p>Choked flow at the throat gives the mass flow rate:</p>
<p>ṁ = p<sub>c</sub> A<sub>t</sub> √(γ / (R T<sub>c</sub>)) (2/(γ+1))^((γ+1)/(2(γ-1)))</p>
<p>Vacuum thrust can then be calculated as:</p>
<p>F = ṁ v<sub>e</sub> + (p<sub>e</sub> - p<sub>a</sub>) A<sub>e</sub> ≈ ṁ v<sub>e</sub></p>
<ul>
  <li>ṁ ≈ 512 kg/s</li>
  <li>v<sub>e</sub> = 4460 m/s</li>
  <li>F ≈ 512 × 4460 ≈ 2.28 × 10<sup>6</sup> N ≈ 2280 kN</li>
</ul>
