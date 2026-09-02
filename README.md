# PID-Controlled-DC-Motor
A closed loop control of a JGA25-371 gearmotor using position feedback with a magnetic encoder running at 50Hz using a microcontroller.
## Features
Logic is currently managed by the Arduino UNO R3.
The L298N motor driver is used.
The L298N has a voltage drop off of around 2V, given the voltage source used provides 9V this leaves the  motor with a maximum of 7V hence a minimum PWM value of 60 us implemented.

