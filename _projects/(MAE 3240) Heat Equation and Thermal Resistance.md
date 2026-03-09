---
layout: project
title: Heat Equation & Thermal Resistance
description: Assignment Upload
technologies: [Numerical Calculation]
image: /assets/images/thermometer.png
---

**Overview:**

Problem Set 3 was one of the most valuable and educational assignments in the course because it required the implementation of the heat equation in finding the spatial temperature profile of objects. The first two problems involved applying the heat equation to derive the governing equation and determine the temperature distribution within a solid. In this assignment, I learned how to derive the heat equation, specifically by applying an energy balance to a differential control volume and using Fourier’s law to describe conductive heat transfer. The derivation also incorporated a Taylor series expansion to represent the heat flow entering and leaving the control volume at a position x+dx. Through this process, I gained a deeper understanding of how the heat equation mathematically relates heat flux and temperature. The problem set also emphasized the importance of boundary conditions and initial conditions in determining unknown constants within the governing equation. Common boundary conditions include constant surface temperature, constant heat flux (corresponding to insulated or adiabatic surfaces), and convective boundary conditions. Each of these cases can be represented mathematically, in a way that can be useful in evaluating constants of the governing equation. The heat equation can be used to derive the governing equation for different geometries and thermal conditions. For instance, a one-dimensional system with constant thermal conductivity, steady-state conditions, and no heat generation leads to a linear temperature profile.

This method is especially useful because it provides a more powerful and general approach for analyzing heat transfer than techniques discussed earlier in the course. Previous methods mainly considered simple one-dimensional systems with uniform materials; they could not be used to determine the temperature at arbitrary points within a control volume. In contrast, the heat equation can be applied to more complex, real-world problems involving multidimensional geometries and materials with non-uniform thermal properties. The final problem in the assignment introduced thermal resistance networks, which serve as another practical tool for analyzing heat transfer. By modeling thermal processes with resistances arranged in parallel or series relative to one another, it becomes possible to determine heat flux and unknown temperatures within a system. This approach is analogous to electrical circuits, where temperature difference corresponds to voltage, heat flux corresponds to current, and thermal resistance plays the same role as electrical resistance. Learning this analogy and applying it to an example (i.e., finding the exterior surface temperature of a superalloy blade) demonstrated how thermal resistance networks can simplify the analysis of complicated heat transfer systems. 

<embed 
  src="{{ '/assets/heat-eqn-thermal-resistance.pdf' | relative_url }}" 
  type="application/pdf" 
  width="100%" 
  height="700px" />