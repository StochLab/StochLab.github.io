---
title: Dynamic Manipulator

description: |
  A highly dynamic, torque controllable manipulator for quadruped robots.
people:
  - prakharg
  - amritanshu
  - vedvyas
  - shishir

layout: project
image: "/img/manipulator/manipulator.png"
last-updated: 2023-11-30
---

<br>

## Introduction

A highly dynamic torque controllable manipulator, developed for quadruped robots. The overall system is an articulated robotic arm designed to meet the mandatory requirements of having four degrees of freedom, a length of approximately 1000mm, a payload capacity of 500g to 1 kilogram, support for both position and torque control, custom planetary gearboxes with high reduction ratios (>8:1) and low backlash, support for control in both joint and cartesian space, based on the ROS2 software stack, with a total weight of <=6.5 kilograms, finished with 6061 Aluminium or Carbon Fibre, and equipped with Aruco tag detection and obstacle avoidance capabilities, as well as appropriate spray volume for pesticide spraying applications. The system also incorporates desirable requirements, such as a cost of less than INR 3 Lakhs, consideration of product design constraints and aesthetic finish, suitability for various ground mobile robots, utilization of hollow links for wiring and additional routing, manufacturing of electronics and mechanical components in India, use of hybrid manufacturing systems for fast iteration, modular design for easy scaling and integration of multiple end effectors, software control of spraying equipment pressure for adaptive applications, and an electronics interface panel for easy integration with existing robotic systems

Fore more references, refer to paper at [bachelor thesis](https://drive.google.com/file/d/1mahLrWoYIt20TMIxsCvkgQzFZwlG1I-C/view?usp=drive_link)
<br>

## Specifications (version1)

- Degrees of Freedom: 4
- Length at full extension ~1.2m
- Weight: 7.5kgs, with Al finish
- Payload at full extension: 800gms-1kg
- Control: Position and Torque(Force control). FOC at 40Khz
- Workspace: Articulated constrained spherical (x,y,z,pitch)
- ROS2 enabled software stack powered by ROS2 control driver and Moveit2 planners
- End effector: 1 DOF (Pitch), with realsense depth camera and precision spray nozzle
  <br>
<p align="center">
  <img width="70%" src="{{site.base}}/img/manipulator/specs.png">
</p>
<br>

## CyberPhysical Architecture

<p align="center">
  <img width="90%" src="{{site.base}}/img/manipulator/cpa.png">
</p>
<br>

## Actuator Development Lifecycle

<p align="center">
  <img width="90%" src="{{site.base}}/img/manipulator/adlc.png">
</p>
<br>

### Actuator Specifications
* Reducer Technology: Planetary
* Gear Reduction: 8:1
* Weight: 900gms
* Torque(Rated): 32NM (12s)
* Backlash: Minimal
* Back drivaibility: Yes
* Bearing: Deep groove Ball Bearings
<br>

## Video

<br>
<p align="center">
<iframe width="500" height="315" src="https://www.youtube.com/watch?v=IA0kupzC7p8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

<br>

<br/>

## Queries

Contact : Prakhar Goel

Email: prakhs00@gmail.com

<!-- ## Citations ##
```
    @article{mishra2021dynamic,
    title={Dynamic Mirror Descent based Model Predictive Control for Accelerating Robot Learning},
    author={Mishra, Utkarsh A, Samineni, Soumya R, Goel, Prakhar, Kunjeti, Himanshu, Lodha, Aman, Singh, Aditya, Sagi, Shalabh, Bhatnagar, and Kolathaya, Shishir},
    journal={arXiv preprint arXiv:2106.15273},
    year={2021}
}
``` -->
<br>
<br/>
