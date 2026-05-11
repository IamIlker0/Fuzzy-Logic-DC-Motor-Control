# DC Motor Speed Control using Fuzzy Logic

This repository contains a **MATLAB/Simulink** implementation of a Fuzzy Logic Controller (FLC) designed for the speed regulation of a DC motor. The project focuses on maintaining a setpoint speed and ensuring robust **disturbance rejection** under sudden load changes.

## Project Overview

In industrial applications, DC motors are often subject to external torques that can cause speed fluctuations. This project demonstrates how a **Mamdani-type Fuzzy Inference System** can be used to restore the motor's speed quickly and accurately without steady-state error.

### Key Features:
- **Control Strategy:** Fuzzy Logic (Error and Change of Error as inputs).
- **Target Speed:** 50 rad/s.
- **Disturbance:** External load torque applied at $t = 5s$.
- **Software:** MATLAB / Simulink.

## System Architecture
The control loop includes the DC motor transfer function, an integrator for zero steady-state error, and the Fuzzy Logic Controller block.

<img width="1101" height="475" alt="Ekran görüntüsü 2026-05-11 095256" src="https://github.com/user-attachments/assets/db1a2805-b26b-4266-9aa2-75838f68e8cb" />

## Performance & Results
The simulation results show the controller's effectiveness. When the disturbance occurs at the 5th second, the system experiences a momentary drop but recovers back to the **50 rad/s setpoint** within approximately 2 seconds.

<img width="702" height="629" alt="Ekran görüntüsü 2026-05-11 100851" src="https://github.com/user-attachments/assets/e40a0011-69c3-43ab-aa9b-45b67039b00c" />

## How to Use
1. Clone or download this repository.
2. Ensure `dc_motor_fuzzy_control.slx` and `fuzzy_controller.fis` are in the same directory.
3. Open the `.slx` file in MATLAB.
4. Run the simulation to observe the system response in the Scope block.

---
*Developed as part of a Mechatronics Engineering control systems project.*
