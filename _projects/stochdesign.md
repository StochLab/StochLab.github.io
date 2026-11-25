---
title: Stoch 1

description: |
  A complete description of the hardware design and control architecture of our custom built quadruped robot, called the Stoch
people:
  - dhaivat
  - shounak
  - ajay
  - abhik
  - shalabh
  - bharadwaj
  - ashitava
  - shishir

layout: project
image: "/img/stoch13.jpg"
last-updated: 2020-10-08
status: inactive
---
### Design & Development of Stoch 1 
In this paper, we present a complete description of
the hardware design and control architecture of our custom
built quadruped robot, called the Stoch. Our goal is to realize a
robust, modular, and a reliable quadrupedal platform, using
which various locomotion behaviors are explored. This
platform enables us to explore different research problems in
legged locomotion, which use both traditional and learning
based techniques. We discuss the merits and limitations of the
platform in terms of exploitation of available behaviours, fast
rapid prototyping, reproduction and repair. Towards the end,
we will demonstrate trotting, bounding behaviors, and
preliminary results in turning. In addition, we will also show
various gait transitions i.e., trot-to-turn and trot-to-bound
behaviors. 
 
 
### Realizing Learned Locomotion Behaviors through Kinematic Motion Primitives
Our main objective in next paper is two fold 1) Obtain an effective tool to realize these basic
motion patterns for quadrupedal walking, called the kinematic
motion primitives (kMPs), via trajectories learned from deep
reinforcement learning (D-RL) and 2) Realize a set of behaviors,
namely trot, walk, gallop and bound from these kinematic
motion primitives in our custom four legged robot, called the
“Stoch”. D-RL is a data driven approach, which has been shown
to be very effective for realizing all kinds of robust locomotion
behaviors, both in simulation and in experiment. On the other
hand, kMPs are known to capture the underlying structure
of walking and yield a set of derived behaviors. We first
generate walking gaits from D-RL, which uses policy gradient
based approaches. We then analyze the resulting walking by
using principal component analysis. We observe that the kMPs
extracted from PCA followed a similar pattern irrespective
of the type of gaits generated. Leveraging on this underlying
structure, we then realize walking in Stoch by a straightforward
reconstruction of joint trajectories from kMPs. This type of
methodology improves the transferability of these gaits to real
hardware, lowers the computational overhead on-board, and
also avoids multiple training iterations by generating a set of
derived behaviors from a single learned gait


<img src="{{site.base}}/img/stoch11.jpg" alt="drawing" width="600"/>

<img src="{{site.base}}/img/stoch12.jpg" alt="drawing" width="600"/>

[![ICCAR](http://i3.ytimg.com/vi/EXb4tONlJe0/hqdefault.jpg)](https://www.youtube.com/watch?v=EXb4tONlJe0&ab_channel=DhaivatDholakiya "ICCAR")
[![ICRA](http://i3.ytimg.com/vi/Wxx9pwwTIL4/hqdefault.jpg)](https://www.youtube.com/watch?v=Wxx9pwwTIL4&t=7s&ab_channel=Stoch_IISc "ICRA")

<br/>
## Citation ##
```
        @inproceedings{dholakiya2019design,
          title={Design, development and experimental realization of a quadrupedal research platform: Stoch},
          author={Dholakiya, Dhaivat and Bhattacharya, Shounak and Gunalan, Ajay and Singla, Abhik and Bhatnagar, Shalabh and Amrutur, Bharadwaj and Ghosal, Ashitava and Kolathaya, Shishir},
          booktitle={2019 5th International Conference on Control, Automation and Robotics (ICCAR)},
          pages={229--234},
          year={2019},
          organization={IEEE}
        }
        
        @inproceedings{singla2019realizing,
          title={Realizing learned quadruped locomotion behaviors through kinematic motion primitives},
          author={Singla, Abhik and Bhattacharya, Shounak and Dholakiya, Dhaivat and Bhatnagar, Shalabh and Ghosal, Ashitava and Amrutur, Bharadwaj and Kolathaya, Shishir},
          booktitle={2019 International Conference on Robotics and Automation (ICRA)},
          pages={7434--7440},
          year={2019},
          organization={IEEE}
        }
```
<br/>
