# High-Speed Elevator – Dynamic Analysis & MATLAB Simulation

## About This Fork
This repository is a fork of the **High-Speed-Elevator** project.  
I am an active contributor to this project, and my primary responsibility was the **dynamic analysis of high-speed elevators**, with emphasis on **vibration behavior in skyscraper applications**.

My contributions include:
- Research on dynamic behavior of high-speed elevators
- Mathematical modeling of elevator vibration systems
- MATLAB-based simulation and analysis
- Interpretation of vibration results for ride comfort and safety

---

## Project Overview
High-speed elevators are critical vertical transportation systems in high-rise and supertall buildings, typically operating at speeds ranging from **5 m/s to over 20 m/s**.  
At such speeds, mechanical vibrations significantly influence passenger comfort, system stability, and structural safety.

This project focuses on:
- Understanding the source of vibrations
- Developing dynamic models
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
- Elevator car modeled as a rigid body with lateral translation and yaw rotation
- Guide shoes represented as spring–damper elements
- Guide rails modeled as Euler–Bernoulli beams
- Car–rail interaction treated as a coupled dynamic system

### Mathematical Representation
The horizontal vibration system is expressed as:


where:
- `M` – Mass matrix  
- `C` – Damping matrix  
- `K` – Stiffness matrix  

### MATLAB Implementation
- Definition of system matrices (M, C, K)
- Eigenvalue analysis for natural frequencies
- Time-domain response using numerical solvers
- Parametric studies on stiffness, damping, and elevator speed

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

### Mathematical Formulation
Equations of motion are derived using **Lagrange’s method**, incorporating:
- Gravitational forces
- Rope elastic and damping forces
- Traction wheel dynamics

### MATLAB Simulation
- Definition of physical parameters (mass, stiffness, damping)
- Time-varying rope length modeling
- Numerical integration using ODE solvers
- Analysis of acceleration and jerk for passenger comfort

---

## MATLAB Codes
This repository includes MATLAB scripts for:
- Parameter initialization
- Mass–stiffness–damping matrix formulation
- Eigenvalue and frequency analysis
- Time-domain vibration response simulation
- Frame vs passenger cabin acceleration comparison

---

## Optimization & Design Insights
- Increasing damping reduces vibration amplitude
- Proper guide shoe stiffness improves lateral stability
- Vibration isolation reduces transmission to passenger cabin
- Optimized parameters lead to smoother ride quality

---

## Key Outcomes
- Clear distinction between horizontal and vertical vibration mechanisms
- Validated dynamic models using MATLAB simulations
- Insights into vibration reduction for high-speed elevators
- Improved understanding of ride comfort and safety constraints

---

## Author Contribution
**Anumula Bharath Kumar**  
Dynamic analysis, vibration modeling, and MATLAB simulation for high-speed elevator systems.

---

## References
Relevant research papers and technical references are provided in the project documentation.
