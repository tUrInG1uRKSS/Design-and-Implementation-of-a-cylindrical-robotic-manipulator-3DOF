# Design and Implementation of a Cylindrical Robotic Manipulator (3DOF)
![vista](https://github.com/user-attachments/assets/477fc6bc-2854-445a-aa8a-e73820bc69a5)

## Overview
This repository contains the documentation and design files for a 3-Degree-of-Freedom (3DOF) cylindrical robotic manipulator. The project was developed as part of the Multibody System Dynamics (MT516) course at the National University of Engineering (UNI), Lima, Peru.

The project focuses on the design, mechanical analysis, electronic integration, and construction of a robot capable of performing pick-and-place operations using a cylindrical coordinate system (RPP - Rotational, Prismatic, Prismatic).

## Project Status
* **Current Content:** Design, Implementation, Kinematic Analysis, and Application reports.
* **Upcoming Content:** MATLAB simulation scripts and Arduino control code (to be uploaded).
<img width="1255" height="973" alt="image" src="https://github.com/user-attachments/assets/ff9be8af-e177-429c-8158-9e5ca019e6d2" />

<img width="1182" height="896" alt="image" src="https://github.com/user-attachments/assets/82698e36-785e-4cfa-8e9f-f17f8e5acf91" />

## Features
* **Configuration:** Cylindrical (RPP).
* **Degrees of Freedom:** 3 (1 Rotational, 2 Linear).
* **Control System:** Arduino-based control using CNC Shield and GRBL compatibility.
* **Mechanical Structure:** Custom 3D printed parts, aluminum rods, and lead screws.

## Hardware Specifications

### Electronics
* **Microcontroller:** Arduino UNO R3 (SMD version)
* **Shield:** CNC Shield V3.0
* **Drivers:** DRV8825 Stepper Drivers (1/32 microstepping)
* **Motors:**
    * NEMA 17 Stepper Motor (JK42HS60-1704) - 7.3 kg.cm torque
    * NEMA 17 Stepper Motor (JK42HS40-1704) - 4.2 kg.cm torque
* **Power Supply:** Switching Power Supply 12V 10A (120W)

### Mechanical Components
* **Linear Motion:** 8mm Lead Screws (T8) with anti-backlash nuts.
* **Guides:** 8mm smooth rods with SC8UU linear bearings.
* **Transmission:** Worm gear mechanism for the base rotation (Joint 1).
* **Couplers:** Flexible aluminum couplers (5mm to 8mm).
<img width="707" height="808" alt="image" src="https://github.com/user-attachments/assets/69ca3f80-468e-4bdc-aa8b-b11e8a93a7ad" />
<img width="886" height="1184" alt="image" src="https://github.com/user-attachments/assets/39dea0b9-6807-4597-8e5b-0022bdf6ba39" />

## Kinematics and Workspace
The robot operates in a cylindrical workspace defined by the following joint limits:

| Joint | Type | Variable | Range |
| :--- | :--- | :--- | :--- |
| **Joint 1** | Rotational (Base) | $\theta_1$ | $0^\circ < \theta_1 < 360^\circ$ |
| **Joint 2** | Prismatic (Vertical) | $d_2$ | $90 \text{ mm} < d_2 < 537 \text{ mm}$ |
| **Joint 3** | Prismatic (Horizontal)| $d_3$ | $90 \text{ mm} < d_3 < 532 \text{ mm}$ |

## Documentation
The `reports/` folder (or root directory) currently contains the following detailed documents:
1.  **InformeT1-Design.pdf:** Detailed mechanical and electronic design, component selection, and CAD assembly (SolidWorks/Eagle).
2.  **InformeT2-Implementation.pdf:** Physical assembly process and integration.
3.  **InformeT3-AnalisisCinematico.pdf:** Mathematical modeling of the robot's motion.
4.  **InformeT4-Aplicacion.pdf:** Specific application and testing of the manipulator.

## Software Tools
* **CAD Design:** SolidWorks
* **PCB Design:** Eagle
* **Control:** Arduino IDE (Code coming soon)
* **Simulation:** MATLAB (Scripts coming soon)

## Authors
* **Angel Steven Belleza Martínez**
* **Fidel Angel Castro Suazo**
* **Marco Leandro Llontop Herrera**

**Supervisor:** Ing. Ivan Calle Flores

---
*University: Universidad Nacional de Ingeniería (UNI)*
*Faculty: Facultad de Ingeniería Mecánica*
*Date: 2022*
