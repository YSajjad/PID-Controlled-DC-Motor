# PID-Controlled-DC-Motor
A closed loop control of a JGA25-371 gearmotor using position feedback with a magnetic encoder running at 50Hz using a microcontroller. 
The target position can be specified by turning the rotary device, this is displayed on the LCD - the motor will then adjust to reach the specified position using PID logic.

<img width="810" height="605" alt="image" src="https://github.com/user-attachments/assets/ae5ea688-59e2-4cf3-b3c1-c3a937c6dd19" />

## Components
- JGA25-371 gearmotor with magnetic encoder
- Arduino UNO R3
- L298N motor driver
- KY-040 rotary encoder
- 2X16 LCD with I2C backpack

## Features
- A KY-040 rotary encoder is used to set the target position, this is displayed on an LCD with an I2C backpack
- Logic is currently managed by the Arduino UNO R3.
- The L298N motor driver is used.
- The L298N has a voltage drop off of around 2V, given the voltage source used provides 9V this leaves the  motor with a maximum of 7V hence a minimum PWM value of 60 us implemented.
- Via the use of millis() the code is none time blocking


## Tuning and PID
PID is a feedback loop system which 
PID tuning is a process of adjusting the 3 PID to eliminate error and come to the target quicker.
The system was tuned via the Arduino IDE serial plotter.


## Future development

In the future adding speed based feedback using a target RPM is to be implemented.
