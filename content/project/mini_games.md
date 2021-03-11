---
title: "Mini Games in Unity"
description: "Four mini games developed in Unity for modern computer games course"
code: ""
tags: ["Computer Games", "Unity", "c#"]
weight: 4
report: false
draft: false
---

## Introduction

I have implemented four interesting mini games for my modern computer game course. All four games were developed in [Unity](https://unity.com/) and require a version of [2018.2.8](https://unity3d.com/get-unity/download/archive) at least to run properly. 

### [Maze Shooter](#maze-shooter)

This is a first-person shooter game in 3D. Players can move with ```WASD``` control, jump with ```space```, and fire projectiles with ```F``` key. The view camera is controlled by mouse input. The terrain consists of 3 parts: a starting area, a destination area, and a dynamically generated maze connecting the two areas. Maze generation is implemented based on [Eller's algorithm](http://weblog.jamisbuck.org/2010/12/29/maze-generation-eller-s-algorithm). More detailed game design can be found [here](/pdf/maze_shooter.pdf). [[code](https://github.com/FrankZhang427/maze-shooter)]

### [Turkey Cannon](#turkey-cannon)

This is a 2D cannon shooting game where the player controls a cannon to shoot turkeys over a mountain. The scene consists of a randomized (with midpoint-bisection) mountian in the middle, a cannon on the right, and some turkeys on the left. Several factors affect the cannonball trajectory including gravity, wind (the direction and magnitude of which are indicated by a cloud on the top) and collisions with scene objects. Turkeys are modelled by [Verlet integration](https://en.wikipedia.org/wiki/Verlet_integration). Turkeys slowly pace back and forth, and sometimes leap upward. More detailed game design can be found [here](/pdf/turkey_cannon.pdf). [[code](https://github.com/FrankZhang427/turkey-cannon)]

### [Pac-Man AI](#pac-man-AI)

This is a 2D Pac-Man game where two agents compete with each other. One of the agents is controlled by the player (```WASD``` to move and ```space``` to teleport trap), and the other one is controlled by game AI. Simple enemies patrol the corridor area to catch both agents. Each agent has two teleport traps, when used, the closest enemy or agent is selected, and immediately moved to a random room (agent), or de-and-re-spawned (enemy). The AI agent is controlled through a [hierarchical task network (HTN)](https://en.wikipedia.org/wiki/Hierarchical_task_network). The HTN design of AI agent is documented [here](/pdf/HTN.pdf). More detailed game design can be found [here](/pdf/pac-man_AI.pdf). [[code](https://github.com/FrankZhang427/pac-man-AI)]


### [Social Behavior Simulator](#social-behavior)

This is an Unity simulator that simulates the flow of travellers with presence of wanderers, social agents and obstacles. The scene consists of a large rectangle area and several obstacles (dynamically generated). A travelling agent spawns at the right side of rectangle area and tries to reach one of the doorway on the left side. Wanderer agents simply wander around the level with varying but relatively fast speed. Wanderers try to interfere the travelling agents from reaching their goals. Social agents move randomly around the level. When they are close to other social agents or a group of social agents, they randomly decide whether or not to start a conversation with other social agents or join the social group. This simulator tries to measure the throughput of travelling agents with interference from wanderers, social agents, and obstacles. The instruction of setting simulation parameters and test results can be found [here](/pdf/setup_result.pdf). More detailed simulator design can be found [here](/pdf/social_behavior.pdf). [[code](https://github.com/FrankZhang427/social-behavior)]