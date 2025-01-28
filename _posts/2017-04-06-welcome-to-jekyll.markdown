---
layout: post
title: GaitKeep - Biomedical Engineering Competition - 3rd Place
date: 2022-03-15 12:00:00
description: Developed a prototype using Rhythmic Auditory Simulation to decrease gait variability in Parkinson's dementia patients.
img: gaitkeep_app.png # Add image post (optional)
fig-caption: GaitKeep Prototype for Parkinson's Dementia Patients
tags: [Biomedical Engineering, Parkinson's, Prototype, MATLAB, Python]
---

This project focused on decreasing gait variability in Parkinson's dementia patients through **Rhythmic Auditory Simulation** (RAS), a method shown to improve cadence in medical research.
![GaitKeep Prototype]({{site.baseurl}}/assets/img/gaitkeep_app.png)

## Prototype Design
- **GaitKeep** is a wearable necklace with a built-in speaker that plays calibrated rhythmic audio based on the user's walking cadence.
- A mobile app was developed to **calibrate** the necklace by identifying the user's natural walking cadence through a short **100-step walking test**.
![GaitKeep Prototype]({{site.baseurl}}/assets/img/gaitkeep_diag.png)

## Data Collection & Algorithm
- **MATLAB** was used to collect accelerometer data from the user's phone to determine their optimal walking cadence.
- A **Python BPM algorithm** and **discrete wavelength transform** were applied to match **music** with the user’s walking cadence, delivering the auditory stimulus needed to stabilize gait.
![GaitKeep Prototype]({{site.baseurl}}/assets/img/gaitkeep_graph.png)
## Competition Results
- The project was well-received at the **University of Toronto CUBE Biomedical Engineering Competition**, where it earned **3rd place**.

## Key Features
- Integration of **wearable technology** with real-time feedback.
- Use of **MATLAB** for cadence analysis and **Python** for audio synchronization.
- **Mobile app** that personalizes cadence and plays music tailored to individual users.

![GaitKeep Prototype]({{site.baseurl}}/assets/img/gaitkeep-prototype.png)

This project highlights:
- Application of **Rhythmic Auditory Simulation** in medical devices.
- Prototyping wearable technology.
- Algorithm development for cadence tracking and music synchronization.

