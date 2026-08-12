---
title: Collision Cone Control Barrier Functions (C3BF)

description: |
  Control Barrier Functions for Kinematic Obstacle Avoidance :A Collision Cone Approach
  
people:
  - manan
  - bhavya
  - phani
  - pushpak
  - shishir

layout: project
image: "/img/C3BF/c3bf.gif"
last-updated: 2024-03-28
status: inactive
category: safety

---
## Introduction 
This work presents a unified approach for collision avoidance using Collision-Cone Control Barrier Functions (CBFs) in both ground (UGV) and aerial (UAV) unmanned vehicles. We propose a novel CBF formulation inspired by collision cones, commonly used in trajectory planning, to ensure safety by constraining the relative velocity between the vehicle and the obstacle to always point away from each other. The efficacy of this approach is demonstrated through simulations and hardware implementations on the Turtlebot, Stoch-Jeep (Ackermann), and Crazyflie 2.1 quadrotor robot, showcasing its effectiveness in avoiding collisions with dynamic obstacles in both ground and aerial settings. The real-time controller is developed using CBF Quadratic Programs (QPs) formulation. Comparative analysis with existing CBF-QPs, particularly Higher-Order CBF (HOCBF), highlights the less conservative nature of the proposed approach. Overall, this research contributes to a novel control formation that can give a guarantee for collision avoidance in unmanned vehicles by modifying the control inputs from existing path-planning controllers, enhancing the vehicle's maneuverability and safety in dynamic environments.

## Simulation Results
### Obstacle avoidance on UGVs (Unicycle & Bicycle Models)
<iframe width="560" height="315" src="https://www.youtube.com/embed/Dme7Wm9y6es?si=MJtqDGpFVl71ZDMD" 
      title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

### Obstacle avoidance on UAV (Quadrotor Model)
<iframe width="560" height="315" src="https://www.youtube.com/embed/oTauuHCpFM0?si=xlMvqoxhGrRpvOgm" 
      title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Hardware Experiments
### Obstacle avoidance on Turlebot (Unicycle Model)
<iframe width="560" height="315" src="https://www.youtube.com/embed/L7y6x_121T8?si=2Vf_1IINKDDmOGqv" 
      title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

### Obstacle avoidance on Stoch-Jeep (Bicycle Model)
<iframe width="560" height="315" src="https://www.youtube.com/embed/bYME1ZF98TQ?si=5I-RhM3igN1eQD9-" 
      title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

### Obstacle avoidance on Crazyflie 2.1 (Quadrotor Model)</h3>
<iframe width="560" height="315" src="https://www.youtube.com/embed/_OIX3QhtQUM?si=4oo1aWrbs3rv9hFT" 
      title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<br/>
## Citation ##
```
        @article{tayal2024collisionconeapproachcontrol,
              title={A Collision Cone Approach for Control Barrier Functions}, 
              author={Manan Tayal and Bhavya Giri Goswami and Karthik Rajgopal and Rajpal Singh and Tejas Rao and Jishnu Keshavan and Pushpak Jagtap and Shishir Kolathaya},
              year={2024},
              eprint={2403.07043},
              archivePrefix={arXiv},
              primaryClass={cs.RO},
              url={https://arxiv.org/abs/2403.07043}, 
        }
        
        @article{thontepu2022control,
          title={Control Barrier Functions in UGVs for Kinematic Obstacle Avoidance: A Collision Cone Approach},
          author={Thontepu, Phani and Goswami, Bhavya Giri and Singh, Neelaksh and PI, Shyamsundar and Sundaram, Suresh and Katewa, Vaibhav and others},
          journal={arXiv preprint arXiv:2209.11524},
          year={2022}
        }
        
        @article{tayal2023control,
          title={Control Barrier Functions in Dynamic UAVs for Kinematic Obstacle Avoidance: A Collision Cone Approach},
          author={Tayal, Manan and Kolathaya, Shishir},
          journal={arXiv preprint arXiv:2303.15871},
          year={2023}
        }
        @misc{goswami2023collision,
              title={Collision Cone Control Barrier Functions: Experimental Validation on UGVs for Kinematic Obstacle Avoidance}, 
              author={Bhavya Giri Goswami and Manan Tayal and Karthik Rajgopal and Pushpak Jagtap and Shishir Kolathaya},
              year={2023},
              eprint={2310.10839},
              archivePrefix={arXiv},
              primaryClass={cs.RO}
        }
        
```
<br/>
