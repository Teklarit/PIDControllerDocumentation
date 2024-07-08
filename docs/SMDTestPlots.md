# SMD test plots

Arbitrary physical system (mass-spring-damper model):

![](./img/SMD_Theory.PNG ':size=25%')

Some force must be applied to move the object to the desired position. Graph with the object position (result of the simulation of the physical system) for a constant value:

![](./img/SpringMassDamper.svg ':size=40%')

**Task:** to reach the desired value (position) in the shortest time and maintain the desired position, minimizing oscillations and errors.

We use a PID controller. The controller gives a signal (what force should be applied over time) to reach the desired value (knowing only the current value and the desired one).

## Kp:

![](./img/PID_0.0_0.0_0.0.svg ':size=40%')
![](./img/PID_0.5_0.0_0.0.svg ':size=40%')
![](./img/PID_1.0_0.0_0.0.svg ':size=40%')
![](./img/PID_3.0_0.0_0.0.svg ':size=40%')
![](./img/PID_5.0_0.0_0.0.svg ':size=40%')
![](./img/PID_10.0_0.0_0.0.svg ':size=40%')

## Ki:

![](./img/PID_5.0_0.5_0.0.svg ':size=40%')
![](./img/PID_5.0_1.0_0.0.svg ':size=40%')
![](./img/PID_5.0_3.0_0.0.svg ':size=40%')
![](./img/PID_5.0_5.0_0.0.svg ':size=40%')

## Kd:

![](./img/PID_5.0_3.0_0.5.svg ':size=40%')
![](./img/PID_5.0_3.0_1.0.svg ':size=40%')
![](./img/PID_5.0_3.0_3.0.svg ':size=40%')
![](./img/PID_5.0_3.0_5.0.svg ':size=40%')
