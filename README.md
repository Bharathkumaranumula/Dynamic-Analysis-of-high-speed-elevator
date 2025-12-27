# High-Speed Elevator – Dynamic Analysis & MATLAB Simulation

## About This Fork
This repository is a fork of the **High-Speed-Elevator** project.  
I am an active contributor to this project, and my primary responsibility was the **dynamic analysis of high-speed elevators**, with emphasis on **vibration behavior in skyscraper applications**.

My contributions include:
- Research on dynamic behavior of high-speed elevators
- Dynamic modeling of elevator vibration systems
- MATLAB-based simulation and analysis
- Interpretation of vibration results for ride comfort and safety

---

## Project Overview
High-speed elevators are critical vertical transportation systems in high-rise and supertall buildings, typically operating at speeds ranging from **5 m/s to over 20 m/s**.  
At such speeds, mechanical vibrations significantly influence passenger comfort, system stability, and structural safety.

This project focuses on:
- Understanding the physical sources of vibrations
- Developing suitable dynamic modeling approaches
- Simulating vibration responses using MATLAB
- Identifying parameters for vibration reduction

---

## Types of Vibrations
The vibration analysis is divided into two major categories:

---

## Horizontal Vibrations (Lateral Dynamics)

### Background
Horizontal vibrations occur due to interaction between the elevator car, guide rails, guide shoes, and building sway. These vibrations directly affect ride comfort and lateral stability.

### Primary Causes
- Guide rail misalignment or waviness  
- Nonlinear stiffness and damping of guide shoes  
- Uneven mass distribution in the elevator car  
- Transmission of building sway through rail brackets  

### Dynamic Modeling
- The elevator car is modeled as a rigid body with dominant lateral translation and yaw motion.
- Guide shoes are represented using equivalent spring–damper elements to capture contact stiffness and energy dissipation.
- Guide rails are modeled as flexible structural members influenced by building motion.
- The interaction between the car and guide rails is treated as a coupled dynamic system.
- System response is evaluated using numerical simulation techniques.

### MATLAB Implementation
- Definition of mass, stiffness, and damping parameters
- Evaluation of system natural frequencies
- Time-domain response analysis using numerical solvers
- Parametric studies on guide stiffness, damping, and elevator speed

---

## Vertical Vibrations (Longitudinal Dynamics)

### Why Vertical Vibrations Occur
- Elastic stretching of hoisting ropes
- Sudden torque changes during acceleration and braking
- Inertia of the car, counterweight, and traction wheel
- Uneven rope tension and time-varying rope length

Vertical vibrations are particularly severe during emergency braking conditions.

### Modeling Approach
A **3-DOF lumped mass model** is used, consisting of:
- Elevator car
- Counterweight
- Traction wheel

These components are connected through rope stiffness and damping, forming a non-stationary dynamic system.

### System Assumptions
- Rope always remains in tension
- Car and counterweight behave as rigid bodies
- Rope elasticity follows Hooke’s law
- Only vertical motion is considered

### MATLAB Simulation
- Definition of physical parameters such as mass, stiffness, and damping
- Inclusion of time-varying rope length effects
- Numerical integration using ODE solvers
- Analysis of acceleration and jerk related to passenger comfort

---

## MATLAB Codes
This repository includes MATLAB scripts for:
- System parameter initialization
- Dynamic model implementation
- Eigenvalue and frequency analysis
- Time-domain vibration response simulation
- Comparison between structural frame and passenger cabin response

---

## Optimization & Design Insights
- Increasing damping effectively reduces vibration amplitude
- Proper guide shoe stiffness improves lateral stability
- Vibration isolation minimizes vibration transmission to the passenger cabin
- Optimized dynamic parameters lead to smoother and safer ride quality

---

## Key Outcomes
- Clear distinction between horizontal and vertical vibration mechanisms
- Validated modeling approaches through MATLAB simulations
- Practical insights into vibration reduction for high-speed elevators
- Improved understanding of ride comfort and safety constraints

---

## References
Relevant research papers and technical references are provided in the project documentation.
