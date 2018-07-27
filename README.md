# PumpControl
Arduino-based pressure-dependent pump control 

## Summary

We have a pump that we use to water plants in the garden with rainwater. The distance between pump and garden beds is long enough that you don't want to run back and forth to turn the pump on and off. Furthermore, you don't want the pump to run dry.

The idea came up to add a pressure sensor at the output of the pump and a relay to turn the pump on and off based on pressure.

That works quite well.

## Festures

- Three configurable thresholds:
  - protection pressure: if pressure is below, pump is turned off
  - on pressure: if pressure falls below, pump is turned on
  - off pressure: if pressure is above, pump is turned off
- Before the pump is turned off, a delay is used
- To start the pump while below protection pressure, a manual on switch can be used
- An I2C OLED Display shows all pressures and allows for on-the-fly adjustments
