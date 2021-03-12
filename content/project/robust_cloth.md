---
title: "Robust Cloth Simulation with Constraints and Collision Detection"
description: "Project for computer animation course"
code: "RobustCloth"
tags: ["Animation", "physically-based simulation", "java", "OpenGL"]
weight: 4
report: true
draft: false
---

## Abstract

The goal of this project is to extend the idea of particle-spring system, constraints and collision detection into 3D by implementing a cloth simulator in 3D. The first step is to extend the existed functionalities from previous 2D version into 3D. The position and velocity of each particle at each time step are updated by Backward Euler integrator. Using an explicit integrator generally produces an unstable simulation for large time steps. Since the system in cloth simulation usually contains hundreds of particles, it is also impractical to use small time step in real time simulation. Collision and cloth self-penetration can happen during cloth simulation. Therefore, robust collision detection and response is implemented to resolve cloth collision with objects. The cloth simulator can also handle constraints in the system, such as fixed points and impenetrable areas.


## Demo Video

A cloth of size 20x20 is simulated in real time. In the first simulation, the cloth has a constraint that top left and right corners are fixed. In the second simulation, such constraint is removed. In both simulations, yellow icosahedron sphere mesh represents a random object to collide with cloth, and the blue sphere is an impenetrable constraint.

{{< youtube -NANlFgXHUI >}}