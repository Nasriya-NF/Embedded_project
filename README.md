# Embedded_project
Title: Intelligent Weight-Carrying Automation System.
Team members:
1.	NASRIYA N.F. – 2021/E/105
2.	JENCILY S. – 2021/E/140
3.	HAMSANA S. – 2021/E/152
4.	GUNASEKARA W.M.P.  – 2021/E/172

2.	PROBLEM AND SOLUTION
Introduction
Modern logistics and personal transport solutions demand automated systems capable of optimizing time and energy. This project focuses on developing an autonomous weight-carrying device integrated with a mobile application. The app enables user login and device tracking through location services. The device will be equipped with a flexible mapping system to calculate the shortest and obstacle-free path to a specified destination. This innovation aims to enhance efficiency in transport and handling of loads up to 10 kg, particularly in environments where manual handling is challenging.

Problem:
In stores, warehouses, libraries or supermarkets, employees and customers often need to carry weights manually to different locations. This is both time-consuming and physically demanding. Manual handling may also lead to inefficiency and errors in task completion.

Solution:
The Weight Carrying Automated Roller is a compact with path adaptability, by using embedded system and design knowledge, Desigen an IoT-enabled device to follow user commands and transport weights up to 10 kg. 
3.	NOVELTY
The project stands out due to its combination of location-based pathfinding, obstacle avoidance, and user-following capabilities in a compact, cost-effective design. Unlike other existing rollers, this device integrates real-time obstacle detection and path optimization for smoother operations in busy environments.
4.	 HIGH-LEVEL ARCHITECTURE
Technologies Used:
•	Microcontroller: ESP32 for IoT capabilities and control.
•	Sensors:
 Ultrasonic sensors for obstacle detection and avoidance.
 GPS Module (e.g., NEO-6M) to determine the device's real-time location.
 Inertial Measurement Unit (IMU) (e.g., MPU6050) for stability and orientation tracking.
 IR Sensors to detect edges or cliffs.
 Weight Sensor to measure the load being carried.



•	Communication Modules: Wi-Fi Module for app-based commands and updates.
•	Motor Drivers: For controlling roller movement.
•	Communication Protocols: Wi-Fi or Bluetooth for connectivity.
•	Power Source: Rechargeable Li-ion battery.
High-Level Workflow:
•	User Login: The user logs into the device via a mobile application or interface. Once logged in, the device becomes ready to execute instructions.
•	Location Input: The user provides the destination location through the application. The device calculates the shortest path to the endpoint.
•	Path Adaptability: The device moves towards the endpoint while continuously monitoring for obstacles. If the device detects obstacles or disturbances along the way, it dynamically recalculates and adapts its path to reach the destination.
•	Follow-Mode Capability: The roller can also follow the user within a specified range when commanded.

5.	CIRCUIT DESIGN AND PROTOCOLS
Components:
•	Microcontroller: ESP32 for IoT capabilities and control.
•	Sensors:
 Ultrasonic sensors for obstacle detection and avoidance.
 GPS Module (e.g., NEO-6M) to determine the device's real-time location.
 Inertial Measurement Unit (IMU) (e.g., MPU6050) for stability and orientation tracking.
 IR Sensors to detect edges or cliffs.
 Weight Sensor to measure the load being carried.
•	Communication Modules: Wi-Fi Module for app-based commands and updates.
•	Motor Drivers: For controlling roller movement.
•	Communication Protocols: Wi-Fi or Bluetooth for connectivity.
•	Power Source: Rechargeable Li-ion battery.
Basic Connections:
•	All sensors and modules are interfaced with GPIO, I2C, or UART pins of the microcontroller.
•	The GPS module and Bluetooth module are connected via UART for location tracking and user communication respectively.
•	The motor driver connects to the GPIO pins for directional control and to the motors for movement.
•	The ultrasonic sensors are distributed around the chassis and connected to GPIO pins for obstacle detection.
•	The load sensor is connected to the I2C interface for weight measurement.
•	A voltage regulator distributes stable power from the Li-ion batteries to the components.
•	The ESP32 handles data processing, communication, and decision-making.


Protocols
Communication Protocols
1.	MQTT (Message Queuing Telemetry Transport):
For sending commands and receiving updates between the app and the device.
2.	HTTP/REST API:
For communication between the mobile app and the backend server.
3.	I2C and SPI:
For communication between sensors and the microcontroller.
Navigation Protocol
1.	NMEA (National Marine Electronics Association):
Used by GPS modules for sharing location data.
2.	Obstacle Avoidance Protocol
Custom algorithm based on real-time sensor data (e.g., a combination of ultrasonic sensors and IMU data)

Component/Protocol	    Quantity	Total Price
Microcontroller (ESP32)	1	        1200
GPS Module            	1	        1800
Ultrasonic Sensors	    2	        1000
Motor Driver (L298N)	  1	        1000
DC motors	              4	        2800
Wheels                  4	        2000
Li-ion Batteries	      2	        1400
Chassis for Robot     	1	        1500
Load Sensor	            1	        1500
Bluetooth/ Wi-Fi Module	1	        1200
Additional	-	3000
Total 	18400


TASK	                                                             DURATION	                          DEADLINE
Information gathering, research and analysis on the topic.         2 weeks	                          10 FEB 2025
Finalizing the plan.	

Hardware collection/ purchase 	                                   4 days                             15 FEB 2025

Circuit design and testing.	                                       4 weeks	                          10 MAR 2025

Software development. (Eg-UI/UX)	                                 5 weeks	                          25 MAR 2025
Testing 

calibration & correcting	                                         1 week	                            10 APR 2025

Final documentation.	                                             2 days                           	12 APR 2025.
