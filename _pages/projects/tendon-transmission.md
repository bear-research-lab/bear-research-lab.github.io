---
layout: page
title: " "
permalink: /projects/tendon-transmission/
---
### 1. Why are we interested in under-actuated tendon transmission?
Many robots, especially hands and wearable robots, have far more joints than they can afford motors. Adding an actuator for every joint makes a system **heavy**, **bulky**, and **hard to control**.

Under-actuated tendon transmission offers a different path: a small number of actuators pull tendons routed through the structure, and the **routing itself** determines how the joints move and how forces are distributed. Complexity moves from the motors and controllers into the **mechanical design**, so that a simple system can still produce rich, useful motions.

---

### 2. What are we working on?
We study tendon transmission as a **general design method**, not as part of a single robot:
- **Tendon routing analysis and design** – how the path, constraints, and coupling of tendons shape joint motion, motion sequence, and force distribution.
- **Compact actuation** – actuators and transmissions that drive multiple tendons from few motors.
- **Sensing through tendons** – estimating joint angles and contact forces from tendon tension, stroke, and embedded sensors.

Representative work:
- **Constrained tendon routing** for a soft hand-wearable robot (Exo-Glove Pinch). *IEEE RA-L, 2025.* [Paper](https://bear-research-lab.github.io/assets/pub/RAL_CTR.pdf), [Project](https://sites.google.com/view/constrained-tendon-routings)
- **Dual-Tendon Routing** for under-actuated, tendon-driven soft hand-wearable robots. *IEEE RA-L, 2025.* [Paper](https://bear-research-lab.github.io/assets/pub/RAL_DTR.pdf), [Project](https://sites.google.com/view/dt-routing/overview), [Video](https://www.youtube.com/watch?v=3sa5VhzjjoU)
- **Modulating thumb and finger motion sequence with a single actuator** (Exo-Glove Poly III). *Soft Robotics, 2025.* [Paper](https://bear-research-lab.github.io/assets/pub/SORO_EP3.pdf), [Video](https://www.youtube.com/watch?v=XG7Zscma3a4)
- **Slider-Tendon Linear Actuator** with under-actuation and fast connection. *IEEE/ASME T-MECH, 2021.* [Paper](https://bear-research-lab.github.io/assets/pub/TMECH_STLA.pdf), [Video](https://youtu.be/BQsyxZ3xNZc)
- **Under-actuated robotic gripper with fiber-optic force sensing tendons.** *IEEE RA-L, 2024.* [Paper](https://bear-research-lab.github.io/assets/pub/RAL_FBG.pdf), [Video](https://www.youtube.com/watch?v=m80z5AHBeTk)

These methods are the foundation of our [robotic hands](/projects/robotic-hands/) projects, and we plan to combine them with [computational robot co-design](/projects/codesign/) so that tendon routings can be designed automatically for a given task.

---
This page was written with the help of a large language model (LLM).
