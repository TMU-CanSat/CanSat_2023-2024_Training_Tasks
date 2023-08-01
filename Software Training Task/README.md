# Software Training Task

## Task Description
The task is to collect data from various sensors, package it into a string, then save it to an SD card and transmit it to the host computer. Also if certain conditions are met perform an action. Use Wokwi to simulate your code and test it. https://wokwi.com/
  
1. Initialize the servo motor at 0 degrees.
2. Write code to read data from all the sensors listed in [Devices].
3. Collect the following data points:
	- Temperature
	- Distance (HC-SR04)
	- Acceleration (X, Y, Z) in m^s2
	- Rotation Rate (X, Y, Z) in rad/s
	- Count (How many transmissions have been made. This should increment by 1 every time a new transmission is sent. Starts at 0.)
4. Create a string with the following format:
	COUNT_TEMPERATURE_DISTANCE_ACCELERATIONX_ACCELERATIONY_ACCELERATIONZ_ROTATIONX_ROTATIONY_ROTATIONZ
5. Store the string on the SD Card in a file type of your choice. Each new transmission should be saved on a new line so that all data is logged.
6. Transmit the string via Serial to the host computer at a baudrate of 115200.
7. Repeat steps 2-5 at a rate of 1 Hz until Count reaches 100.
8. If the Temperature reaches above 35 degrees or is equal to 35 degrees rotate the servo motor 90 degrees.
9. If the Temperature drops below 35 degrees return the servo motor to 0 degrees.

## Notes
You can use any pins on the Arduino to connect the devices. As long as they work of course.

## Devices
- Arduino Mega
- Micro SD Card Module (SPI)
- HC-SR04 Ultrasonic Distance Sensor
- DS18B20 Temperature Sensor
- MPU6050 6-Axis Accelerometer & Gyroscope Sensor
- Servo motor

## Submission
Submit the link to your public Wokwi project in the submission form below.  
https://forms.gle/odUKQcjkpXAaYcKf6