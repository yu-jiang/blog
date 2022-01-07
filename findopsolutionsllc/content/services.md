---
title: "Consulting Services"
date: 2022-01-01T15:35:50-05:00
draft: false
---

## Consulting Services
Findop Solutions LLC provides technical consulting services on

* Helping you identify the right tools from control and optimization theories for your specific engineering applications
* Prototyping control algorithms 
(e.g., PID, LQR, Adaptive, Robust, Learning-based) for various applications
* Reviewing control architecture and algorithms design
* Fundamentals on Simulink/Simscape modeling and model-based-design
* Literature review / patent research on autonomous driving and robotics related inventions

Note that due to my current engagement with ClearMotion, I will not be able to work on things related to **active vehicle suspension systems**

## Sample Projects
Here is list of selected projects I worked on for both my full-time employers and clients. For the sake of confidentiality, I will provide only the minimum information.

### Operating point search on a Simscape model of a backhoe
This was the major cross-team application project I participated at MathWorks. The client makes backhoe machines and needed enhanced feature in Simulink Control Design to effectively trim the model (i.e., find the operating point). I led the work on reformulating the optimization problem in model trimming and developed the enhanced features. See [MathWorks Example: Steady-State Simulation with Projection-Based Trim Optimizer](https://www.mathworks.com/help/slcontrol/ug/steady-state-simulation-with-projection-based-trim-optimizer.html) that illustrates this feature.

### Low-speed truck-trailer planning and control
As the tech lead in controls at ISEE AI, I prototyped the first version of control systems (speed regulation, steering, and gear shifting) for autonomous yard trucks. I also designed the first interface between planner and controller. See [ISEE AI's official website](https://www.isee.ai) for video footages of the company's yard trucks operating in the real world.

(Note: I left ISEE AI in April 2020. I am not subject to any non-compete restrictions.)

### Preview suspension control (RoadMotion)
This has been my major focus at ClearMotion. We collected road surface data and use that for proactive active suspension control. See [The RoadMotion Project](https://www.clearmotion.com/roadmotion/) for more details.

### Torque vectoring optimization and control
The client is making a certain type of vehicles that can distribute individual torques to different wheels. I helped with formulating it into an optimazation problem to achieve optimal torque vectoring and implemented a real-time solver for it.

### ACC controller design for OTR trucks
The client is making electrical over-the-road trucks, and the scope of the consulting work is to prototype the first version of an adaptive cruise controller through iterations between simulation and analyzing vehicle testing data.

### Simscape modeling and MBD design
The client is making excavator-like heavy equipment for mining purpose. The work is to provide training, guidance, and trouble-shooting on simscape modeling regarding the hydraulic and mechanical components of the system. Also, training on model-based-design workflow with [Speedgoat](https://www.speedgoat.com) is provided.