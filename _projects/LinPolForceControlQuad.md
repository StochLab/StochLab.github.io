---
title: 'Force control for Robust Quadruped Locomotion: A Linear Policy Approach'

description: |
  A framework for designing controllers to achieve robust blind quadrupedal walking using force control thorugh learnt linear policies.
people:
  - ashirwat
  - vamshi
  - devarajuvinoda
  - shishir

layout: project
image: "/img/LinPolForceControl/stoch3_combined.GIF"
last-updated: 2023-01-28
status: inactive

---

<br>
#### Abstract

This work presents a simple linear policy for direct force control for quadrupedal robot locomotion. The motivation is  that  force  control  is  essential  for  highly  dynamic  and  agile motions. Unlike  the  majority  of  the  existing  works  that  use complex nonlinear function approximators to represent the RL policy  or  model  predictive  control  (MPC)  methods  with  many optimization  variables  in  the  order  of  hundred,  our  controller uses a simple linear function approximator to represent policy. We   demonstrate   this   compute-efficient controller  on  our  robot  Stoch3  in  simulation  and  real-world experiments on indoor and outdoor terrains with push recovery.

*Full paper will be uploaded soon*

<br>


## Simulation Results

<p align="center">
  <img width="60%" src="{{site.base}}/img/LinPolForceControl/stoch3_1.GIF">
</p>
<br>

## Hardware Results

<p align="center">
  <img width="70%" src="{{site.base}}/img/LinPolForceControl/stoch3_2.GIF">
</p>

<p align="center">
  <img width="45%" src="{{site.base}}/img/LinPolForceControl/stoch3_3.GIF"> 
  <img width="45%" src="{{site.base}}/img/LinPolForceControl/stoch3_4.GIF">
</p>

<br>

## Video
<br>
<p align="center">
<iframe width="560" height="315" src="https://www.youtube.com/embed/k89QdImcqdo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

<br>

<br/>
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
