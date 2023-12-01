---
title: Off-Policy Average Reward Actor-Critic with Deterministic Policy Search

description: |
  Policy gradient theorem for average reward criteria with deterministic policy. 
people:
  - namansaxena
  - subho
  - shishir
  - shalabh

layout: project
image: "/img/AverageRL/flow_diagram.png"
last-updated: 2023-08-05
status: inactive
---

<br>
#### Abstract
The average reward criterion is relatively less studied as most existing works in the Reinforcement Learning literature consider the discounted reward criterion. There are few recent works that present on-policy average reward actor-critic algorithms, but average reward off-policy actor-critic is relatively less explored. In this work, we present both on-policy and off-policy deterministic policy gradient theorems for the average reward performance criterion. Using these theorems, we also present an Average Reward Off-Policy Deep Deterministic Policy Gradient (ARO-DDPG) Algorithm. We first show asymptotic convergence analysis using the ODE-based method. Subsequently, we provide a finite time analysis of the resulting stochastic approximation scheme with linear function approximator and obtain an $\epsilon$-optimal stationary policy with a sample complexity of $\Omega(\epsilon^{-2.5})$. We compare the average reward performance of our proposed ARO-DDPG algorithm and observe better empirical performance compared to state-of-the-art on-policy average reward actor-critic algorithms over MuJoCo-based environments.

Fore more references, refer to paper at [proceedings.mlr.press/v202/saxena23a/saxena23a.pdf](https://proceedings.mlr.press/v202/saxena23a/saxena23a.pdf) and code at [github.com/namansaxena9/ARO-DDPG](https://github.com/namansaxena9/ARO-DDPG)

<br>

## Block Diagram of the algorithm
<div style="text-align:center">
<img src="{{site.base}}/img/AverageRL/flow_diagram.jpg" alt="drawing"/>
</div>
<br>

## Simulation Results

<p align="center">
  <img width="60%" src="{{site.base}}/img/AverageRL/empresults.png">
</p>
<br>

<br/>

## Citations ##
```
@inproceedings{saxena2023off,
  title={Off-Policy Average Reward Actor-Critic with Deterministic Policy Search},
  author={Saxena, Naman and Khastagir, Subhojyoti and Shishir, NY and Bhatnagar, Shalabh},
  booktitle={International Conference on Machine Learning},
  pages={30130--30203},
  year={2023},
  organization={PMLR}
}
```
<br>
<br/>

