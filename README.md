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
The vibration analysis in this project is divided into two major categories:

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

### MATLAB Simulation – Horizontal Vibrations
MATLAB is used to simulate the lateral dynamic behavior of the elevator system using the following technical approach:

- Formulation of lumped-parameter dynamic models for lateral motion
- Assembly of mass, stiffness, and damping matrices representing car–guide interactions
- Eigenvalue and modal analysis to evaluate natural frequencies and mode shapes
- Time-domain response simulation using numerical ODE solvers such as `ode45`
- Parametric studies on guide shoe stiffness, damping, and elevator speed
- Visualization of lateral displacement, velocity, and acceleration responses using MATLAB plotting tools
- Evaluation of ride comfort based on lateral acceleration levels

---

## Vertical Vibrations (Longitudinal Dynamics)

### Why Vertical Vibrations Occur
- Elastic stretching of hoisting ropes
- Sudden torque changes during acceleration and braking
- Inertia of the car, counterweight, and traction wheel
- Uneven rope tension and time-varying rope length

Vertical vibrations are particularly severe during transient events such as emergency braking.

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

### MATLAB Simulation – Vertical Vibrations
The vertical vibration behavior is analyzed in MATLAB using the following workflow:

- Development of a lumped mass dynamic model incorporating rope elasticity and damping
- Inclusion of time-varying rope length to capture non-stationary system behavior
- Implementation of governing equations using MATLAB scripts and function files
- Time-domain numerical integration using solvers such as `ode45` and `ode15s`
- Simulation of acceleration and braking conditions, including emergency braking cases
- Post-processing of results to analyze displacement, acceleration, and jerk
- Comparative assessment of vibration levels between structural frame and passenger cabin

---

## MATLAB Codes
This repository contains MATLAB scripts and functions for:
- System parameter initialization
- Dynamic model implementation for horizontal and vertical vibrations
- Eigenvalue and frequency analysis
- Time-domain vibration response simulation
- Parametric and comparative studies
- Visualization of vibration characteristics

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
- Practical insights into vibration reduction strategies for high-speed elevators
- Improved understanding of ride comfort and safety constraints

---

## References
Relevant research papers and technical references are provided in the project documentation.
