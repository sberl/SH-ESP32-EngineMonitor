Code for monitoring temperatures, and eventually other data from boat engine.

Currently can monitor 2 temperatures. 
  - Engine coolant temperature
  - Engine oil temperature

Would like to add later
  - Engine RPM
  - Engine state: On/off and transmission state forward, reverse, neutral
  - Engine fuel flow rate

The ESP32 connects to a signalk server over WiFi. 
No NMEA2000 connection yet, though the example code contains that function. Signalk can resend the data it receives from this device over NMEA2000.

Board is powered from engine electrical 12V. Not sure yet if it will be "always on", or will turn on when engine ignition key turns on.

This is based on 
https://github.com/hatlabs/SH-ESP32-onewire-temperature
# SH-ESP32 1-Wire temperature sensor example

This repo implements an example engine temperature sensor for the SH-ESP32 development board using Signal K and the SensESP library.
The temperatures are measured using 1-Wire DS18B20 sensors.
