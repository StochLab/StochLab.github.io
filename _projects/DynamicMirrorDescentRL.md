---
title: Dynamic Mirror Descent MPC for Model-based Model-free Reinforcement Learning

description: |
  A framework for utilizing experience for generating predictive simulations and learning from them.
people:
  - utkarsh
  - soumya
  - prakharg
  - shishir


layout: project
image: "/img/DeMoRL/all_combined.gif"
last-updated: 2022-01-31
status: inactive
---

<br>
#### Abstract
Recent works in Reinforcement Learning (RL) combine model-free (Mf)-RL algorithms with model-based (Mb)-RL approaches to get the best from both: asymptotic performance of Mf-RL and high sample-efficiency of Mb-RL. Inspired by these works, we propose a hierarchical framework that integrates online learning for the Mb-trajectory optimization with off-policy methods for the Mf-RL. In particular, two loops are proposed, where the Dynamic Mirror Descent based Model Predictive Control (DMD-MPC) is used as the inner loop Mb-RL to obtain an optimal sequence of actions. These actions are in turn used to significantly accelerate the outer loop Mf-RL. We show that our formulation is generic for a broad class of MPC-based policies and objectives, and includes some of the well-known Mb-Mf approaches. We finally introduce a new algorithm: Mirror-Descent Model Predictive RL (M-DeMoRL), which uses Cross-Entropy Method (CEM) with elite fractions for the inner loop. Our experiments show faster convergence of the proposed hierarchical approach on benchmark MuJoCo tasks. We also demonstrate hardware training for trajectory tracking in a 2R leg and hardware transfer for robust walking in a quadruped. We show that the inner-loop Mb-RL significantly decreases the number of training iterations required in the real system, thereby validating the proposed approach.

Fore more references, refer to paper at [arxiv.org/pdf/2112.02999.pdf](https://arxiv.org/pdf/2112.02999.pdf) and code at [github.com/UtkarshMishra04/DMD-MPC-RL](https://github.com/UtkarshMishra04/DMD-MPC-RL)

<br>
## Control Framework
<div style="text-align:center">
<img src="{{site.base}}/img/DeMoRL/methodology.jpg" alt="drawing"/>
</div>
<br>

## Simulation Results

<p align="center">
  <img width="60%" src="{{site.base}}/img/DeMoRL/simresults.gif">
</p>
<br>

## Hardware Results

<p align="center">
  <img width="70%" src="{{site.base}}/img/DeMoRL/legresults.jpg">
</p>

<p align="center">
  <img width="45%" src="{{site.base}}/img/DeMoRL/hardresults.gif"> 
  <img width="45%" src="{{site.base}}/img/DeMoRL/stochresults.gif">
</p>

<br>

## Video
<br>
<p align="center">
<iframe width="500" height="315" src="https://www.youtube.com/embed/Bj9dN1KNPAs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

<br>

<br/>
## Citations ##
```
    @article{mishra2021dynamic,
    title={Dynamic Mirror Descent based Model Predictive Control for Accelerating Robot Learning},
    author={Mishra, Utkarsh A, Samineni, Soumya R, Goel, Prakhar, Kunjeti, Himanshu, Lodha, Aman, Singh, Aditya, Sagi, Shalabh, Bhatnagar, and Kolathaya, Shishir},
    journal={arXiv preprint arXiv:2106.15273},
    year={2021}
}
```
<br>
<br/>

