# Craftbeerpi4 Kettle Logic Plugin

## PID Logic with boil threshold.

If the target Temperature is above a configurable threshold the PID will be ignored and heater is switched on constantly. This is helpful if you use the same kettle for mashing and boiling.

### Parameter
P - proportional value
I - integral value
D - derivative value
max output - heater power which is set above boil threshold
Boil Threshold - Above this temperature the heater will be constantly on
