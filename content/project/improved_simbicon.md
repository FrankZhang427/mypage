---
title: "Improving SIMBICON for Biped Animation"
description: "Master's project based on SIMBICON controller"
code: "Improved_Simbicon"
tags: ["Computer Graphics and Animation", "physically-based simulation", "java"]
weight: 1
draft: false
---

Biped balance control strategy is difficult to design as biped locomotion suffers from high-dimensional action spaces, underactuated dynamics, and unstable joint controls. We propose a generalized balance control strategy that can synthesize robust biped walking locomotion. The generalization consists of two parts, a coordinated joint control and generalized ground height feedback. We also conduct principle component analysis on generated locomotion to further improve the state used in finite state machine. Systems employing proportional-derivative controllers face the trade-off between simulation efficiency and effectiveness. We explore and exploit a stable variant of proportional-derivative controller to enhance the simulation process. Our main contributions are improving the robustness of biped control against upward steps in real time, and generating more torque-efficient and smoother simulations.