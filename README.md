# Craftbeerpi4 Kettle Logic Plugin

### PID Logic with boil threshold.

If the target Temperature is above a configurable threshold the PID will be ignored and heater is switched on constantly. This is helpful if you use the same kettle for mashing and boiling.

The code is ported form the cbpi3 version with some minor fixes and additional features( >= 0.0.3)

### Parameter

	P - proportional value

	I - integral value

	D - derivative value

	max output - heater power which is set above boil threshold

	Boil Threshold - Above this temperature the heater will be set to Max Boil Output Power (default: 98°C / 208F)

	Max Boil Output - Power (%) that is used above Boil Threshold Temperature (default: 100%)

### Changelog

- 19.08.21: Initial commit (0.0.1)
- 12.10.21: Bug fixing MashStep Automode Issue (0.0.2)
- 13.10.21: Improvement of actor toggling in case of 0% or 100% heating (0.0.3)
- 13.10.21: Added Power setting for Boil (0.0.4)
