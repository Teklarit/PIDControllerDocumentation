# Manual tuning

An alternative way to understand the role of the gains is that KP works on the current error, KI on the past error (integral), and KD on predicting the future error (derivative).

1. Set all values ​​to 0.
2. Increase Kp until the system starts to oscillate constantly.
3. Increase Kd until the oscillations disappear.
4. Repeat steps 2-3 and take the last stable values.
5. Increasing Ki eliminates the stable error. (The error accumulates with the coefficient, the signal is pulled up).

It is not necessary to select all 3 coefficients of the controller. If the Kp coefficient is enough for your case, this is a P-controller. Kp and Kd are a PD controller. All 3 are a PID controller. Keep the controller as simple as possible.