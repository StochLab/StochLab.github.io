---
title: 'Co-design Optimization and Actuator Optimization for Legged Robots'

description: |
  
people:
  - amansingh
  - amishra
  - shishir

layout: project
image: "/img/Codesign/main.png"

last-updated: 2025-02-28

---
<br>
<br>

### Introduction

Legged robots—such as quadrupeds and humanoids—require actuators that are not only high in torque and efficiency but also lightweight and responsive. Multiple actuator architectures exist for meeting joint-level performance requirements, including single-stage, two-stage, and compound planetary gearboxes, cycloidal drives, and strain-wave gearboxes. However, most actuator designs in the field today rely heavily on heuristics or designer intuition, with limited use of rigorous optimization-based design techniques. While some studies have employed optimization methods for actuator design, they often fail to account for key real-world parameters like mass and efficiency. Even when such factors are considered, the underlying models tend to be overly simplistic, limiting their applicability in practical robotic systems.

Recent approaches in robot design use co-design optimization, where mechanical design and control strategies are optimized simultaneously. Although these methods optimize parameters such as link lengths, gear ratios, compliance, and actuator scaling, they often overlook the critical choice of gearbox architecture itself. Moreover, their actuator models lack detailed representation of mass and efficiency, which are essential for realistic, high-performance designs.

Our research aims to bridge this gap by addressing two core questions:
- Can we formulate an optimization framework that, given a joint-level performance requirement, not only determines optimal design parameters but also selects the most suitable gearbox type?
- Can we incorporate accurate, real-world models of actuator mass and efficiency into this optimization to produce designs that are directly manufacturable and performance-aligned?

#### Applications

This research has two primary applications:
- Component-Level Optimization: Given joint performance requirements, our framework enables the selection of the most appropriate gearbox type and its corresponding optimal parameters—streamlining actuator selection and design.
- System-Level Co-Design: The insights and models developed through this work can be directly integrated into larger co-design frameworks for legged robots. This allows for more accurate optimization of the entire system.

<br>
<br>

### Methodology

<br>

<!-- html image -->
<div style="text-align: center;">
  <img src="/img/Codesign/codesign_1.png" alt="drawing" width="100%"/>
</div>

The optimization framework (left) optimizes gearbox parameters for a given motor and performance requirements, passing them to the design automation block. This generates a parametric template model, which a human designer uses to create the manufacturable CAD of the actuator.

#### Current Work Status

Currently, we have developed a comprehensive optimization framework for two widely used single-stage planetary gearbox architectures: the Internal Single-Stage Planetary Gearbox (ISSPG) and the External Single-Stage Planetary Gearbox (ESSPG). Given a specific motor and joint performance requirements, this framework computes the optimal design parameters for both gearbox architectures. In addition, we have developed an automated actuator design framework that utilizes these optimized parameters to generate a template CAD model. This CAD generation process is fully automated and provides a baseline design that captures the essential mechanical features needed for manufacturability. Using the generated template, designers can efficiently finalize and detail the actuator for fabrication.

<br>
<br>

### Actuator Designs

<!-- <div style="text-align: center;">
  ESSPG Actuator with gear ratio 7.2:1. (a, b) Design for Manufacturing; (c, d) Template Designs.
  <img src="/img/Codesign/esspg_actuator.png" alt="drawing" width="50%"/>
</div>

<div style="text-align: center;">
  ISSPG Actuator with gear ratio 6:1. (a, b) Design for Manufacturing; (c, d) Template Designs.
  <img src="/img/Codesign/isspg_actuator.png" alt="drawing" width="50%"/>
</div> -->

<!-- Table -->

<!-- | Gearbox Type | Gear Ratio |       (a, b) Design for Manufacturing; (c, d) Template Designs        |
|--------------|------------|-----------------------------------------------------------------------|
|     ESSPG    |   7.2:1    |<img src="/img/Codesign/esspg_actuator.png" alt="drawing" width="80%"/>|
|     ISSPG    |    6:1     |<img src="/img/Codesign/isspg_actuator.png" alt="drawing" width="80%"/>| -->

<div style="display: flex; justify-content: center; margin-top: 20px;">
  <table style="border-collapse: collapse; text-align: center; width: 80%; border: 1px solid #ddd;">
    <thead>
      <tr style="background-color: #f2f2f2;">
        <th style="padding: 10px; border: 1px solid #ddd;">Gearbox Type</th>
        <th style="padding: 10px; border: 1px solid #ddd;">Gear Ratio</th>
        <th style="padding: 10px; border: 1px solid #ddd;">(a, b) Design for Manufacturing; (c, d) Template Designs</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td style="padding: 10px; border: 1px solid #ddd;">ESSPG</td>
        <td style="padding: 10px; border: 1px solid #ddd;">7.2:1</td>
        <td style="padding: 10px; border: 1px solid #ddd;">
          <img src="/img/Codesign/esspg_actuator.png" alt="ESSPG Actuator" style="width: 80%;" />
        </td>
      </tr>
      <tr>
        <td style="padding: 10px; border: 1px solid #ddd;">ISSPG</td>
        <td style="padding: 10px; border: 1px solid #ddd;">6:1</td>
        <td style="padding: 10px; border: 1px solid #ddd;">
          <img src="/img/Codesign/isspg_actuator.png" alt="ISSPG Actuator" style="width: 80%;" />
        </td>
      </tr>
    </tbody>
  </table>
</div>

<br>
<br>

### Future Work

- We aim to extend this research to multi-stage planetary, cycloidal, and strain-wave gearboxes for broader actuator optimization applicability.
- We plan to optimize actuator-to-joint transmission systems, investigating belts, chains, and linkages with detailed mass and efficiency models.
- We aim to integrate actuator optimization into system-level co-design for legged robots like monopeds, bipeds, and quadrupeds.
