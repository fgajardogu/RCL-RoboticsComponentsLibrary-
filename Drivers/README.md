# Power Drivers

## Motor Drivers

### H Bridges
* __L298N__ -> Beginner friendly, available.
* __TB6612FNG__ -> Best efficiency, less heat.
* __BTS7960__ -> High Current Beast. 
* __Cytron MD10C__ -> Efficient All-rounder.
* __Pololu G2 Series__ -> Small Size, Efficient precision driver.. 

| Feature | L298N | TB6612FNG | BTS7960 | MD10C | G2 |
| ------- | ----- | --------- | ------- | ----- | -- |
| Tech. | BJT Transistor | N/P Mosfets | H.C. Mosfets | Mosfets | Mosfets |
| Power Volt. | 5V-35V | 4V5-13V5 | 6V-27V | 6V-30V | 4V5-18V |
| Logic Volt. | 5V | 2V7-5V5 | 5V | 5V | 2V7-5V5 |
| C. Current | 2A | 1A2 | 43A | 10A | 3A |
| P. Current | 3A | 3A2 | 75A | 30A | 6A |
| Volt. Drop | 2-4 V | <.5V | <.2V  | <.15V  | <.2V  |
| Efficiency | 40-60 % | >90 % | >95 % | >90 % | >90 % |
| PWM Freq | <5kHz | <100kHz | <25kHz | <20kHz | <100kHz |
| Protections | Thermal Shutdown | Thermal, UVLO | Thermal, Overcurrent, Undervolt, shortcircuit | OVP,UVP,OPT,OCP, Stall | UVLO, Overcurrent, thermal shutdown |
| HeatSink | Required | No required | Recomended (when high current) | Depends | No required |
| Best For | Basic, Low Power | Compact Robots, Line Followers | High Power, RC Cars, CNC, Heavy loads | Robots, RC, CNC, High perf | Drones, Robotics, Battery powered, precision. |