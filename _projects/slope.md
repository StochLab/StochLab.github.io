---
title: Robust Quadrupedal Locomotion on Sloped Terrains

description: |
  This paper presents a linear policy approach to achieve walking on sloped terrains
people:
  - kartik
  - lokesh
  - aditya
  - sashank
  - naman
  - shalabh
  - bharadwaj 
  - ashitava
  - shishir

layout: project
image: "/img/CORL.gif"
last-updated: 2020-10-15
status: inactive
---

<br>
#### Abstract
In this paper, with a view toward fast deployment of locomotion gaits in low-cost hardware, we use a linear policy for realizing end-foot trajectories in the quadruped robot, Stoch2. In particular, the parameters of the end-foot trajectories are shaped via a linear feedback policy that takes the torso orientation and the terrain slope as inputs.
The corresponding desired joint angles are obtained via an inverse kinematics solver, and tracked via a PID control law.
Augmented Random Search, a model-free and a gradient-free learning algorithm, is used to train this linear policy. Simulation results show that the resulting walking is robust to external pushes and terrain slope variations.
This methodology is not only computationally light-weight, but also uses minimal sensing and actuation capabilities in the robot, thereby justifying the approach.
 

<div style="padding-left:50px" class="row">
<div class="column">
        <figure>  
        <img style="padding:5px" src="{{site.base}}/img/stoch2uphill.gif" alt="uphill" width="250" />
        <figcaption style="text-align:center"> Uphill </figcaption>
        </figure>
 </div>
  
 <div class="column">
        <figure>
        <img style="padding:5px" src="{{site.base}}/img/stoch2sidehill.gif" alt="sidehill" width="250"/>
        <figcaption style="text-align:center"> Sidehill </figcaption>
        </figure>
  </div>
  
   <div class="column">
        <figure>
        <img style="padding:5px" src="{{site.base}}/img/stoch2stair1.gif" alt="staircse" width="250" />
        <figcaption style="text-align:center"> Staircase </figcaption>
        </figure>
    </div>
    
  <div class="column">
        <figure>
        <img style="padding:5px" src="{{site.base}}/img/stoch2dist.gif" alt="disturbance" width="250" height="190"/>
        <figcaption style="text-align:center"> Disturbance Rejection </figcaption>
        </figure>
    </div>
</div>

<div style="text-align:center">
<img src="{{site.base}}/img/control_arch.jpg" alt="drawing" width="700"/>
</div>
<br>
## Video
<br>
<iframe width="560" height="315" src="https://www.youtube.com/embed/KdQn1e3rI7o" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br>

<br/>
## Citation ##
```
        @misc{paigwar2020robust,
              title={Robust Quadrupedal Locomotion on Sloped Terrains: A Linear Policy Approach}, 
              author={Kartik Paigwar and Lokesh Krishna and Sashank Tirumala and Naman Khetan and Aditya Sagi and Ashish Joglekar and Shalabh Bhatnagar and Ashitava Ghosal and Bharadwaj Amrutur and Shishir Kolathaya},
              year={2020},
              eprint={2010.16342},
              archivePrefix={arXiv},
              primaryClass={cs.RO}
        }
```
<br>
<br/>

