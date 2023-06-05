# NodeMCU Security System with Telegram App Integration

This project demonstrates the implementation of a security system using NodeMCU ESP8266 board and the Telegram app. The system utilizes a PIR (Passive Infrared) motion sensor to detect movement and sends real-time notifications to the user's Telegram account, allowing them to monitor and secure their premises remotely.

## Features

- Motion detection using a PIR motion sensor
- Integration with the Telegram app for receiving notifications
- Real-time alerts sent to the user's Telegram account
- Remote monitoring and control of the security system
- Easy setup and customization

## Prerequisites

To set up the NodeMCU security system, you will need the following:

- NodeMCU ESP8266 board
- PIR motion sensor
- USB cable for connecting NodeMCU to your computer
- Arduino IDE (Integrated Development Environment)
- Telegram account and the Telegram app installed on your smartphone

## Getting Started

1. Connect the NodeMCU board to your computer using the USB cable.

2. Open the Arduino IDE and install the required libraries for NodeMCU and Telegram integration. You can use the Arduino Library Manager to install the libraries easily.

3. Create a new Arduino sketch and copy the code provided in the `security_system.ino` file from this repository.

4. Update the Wi-Fi credentials in the code with your network's SSID (name) and password.

5. Obtain your Telegram Bot Token:
   - Open the Telegram app and search for the "BotFather" bot.
   - Create a new bot and obtain the Bot Token.

6. Replace the `TELEGRAM_BOT_TOKEN` placeholder in the code with your Bot Token.

7. Upload the code to the NodeMCU board by clicking on the "Upload" button in the Arduino IDE.

8. Once the upload is complete, disconnect the NodeMCU from your computer and connect it to a power source.

9. Mount the PIR motion sensor in the desired location, adjusting the sensitivity and range according to your requirements.

10. Install and open the Telegram app on your smartphone.

11. Search for the "BotFather" bot and start a chat.

12. Send the command `/mybots` to see your bot.

13. Start a chat with your bot by clicking on the "Start" button or sending a message.

14. Your security system is now ready to use. When the motion sensor detects movement, it will send a notification to your Telegram account.

## Customization

You can customize the security system according to your specific needs:

- Modify the sensitivity of the PIR motion sensor in the code by adjusting the delay and threshold values.
- Add additional features such as a sound alarm, LED indicators, or a camera module for capturing images or videos upon detection.
- Enhance the notification system by adding more functionalities or integrating with other messaging platforms.

## Troubleshooting

If you encounter any issues during the setup or usage of the security system, consider the following:

- Double-check your Wi-Fi credentials and ensure that your NodeMCU is connected to the correct network.
- Verify that the PIR motion sensor is correctly wired to the NodeMCU board.
- Make sure the Telegram Bot Token is correctly entered in the code without any typos.
- Check the serial monitor in the Arduino IDE for any error messages or debugging information.

## License

This project is licensed under the [MIT License](LICENSE), allowing you to modify and distribute the code according to your requirements.

## Acknowledgments

- The NodeMCU community for their contributions and support.
- The Telegram API developers for providing the platform for app integration.

## Further Reading

- [NodeMCU Documentation](https://nodemcu.readthedocs.io/)
- [Telegram Bot

 API](https://core.telegram.org/bots/api)
- [PIR Motion Sensor Tutorial](https://www.instructables.com/PIR-Motion-Sensor-Tutorial/)
- [Arduino IDE](https://www.arduino.cc/en/software)

Feel free to contribute to this project by submitting bug reports, feature requests, or pull requests. Happy coding!
