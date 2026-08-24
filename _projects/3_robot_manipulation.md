---
layout: page
title: UR10e manipulation in MuJoCo
description: kinematics, differential kinematics, and control for a 3D interception task
importance: 3
category: coursework
---

Final project for Foundations of Robotics at NYU. I built a MuJoCo-based simulation framework for the UR10e
manipulator that goes from kinematics all the way to task-level control.

The pipeline covers forward and inverse kinematics with DH parameterization, Jacobian-based velocity mapping,
and damped least-squares IK for handling configurations near singularities. On top of that I implemented
three controllers — joint-space PD, velocity control, and operational-space torque control — so that motion
could be commanded at whichever level the task required.

To exercise the whole stack under time pressure, I demonstrated it on a 3D dynamic interception task inspired
by Fruit Ninja: the robot tracks ballistic targets in flight and strikes them mid-trajectory. This forces the
IK and control loop to run fast enough to matter, which a static reaching task does not.

The project is documented through reproducible notebooks, the environment modifications used, and motion
visualizations.
