---
title: Stoch BiRo

description: |
  Design and Control of a low cost bipedal robot
  
people:
  - manan
  - mothish
  - karthikraj
  - ravikola
 

layout: project
image: "/img/StochBiRo.png"
last-updated: 2023-12-01
---
### Abstract 
This paper introduces the Stoch BiRo, a cost-effective bipedal robot designed with a modular mechanical structure having point feet to navigate uneven and unfamiliar terrains. The robot employs proprioceptive actuation in abduction, hips, and knees, leveraging a Raspberry Pi4 for control. Overcoming computational limitations, a Learning-based Linear Policy controller manages balance and locomotion with only 3 degrees of freedom (DoF) per leg, distinct from the typical 5DoF in bipedal systems. Integrated within a modular control architecture, these controllers enable autonomous handling of unforeseen terrain disturbances without external sensors or prior environment knowledge. Demonstrating efficiency through low Cost of Transport (CoT) across varying walking speeds and blind stair climbing, the robot's policies are trained and simulated using MuJoCo, transferring learned behaviors to the Stoch BiRo hardware for initial walking validations. This work highlights the Stoch BiRo's adaptability and cost-effectiveness in mechanical design, control strategies, and autonomous navigation, promising diverse applications in real-world robotics scenarios.

### Design and Development of Stoch BiRo
We present a complete description of the hardware design and control architecture of our custom built quadruped robot, called the Stoch. Our goal is to realize a robust, modular, and a reliable quadrupedal platform, using which various locomotion behaviors are explored. This platform enables us to explore different research problems in legged locomotion, which use both traditional and learning based techniques. We discuss the merits and limitations of the platform in terms of exploitation of available behaviours, fast rapid prototyping, reproduction and repair.

### Control Framework 
We use a hierarchical structure, that decouples the linear and nonlinear parts of the control framework. The linear part is the foot trajectory modulator, and the nonlinear part is the tracking controller. Based on the orientation of torso and supporting plane, the modulator transforms the semi-ellipses in real-time. The tracking controller then tracks the generated semi-ellipses independently for each leg with a constant phase difference.
Joint-level PD controllers are used to track the required joint targets obtained through inverse kinematics. Note that our controller does not include contact modelling and explicit switching conditions, as a model-free learning algorithm
is used.
