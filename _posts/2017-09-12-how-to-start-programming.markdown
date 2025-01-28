---
layout: post
title: Oscilloscope Front-End Circuit Design
date: 2023-04-27 12:00:00
description: Front-end design of an externally powered oscilloscope with 1x and 10x input modes, frequency attenuation, and AC/DC coupling.
img: osc_pcb.png # Add image post (optional)
fig-caption: Oscilloscope Front-End Circuit Design
tags: [Oscilloscope, Circuit Design, PCB, Analog Filters]
---

This project involved designing the front-end circuit and PCB layout for an externally powered oscilloscope, incorporating two input ranges (1x and 10x modes), frequency attenuation above 20 kHz, and both AC and DC coupling capabilities.
![Oscilloscope Circuit]({{site.baseurl}}/assets/img/osc_diagram.png)

## Circuit Design
- The circuit uses **low-pass filters**, **adders**, **buffers**, and **SPST switches** to implement the functionality of the oscilloscope front-end.
- **LTspice** simulations were conducted to validate the design before creating the PCB layout.
- The low-pass filter was specifically designed using the **Analog Filter Wizard** to attenuate content frequencies above 20 kHz.
![Oscilloscope Circuit]({{site.baseurl}}/assets/img/osc_path.png)

![Oscilloscope Circuit]({{site.baseurl}}/assets/img/osc_ltspice.png)


## PCB Layout
- The PCB was designed using **Autodesk Eagle**, employing **surface-mount technology (SMT)** to achieve a compact and efficient design.
- The design accommodates **both 1x and 10x input modes** and integrates **AC/DC coupling switches**.
![Oscilloscope Circuit]({{site.baseurl}}/assets/img/osc_pcb.png)

## Simulation Results
- The circuit was successfully simulated on **LTspice**, with accurate switching between the two input modes and correct AC/DC coupling behavior.
- The design met the requirements for frequency attenuation and switching functionality.

## Final Outcome
- The design received a grade of **97%** for the assignment, demonstrating successful completion of the project.
- The design ensures reliable oscilloscope performance and meets the specification requirements for input range switching and frequency attenuation.


This project showcases expertise in:
- Analog circuit design.
- PCB layout using SMT.
- Simulation and verification using LTspice.

