<!-- docs/README.md -->

# PID controller

PID (proportional–integral–derivative) controller - is a type of feedback controller that uses a mathematical model to regulate a process. The controller uses a control loop feedback mechanism to control the process variable and minimize the error between the desired setpoint and the actual output of a system. It does this by adjusting an input to the system based on PID.

!> The controller knows nothing about your physical system, the simulation, the absolute values. It just gives a control signal depending on the error.

PID control is structured around three distinct elements, each contributing to the overall control mechanism. These components are the Proportional, Integral, and Derivative terms. They are combined to regulate the process variable, each addressing a specific aspect of the control process.

An easiest way to understand the role of the gains is that the KP works on the present error, KI on the past error (integral), and KD on the prediction of future error (derivative).

A little bit of math and diagrams:

![](./img/PID_Formula.svg ':size=40%')

![](./img/PID_Diagram.webp ':size=40%')
