# Autonomous-IndyCar-Controller
**Simulation of GPS waypoint-based path following for an IndyCar using classical PID controllers in MATLAB/Simulink**  
*(Course project: Control systems modeling, PID design, Simulink simulation)*

## Goal / Overview
- **Primary Features**:
  - Waypoint-based reference trajectory from GPS coordinates
  - Lateral control to minimize cross-track error and heading error
  - Closed-loop steering commands for autonomous track following
  - Implemented and compared three controllers:
    - **Proportional (P)** — basic proportional correction
    - **Proportional-Integral (PI)** — removes steady-state error (especially useful on curves)
    - **Proportional-Integral-Derivative (PID)** — adds damping → smoother tracking, less overshoot/oscillation
- **Motivation**: Demonstrate classical control techniques applied to autonomous vehicle path following; evaluate trade-offs in tracking accuracy, stability, and dynamic response (curves, varying speeds).
- **Outcome**: Simulated successful lap completion with quantifiable metrics (RMS cross-track error, settling time, overshoot); PID showed best overall balance of performance.

## Programs and skills required
- **Modeling & Simulation**: MATLAB (scripting, plotting, waypoint handling), Simulink (vehicle dynamics block, controller implementation, closed-loop simulation)
- **Control Theory**: PID control laws, manual tuning (Kp, Ki, Kd), stability analysis, step response interpretation
- **Toolboxes**: Control System Toolbox, Simulink
- **Data Analysis**: Calculation of error metrics (RMS cross-track error), visualization of trajectories, performance comparison plots
- **Other**: Systems thinking, debugging dynamic models, interpreting simulation results

## Key Takeaways and lessons
- The derivative term is essential for reducing oscillations and improving response on curved sections.
- Integral action effectively eliminates steady-state offset that pure P or PD controllers leave behind.
- Simulink is extremely powerful for rapid prototyping and visual debugging of control performance.
- Classical PID gives strong baseline results for path following; for high-speed racing scenarios, more advanced techniques (MPC, Stanley controller, etc.) would likely outperform it.
- Sensor noise, actuator delays, and model mismatches would need addressing in real hardware (e.g., via Kalman filtering or robust tuning).

## Project Links
- **Final Systems Presentation** (PDF with methodology, results, plots, conclusions):  
  [Systems Final Presentation](https://github.com/Alec-Hudson24/Autonomous-IndyCar-Controller/blob/main/Systems.Final.Presentation%20(1).pdf)

## Model Photo
![Track Simulation Overview](https://github.com/Alec-Hudson24/Autonomous-IndyCar-Controller/blob/main/IndyCar%20Going%20Around%20Track.PNG)

*The autonomous IndyCar following the waypoint path using the tuned controllers*

*This was for a class called System Dynamics and Controls*

[Back](https://github.com/Alec-Hudson24)
