# Software Training Task

## Task Description
1. Write code to read data from all the sensors listed in [Devices]
2. Collect the following data points:
	- Temperature
	- Distance (HC-SR04)
	- Acceleration (X, Y, Z) in m^s2
	- Rotation Rate (X, Y, Z) in rad/s
	- Count (How many transmissions have been made. This should increment by 1 every time a new transmission is sent. Starts at 0.)
3. Create a string with the following format:
	COUNT_TEMPERATURE_DISTANCE_ACCELERATIONX_ACCELERATIONY_ACCELERATIONZ_ROTATIONX_ROTATIONY_ROTATIONZ
4. Store the string on the SD Card in a file type of your choice. Each new transmission should be saved on a new line so that all data is logged.
5. Transmit the string via Serial to the host computer at a baudrate of 115200.
6. Repeat steps 2-5 at a rate of 1 Hz until Count reaches 100.


## Devices
- Arduino Mega
- Micro SD Card Module (SPI)
- HC-SR04 Ultrasonic Distance Sensor
- DS18B20 Temperature Sensor
- MPU6050 6-Axis Accelerometer & Gyroscope Sensor