---
title: Augmented Random Search (RL Algorithm)

description: |
  Reinforcement Learning using ARS (Augmented random Search)to generate Gaits
  
people:
  - shashank
  - aditya
  - kartik
  - ashish
  - shalabh
  - bharadwaj 
  - ashitava
  - shishir

layout: project
image: "/img/3-Figure3-1.png"
last-updated: 2020-10-08
status: inactive
---
### Learning Stable Manoeuvres in Quadruped Robots from Expert Demonstrations 
With the research into development of quadruped
robots picking up pace, learning based techniques are being
explored for developing locomotion controllers for such robots.
A key problem is to generate leg trajectories for continuously
varying target linear and angular velocities, in a stable manner.
In this paper, we propose a two pronged approach to address
this problem. First, multiple simpler policies are trained to
generate trajectories for a discrete set of target velocities and
turning radius. These policies are then augmented using a
higher level neural network for handling the transition between
the learned trajectories. Specifically, we develop a neural
network based filter that takes in target velocity, radius and
transforms them into new commands that enable smooth transitions to the new trajectory. This transformation is achieved by
learning from expert demonstrations. An application of this is
the transformation of a novice user’s input into an expert user’s
input, thereby ensuring stable manoeuvres regardless of the
user’s experience. Training our proposed architecture requires
much less expert demonstrations compared to standard neural
network architectures. Finally, we demonstrate experimentally
these results in the in-house quadruped Stoch 2.



### Gait Library Synthesis for Quadruped Robots via Augmented Random Search ###
In this paper, with a view toward fast deployment
of learned locomotion gaits in low-cost hardware, we generate a
library of walking trajectories, namely, forward trot, backward
trot, side-step, and turn in our custom built quadruped robot,
Stoch 2, using reinforcement learning. There are existing
approaches that determine optimal policies for each time step,
whereas we determine an optimal policy, in the form of endfoot trajectories, for each half walking step i.e., swing phase
and stance phase. The way-points for the foot trajectories are
obtained from a linear policy, i.e., a linear function of the
states of the robot, and cubic splines are used to interpolate
between these points. Augmented Random Search, a modelfree and gradient-free learning algorithm, is used to learn the
policy in simulation. This learned policy is then deployed on
hardware, yielding a trajectory in every half walking step.
Different locomotion patterns are learned in simulation by
enforcing a preconfigured phase shift between the trajectories of
different legs. Transition from one gait to another is achieved
by using a low-pass filter for the phase, and the sim-to-real
transfer is improved by a linear transformation of the states
obtained through regression

<br/>
<img src="{{site.base}}/img/tile_backtrot.png" alt="drawing" width="600"/>
<img src="{{site.base}}/img/tile_sidestep.png" alt="drawing" width="600"/>
<img src="{{site.base}}/img/tile_turn.png" alt="drawing" width="600"/>

[![Gait Library Synthesis](http://i3.ytimg.com/vi/3BQYX2vZdAg/hqdefault.jpg)](https://www.youtube.com/watch?v=3BQYX2vZdAg&t=97s&ab_channel=Stoch_IISc "GaitLibrary")
[![Learning Stable Manuveuers](http://i3.ytimg.com/vi/LRbHetp0dcg/hqdefault.jpg)](https://www.youtube.com/watch?v=LRbHetp0dcg&t=15s&ab_channel=kartikpaigwar "ROMAN")

<br/>
## Citation ##
```
        @article{tirumala2019gait,
          title={Gait Library Synthesis for Quadruped Robots via Augmented Random Search},
          author={Tirumala, Sashank and Sagi, Aditya and Paigwar, Kartik and Joglekar, Ashish and Bhatnagar, Shalabh and Ghosal, Ashitava and Amrutur, Bharadwaj and Kolathaya, Shishir},
          journal={arXiv preprint arXiv:1912.12907},
          year={2019}
        }
        
        @article{tirumala2020learning,
          title={Learning Stable Manoeuvres in Quadruped Robots from Expert Demonstrations},
          author={Tirumala, Sashank and Gubbi, Sagar and Paigwar, Kartik and Sagi, Aditya and Joglekar, Ashish and Bhatnagar, Shalabh and Ghosal, Ashitava and Amrutur, Bharadwaj and Kolathaya, Shishir},
          journal={arXiv preprint arXiv:2007.14290},
          year={2020}
        }
        
```
<br/>