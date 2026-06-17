# Components
A list of usefull components and suppliers for my electronics projects : 

## Power Conversion // Supply : 
When powering different different devices, the needs of noise inmunity and reliability may change with components specs. As general rule, inductive loads (relays, solenoids, motors) storage energy, so when they're switched off, the circuit collapses for a small moment (nanoseconds) 

### Flyback SMPS Transformers 
| Brand | Model | V_in range | V_out | Max Iout | Efficiency | Applications |
| ----- | ----- | ---------- | ----- | -------- | ---------- | ------------ |
| MeanWell | LRS-35-24 | 85-264VAC or 120-373VDC | 24V | 1A5 | ~87% | Industrial cabinets. |
| MeanWell | DR-60-24 | 86-305VAC or 124-370VDC | 24V | 2A5 | ~89% | Same but DIN mount. |
| Recom | RAC03-24SK | 85-264VAC | 24V | .125A | ~78% | LowPower Nodes on PCB. |
| MeanWell | LRS-35-5 | 85-264VAC or 120-373VDC | 5V | 7A | ~82% | MCU or PC clusters |
| MeanWell | IRM-05-5 | 85-305VAC or 120-430VDC| 5V | 1A | ~75% | Small control on PCB. 
| Recom | RAC05-05SK | 85-305VAC | 5V | 1A | ~78% | Same, reinfornced isolation.

* __MeanWell LRS Series__ : LRS-Wattage-output.
* __MeanWell IRM Series__ : IRM-Wattage-output.
* __Recom AC/DC RAC0X-K__ : X is the Wattage and K the V output, current depends on the mix.


### Isolated Flyback BuckConverters DC-DC
Special BuckConverters that isolates the input from the output, killing the ground bouncing possibility, although we still have the spikes traspassing possibility. Being Buck Converters they are highly efficient.

| Brand | Model | V_in range | V_out | Max Iout | Efficiency | Applications | 
| ----- | ----- | ---------- | ----- | -------- | ---------- | ------------ |
| MeanWell | RSD-30G-5 | 9-36V | 5V |  6A | ~89 | General power of logic level when main rail is dirty. |
| MeanWell | RSD-60G-5 | 9-36V | 5V | 12A | ~88% | Extended power of logic level when main rail is dirty. |
| TracoPower | TEN 25-2411 | 18-36V | 5V | 5A | ~85% | Low-Power isolated sensors or COM ports DIP module | 
| Murata | NXE2S0505MC | 4.5-5.5V | 5V | .4A | ~80 | Signal Isolation power for nois breaking. |

* __MeanWell RSD Series__ : RSD-Power(input_id)-V_out, for input id we can have G (9-36), L (18-72) and H(40-160).
* __TracoPower TEN 25 series__ : TEN 25 Vin-Vout. Vout can be 10 (+3V3), 11(+5V), 12(+12V), 13(+15) or 22(+/-12V), 23(+/-15V) 
* __Murata NXE2 Series__ : NXE2-Vin-Vout-MC, Vin can be 5V or 12V and Vout 5V, 12V or 15V. Vin has a 10% tolerance.


### Regular Buck Converters
They offer high efficiency and a big dropout by switching the input signal on and off in order to have a pwm-ish output with lower RMS value, a passive LC filter on the other side and a diode arrange allows the switching output to make a waveform of small amplitude arround the nominal output.  

| Brand | Model | V_in range | V_out | Max Iout | Efficiency | Applications |
| ----- | ----- | ---------- | ----- | -------- | ---------- | ------------ |
| Tracopower | TSR1-2450 | 6.5-36V | 5V | 1A | ~93% | Maximizes efficiency compromising delivered power and noise inmunity. 
| TI | LM2596S-5.0 module | 6-40V | 5V | 3A | ~80% | DIY projects, poor regulation. There is an adjustable version. 
| Tracopower | TSR1-2433 | 4.75-36V | 3V3 | 1A | ~91% | Maximizes efficiency compromising delivered power and noise inmunity.
| TI | TPS54331 |  | 3V3 | 3A | ~92% | To go PCB high-current. Adjustable output. 
| TracoPower | TSR1-24120 | 15-36V | 12V | 1A | ~94% | Source periphericals at 12V from 24V rail
| Recom | R-78E12-0.5 | 7-28V | 12V | .5A | ~95% | low current option.

* __TracoPower TSRX-YYZZ__ : X is the output current, YY the nominal input Voltage and ZZ the nominal output voltage, there are also TSR1.5 on the market. Vout can be 1V2, 1V5, 1V8, 2V5, 3V3, 5V, 6V5, 9V, 12V, 15V.
* __Recom R-78EVout-0.5__ : Vout can be 3V3, 5V, 9V, 12V and 15V, max input is always 28V and at least a couple of V above the nominal output.

### LDO (Linear dropout voltage regulators)
They are ADC controlled, meaning that they will sink current to the ground in order to get the output voltage to match an internal reference. Some of them are adjustable. The efficiency of these components is proportional to the ratio Vout/Vin so the bigger the gap is, the lower the efficiency.
| Brand | Model | V_in range | V_out | Max Iout | Efficiency | Applications |
| ----- | ----- | ---------- | ----- | -------- | ---------- | ------------ |
| AMS1117-5.0 | 

### Resistor divider (DIY power division)
Basically it follows kirkchoff rule to divide a Vin into two dropouts, it may be usefull if you can take both signals or if there is no space to add another system, but it is highly inefficient and noise sensitive. Sometimes it is used for logic-level shifting instead of transistors array.

| V_in | V_ out | R_1 | R_2 | Efficiency | 
| ---- | ------ | --- | --- | ---------- |
| 24V  |   5V   |     |     |            |
| 12V  |   5V   |     |     |            |
|  5V  |   3V3  |     |     |            |


## Level Shifting 

### Resistor Divider

### Transistors arrange 

### Level Shifter Array 

## Digital Drivers 

### Darlington Transistors Array 

### DMos Array 

## LED Drivers 

## Communication protocol adapters : 

### UART to RS485
|      Item         | MAX485 | MAX3485 | SP3485 |
|||||

### UART to CAN

### I2C to Di2c 

||

## 8-bit ARV microcontrollers (for local processing)

## Other Parts 
* __NE555__ : This chip it's a timer, it allows to create PWM signals without software. 


