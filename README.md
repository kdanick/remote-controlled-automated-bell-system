# SinricPro Automated School Bell System

This project demonstrates an advanced setup for using the SinricPro platform to control multiple switches and relays on an ESP module(**Disclaimer:** it's a continuation of the Automated-bell project I did using Arduino). Feel free to check it first out --> https://github.com/kdanick/Automated-bell

The system is designed to facilitate the creation of an automated school bell system, allowing for remote control of bells or any other electrical devices through the SinricPro mobile application.

## Features

- **Multiple Device Control**: The project supports up to N SinricPro Switch devices, enabling the management of multiple electrical devices simultaneously.
- **Manual Control**: In addition to remote control via the SinricPro mobile app, the system features manual control using tactile buttons or toggle switches. This allows for physical interaction with the connected devices, providing flexibility in controlling relays.
- **Integrated Logic**: The system uses a single callback to handle relay control, synchronizing remote and manual operations through one unified mechanism.
  
## How It Works

1. **Device Configuration**: The system uses a structured approach to configure each device, defining the device ID, relay pin, flip switch pin, and whether the device operates in "active low" mode.
2. **SinricPro Integration**: Each switch device is linked to a corresponding relay using the SinricPro library, allowing seamless communication between the ESP module and the SinricPro cloud platform. This enables remote control of devices via the SinricPro mobile app.
3. **Manual Control Handling**: The project incorporates logic to handle manual button presses or switch toggles. The state changes from these manual controls are synchronized with the SinricPro platform, ensuring consistency across all control methods.

## Getting Started

### Configuration

1. **Wi-Fi Credentials**: Set your Wi-Fi SSID and password in the `WIFI_SSID` and `WIFI_PASS` variables.
2. **SinricPro Credentials**: Obtain your `APP_KEY` and `APP_SECRET` from the [SinricPro website](https://sinric.pro/) and update the `APP_KEY` and `APP_SECRET` variables.
3. **Device Mapping**: Configure your devices in the `devices` map, specifying the device ID, relay pin, flip switch pin, and whether the device uses an active-low configuration.

### Dependencies

- [SinricPro ESP8266/ESP32 SDK](https://github.com/sinricpro/esp8266-esp32-sdk)
- Ensure you have the required libraries installed by following the [SinricPro Setup Documentation](https://github.com/sinricpro/esp8266-esp32-sdk/blob/master/README.md).

### Hardware Setup

1. **ESP Module**: Connect the ESP module to the appropriate relay and flip switch pins according to the configuration.
2. **Manual Button or Switch**: Connect a manual button or toggle switch to control the relay directly. Configure this in the code by setting the correct pin and using the `flipSwitchPIN`.

### Compile and Upload

1. Open the code in the Arduino IDE.
2. Compile the code and upload it to your ESP module.
3. Monitor the system via the serial monitor to check for connection status and device operations.

### Testing and Troubleshooting

1. Use the serial monitor to view system activity, including Wi-Fi connection status and relay control actions.
2. Test both remote control via the SinricPro mobile app and manual control through the connected buttons or switches.
3. If you encounter issues, check the SinricPro documentation and open an issue on the [SinricPro GitHub repository](https://github.com/sinricpro/esp8266-esp32-sdk/issues).

## Project Origins

This project was created to build an automated bell system for schools, allowing for remote control and manual operation of bells and other electrical devices. By leveraging the SinricPro platform, the system provides a reliable and flexible solution for controlling devices both remotely and manually.

## Resources

- [SinricPro ESP8266/ESP32 SDK Documentation](https://sinricpro.github.io/esp8266-esp32-sdk)
- [SinricPro GitHub Repository](https://github.com/sinricpro/esp8266-esp32-sdk)

## License

This project is open-source. Feel free to modify and use it for your own projects!

---

### Created by [Kirenga Danick](https://github.com/kdanick)
