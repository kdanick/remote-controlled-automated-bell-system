# Automated-bell with mobile app
A school based automated bell system

SinricPro Automated School Bell System
This project demonstrates an advanced setup for using the SinricPro platform to control multiple switches and relays on an ESP module. The system is designed to facilitate the creation of an automated school bell system, allowing for remote control of bells or any other electrical devices through the SinricPro mobile application.

Features
Multiple Device Control: The project allows for the setup of multiple SinricPro switch devices to control corresponding relays, enabling the management of various electrical components simultaneously.

Manual Control: In addition to remote control via the SinricPro mobile app, the system incorporates manual control through tactile buttons or toggle switches. These manual controls are seamlessly integrated with the SinricPro platform, ensuring synchronization between manual and remote operations.

How It Works
Device Configuration: The system utilizes a structured configuration approach, defining each device's unique identifier, relay pin, flip switch pin, and active low settings. This configuration enables straightforward setup and management of multiple devices within a single ESP module.

SinricPro Integration: Through the SinricPro library, each switch device is linked to its corresponding relay, facilitating seamless communication between the ESP module and the SinricPro cloud platform. This integration enables remote control of devices via the SinricPro mobile app.

Manual Control Handling: The project incorporates logic to handle manual button presses, allowing users to interact directly with connected devices. These manual interactions are detected, processed, and synchronized with the SinricPro platform, ensuring consistent device state across all control methods.

Getting Started
To utilize this project effectively, follow these steps:

Configuration: Define the necessary parameters such as Wi-Fi credentials, SinricPro application key, and secret. Additionally, configure the device mappings in the devices map according to your specific setup.

Dependencies: Ensure all required libraries are installed, as outlined in the SinricPro ESP8266/ESP32 SDK documentation.

Hardware Setup: Connect the ESP module to the relevant relays and flip switches based on the configured pin mappings.

Compile and Upload: Compile the code and upload it to your ESP module using the Arduino IDE or platform of your choice.

Testing and Troubleshooting: Monitor the system via the serial monitor and test both remote and manual control functionalities. Refer to the provided resources for troubleshooting guidance and additional documentation.

Project Origins
This project originated from the need to create an automated school bell system, leveraging the versatility and accessibility of the SinricPro platform. By integrating remote and manual control capabilities, the system offers a comprehensive solution for managing electrical devices in educational environments and beyond.

For further information, refer to the full user documentation and the SinricPro ESP8266/ESP32 SDK GitHub repository.

If you encounter any issues or have suggestions for improvement, please visit the project repository to contribute or seek assistance from the community.
