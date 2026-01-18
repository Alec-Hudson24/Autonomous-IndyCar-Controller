# Autonomous IndyCar Controller

**Simulation of GPS waypoint-based path following for an IndyCar using classical PID controllers in MATLAB/Simulink**

## Goal/Overview
Designed and implemented lateral controllers for an autonomous IndyCar to follow a predefined track using GPS waypoints. The vehicle autonomously navigates the circuit by minimizing cross-track error and heading deviation.

Implemented and compared three controllers:
- **Proportional (P)** — Basic error correction
- **Proportional-Integral (PI)** — Eliminates steady-state error
- **Proportional-Integral-Derivative (PID)** — Adds damping for smoother response and reduced overshoot

The goal was to evaluate controller performance on tracking accuracy, stability, and response to dynamic track conditions (curves, speed variations).

## Programs and Skills Required
- Control theory: PID control laws, tuning (Kp, Ki, Kd), stability analysis
- MATLAB (scripting, plotting, waypoint generation)
- Simulink (modeling vehicle dynamics, controller blocks, simulation)
- MATLAB plugins/toolboxes: Control System Toolbox, Simulink
- Data analysis: Error metrics (e.g., RMS cross-track error), step response, simulation visualization

## Key Features & Implementation
- Waypoint-based reference path (GPS coordinates converted to trajectory)
- Vehicle kinematic/dynamic model in Simulink
- Closed-loop simulation: Controller computes steering/throttle inputs based on current position/error
- Comparison: Step responses, tracking plots, lap completion time, overshoot/settling time

## Key Takeaways & Lessons Learned
- PID tuning is critical: Derivative term reduces oscillations, Integral eliminates steady-state offset on curves.
- Simulink excels for rapid prototyping and visualization of control performance.
- Real-world considerations: Sensor noise, actuator delays, and computational limits would require further robustness (e.g., Kalman filtering).
- PID provides solid baseline performance for path following; advanced methods (MPC, Stanley) could improve high-speed tracking.

## Project Links & Resources
- **Final Systems Presentation** (PDF with methodology, results, conclusions):  
  [Systems.Final.Presentation.pdf](https://github.com/user-attachments/files/24333923/Systems.Final.Presentation.pdf)

## Visual
(Include screenshots from your presentation or new ones — upload to repo /images folder)

![Track Simulation Overview]()  
*The Car making its way around the track using our controllers



This project was part of System Dynamics and Controls, demonstrating application of classical control to autonomous systems.
