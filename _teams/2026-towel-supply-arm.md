---
title: Robot Arm Design for Towel Retrieval in Hotel Supply Rooms
subtitle: 비품실 환경에 최적화된 수건 적재 로봇팔 설계 및 구현
program: URP
year: 2026
participants: [김민정, 박준상]
---

**The problem.** In a robot hotel, mobile robots already carry towels to guest rooms, but nothing loads them. Towels are stacked on shelves in a small, cramped supply room, which is hard for people to work in. A robot arm placed there has to pick one towel at a time from the shelves and put it into the mobile robot's storage bin. Towels are also deformable, which makes them harder to grasp and predict than rigid objects.

**Our question.** Which arm structure fits this room best? We compare seven types (Cartesian, cylindrical, spherical, SCARA, delta, and 6- and 7-axis articulated arms) on reachability, collision-free motion, cycle time, payload, and footprint.

**Approach.**
1. Build a digital twin of the real supply room, the mobile robot, and the towels (real2sim with 3D Gaussian Splatting).
2. Compare the seven arm types with kinematic and workspace analysis in simulation, and choose the best one.
3. Build a first hardware prototype of the chosen arm. Measure grasp success, cycle time, and stacking stability, then use these results to calibrate the simulation.

Winter 2026–27 (Dec. 2026 – Jan. 2027).
