# Sensors

## Acceleration and Gyroscopy
### Digital Sensors
* __MPU6050__ -> beginner friendly. 
* __BMI270__ -> Robot Stability/self balancing. Low Power consumption, high noise filtering; stable angle, fast fusion. 
* __BNO085__ -> Dronves, AR/VR and orientation tracking. Built-in fusion; built-in kalman, outputs rotation directly, less coding. 
* __ICM-20948__ -> Navigation and autonomou robots. Built-in fusion; built-

| Features |MPU6050|BMI270|BNO085|ICM20948|
| -------- |-------|------|------|--------|
| Axis |6-axis|6-axis|9-axis|9-axis|
| Acc Range |+/-2 to 16g|+/-2 to 16g|+/-2 to 16g|+/-2 to 16g|
| Gyro Range |+/-250 to 2000 dps|+/-125 to 2000 dps|+/-125 to 2000 dps | +/-250 to 2000 dps |
| Magnometer | No | No | Yes | Yes |
| Sensor Fusion | No | No | Yes | No |
| Interface | I2C | I2C/SPI | I2C/SPI/UART | I2C/SPI |
| Op. Voltage | 3V3-5V | 1V7-3V6 | 1V7-3V6 | 1V8-3V3 |
| Power Cons. | 3.9mA | 0.7mA | 1.2mA | 3.3mA |
| Best for | Basic Projects | Self Balance | Drones, Motion Tracking | GPS Navigation, Accuracy |


## Temperature Sensors
### Digital Sensors

## Spectometers 

## Proximity : 
* __SR04__ : 
* __VL53LOX__ -> IR based, smaller, can calculate distance.