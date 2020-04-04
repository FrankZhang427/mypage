---
title: "Mini Games in Unity"
description: "Four mini games developed in Unity for modern computer games course"
code: ""
tags: ["Computer Games", "Unity", "c#"]
weight: 0
report: false
draft: false
---

## Introduction

I have implemented four interesting mini games for my modern computer game course. All four games were developed in [Unity](https://unity.com/) and require a version of [2018.2.8](https://unity3d.com/get-unity/download/archive) at least to run properly. 

### [Maze Shooter](#maze-shooter)

This is a first-person shooter game in 3D. Players can move with ```WASD``` control, jump with ```space```, and fire projectiles with ```F``` key. The view camera is controlled by mouse input. The terrain consists of 3 parts: a starting area, a destination area, and a dynamically generated maze connecting the two areas. Maze generation is implemented based on [Eller's algorithm](http://weblog.jamisbuck.org/2010/12/29/maze-generation-eller-s-algorithm). More detailed game design can be found [here](/pdf/maze_shooter.pdf). [[code](https://github.com/FrankZhang427/maze-shooter)]