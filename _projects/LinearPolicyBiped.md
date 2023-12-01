---
title: Learning Controllers for Robust Bipedal Locomotion on Challenging Terrains

description: |
  A framework for sythesizing controllers to achieve blind bipedal walking on challenging terrains thorugh learnt linear policies.
people:
  - lokesh
  - utkarsh
  - shishir

layout: project
image: "/img/linearPolicySuff/all_combined.gif"
last-updated: 2021-08-07
status: inactive
---

<br>
#### Abstract
In this work, we demonstrate robust walking in the bipedal robot Digit on uneven terrains by just learning a single linear policy. In particular, we propose a new control pipeline, wherein the high-level trajectory modulator shapes the end-foot ellipsoidal trajectories, and the low-level gait controller regulates the torso and ankle orientation.The foot-trajectory modulator uses a linear policy and the regulator uses a linear PD control law. As opposed to neural network based policies, the proposed linear policy has only 13 learnable parameters, thereby not only guaranteeing sample efficient learning but also enabling simplicity and interpretability of the policy. This is achieved with no loss of performance on challenging terrains like slopes, stairs and outdoor landscapes.We first demonstrate robust walking in the custom simulation environment, MuJoCo, and then directly transfer to hardware with no modification of the control pipeline. We subject the biped to a series of pushes and terrain height changes, both indoors and outdoors, thereby validating the presented work.
<br>
<div style="padding-left:50px" class="row">
<div class="column">
        <figure>  
        <img style="padding:5px" src="{{site.base}}/img/lpb_incline.gif" alt="incline" width="250" height="190"/>
        <figcaption style="text-align:center"> Slope: Incline </figcaption>
        </figure>
 </div>
  
 <div class="column">
        <figure>
        <img style="padding:5px" src="{{site.base}}/img/lpb_decline.gif" alt="decline" width="250" height="190"/>
        <figcaption style="text-align:center"> Slope: Decline </figcaption>
        </figure>
  </div>

  <div class="column">
        <figure>
        <img style="padding:5px" src="{{site.base}}/img/lpb_vslope.gif" alt="vslope" width="250" height="190"/>
        <figcaption style="text-align:center"> Variying Slope </figcaption>
        </figure>
    </div>

   <div class="column">
        <figure>
        <img style="padding:5px" src="{{site.base}}/img/lpb_sine.gif" alt="sine" width="250" height="190"/>
        <figcaption style="text-align:center"> Sinusoidal Terrain </figcaption>
        </figure>
    </div>
    
  <div class="column">
        <figure>
        <img style="padding:5px" src="{{site.base}}/img/lpb_spike.gif" alt="spike" width="250" height="190"/>
        <figcaption style="text-align:center"> Undulated-Spiky Terrain </figcaption>
        </figure>
    </div>
        
  <div class="column">
        <figure>
        <img style="padding:5px" src="{{site.base}}/img/lpb_steps.gif" alt="steps" width="250" height="190"/>
        <figcaption style="text-align:center"> Undulated-Step Terrain </figcaption>
        </figure>
    </div>
    
  <div class="column">
        <figure>
        <img style="padding:5px" src="{{site.base}}/img/lpb_stairs.gif" alt="stairs" width="250" height="190"/>
        <figcaption style="text-align:center"> Staircase </figcaption>
        </figure>
    </div>

  <div class="column">
        <figure>
        <img style="padding:5px" src="{{site.base}}/img/lpb_omnidircect.gif" alt="omni" width="250" height="190"/>
        <figcaption style="text-align:center"> Omni-Driectional Walking </figcaption>
        </figure>
    </div>

  <div class="column">
        <figure>
        <img style="padding:5px" src="{{site.base}}/img//linearPolicySuff/3.gif" alt="omni" width="250" height="190"/>
        <figcaption style="text-align:center"> Unstructured Outdoors </figcaption>
        </figure>
    </div>
        
  <div class="column">
        <figure>
        <img style="padding:5px" src="{{site.base}}/img//linearPolicySuff/4.gif" alt="omni" width="250" height="190"/>
        <figcaption style="text-align:center"> Push Recovery </figcaption>
        </figure>
    </div>
    
  <div class="column">
        <figure>
        <img style="padding:5px" src="{{site.base}}/img//linearPolicySuff/1.gif" alt="omni" width="250" height="190"/>
        <figcaption style="text-align:center"> Hardware - Stairs </figcaption>
        </figure>
    </div>

  <div class="column">
        <figure>
        <img style="padding:5px" src="{{site.base}}/img//linearPolicySuff/2.gif" alt="omni" width="250" height="190"/>
        <figcaption style="text-align:center"> Hardware - Command Control  </figcaption>
        </figure>
    </div>

</div>
<br>
## Control Framework
<div style="text-align:center">
<img src="{{site.base}}/img/con_arch_policy.jpg" alt="drawing" height="300" width="1000"/>
</div>
<br>
## Video
<br>
<p align="center">
<iframe width="500" height="315" src="https://www.youtube.com/embed/4WhgD8u74OY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="500" height="315" src="https://www.youtube.com/embed/jfdafZWFj9I" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>



<br>

<br/>
## Citations ##
```
    @misc{krishna2021learning,
          title={Learning Linear Policies for Robust Bipedal Locomotion on Terrains with Varying Slopes}, 
          author={Lokesh Krishna and Utkarsh A. Mishra and Guillermo A. Castillo and Ayonga Hereid and Shishir Kolathaya},
          year={2021},
          eprint={2104.01662},
          archivePrefix={arXiv},
          primaryClass={cs.RO}
        }
    @misc{krishna2021linear,
          title={Linear Policies are Sufficient to Realize Robust Bipedal Walking on Challenging Terrains}, 
          author={Lokesh Krishna and Guillermo A. Castillo and Utkarsh A. Mishra and Ayonga Hereid and Shishir Kolathaya},
          year={2021},
          eprint={2109.12665},
          archivePrefix={arXiv},
          primaryClass={cs.RO}
        }

```
<br>
<br/>

