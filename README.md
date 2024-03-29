# Craftbeerpi4 Kettle Logic Plugin

## PID Logic with boil threshold.

If the target Temperature is above a configurable threshold the PID will be ignored and heater is switched on to the max output value. This is helpful if you use the same kettle for mashing and boiling.

Once the boil threshold temperature is reached, the boil will be done with the max boil output power


### Installation:

Please have a look at the [Craftbeerpi4 Documentation](https://openbrewing.gitbook.io/craftbeerpi4_support/readme/plugin-installation)

- Package name: cbpi4-PIDBoil
- Package link: https://github.com/PiBrewing/cbpi4-pidboil/archive/main.zip


### Parameters

![PIDBoil Settings](https://github.com/avollkopf/cbpi4-PIDBoil/blob/main/cbpi4-PIDBoil-logic.png?raw=true)

- P - proportional value
- I - integral value
- D - derivative value
- SampleTime - 2 or 5 seconds -> how often the logic calculates the power setting
- max output - heater power which is set above boil threshold
- Boil Threshold - Above this temperature the heater will be set to Max Boil Output Power (default: 98°C / 208F)
- Max Boil Output - Power (%) that is used above Boil Threshold Temperature (default: 100%)

### Changelog

- 29.12.22: (0.0.9) Fixed Bug related to Boil Threshold Parameter
- 10.05.22: (0.0.8) Updated README (removed cbpi add)
- 10.05.22: (0.0.7) Removed cbpi dependency
- 01.12.21: (0.0.6) If current kettle power is different from kettle logic. logic will overrule kettle power setting
- 21.11.21: (0.0.5) Adapted to cbpi4 4.0.0.45 to accomodate actor power settings incl. the PWM Actor.
- 13.10.21: (0.0.4) Added Power setting for Boil
- 13.10.21: (0.0.3) Improvement of actor toggling in case of 0% or 100% heating
- 12.10.21: (0.0.2) Bug fixing MashStep Automode Issue
- 19.08.21: (0.0.1) Initial commit
