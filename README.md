# NodeMCU Security System with Telegram App Integration

This project demonstrates the implementation of a security system using NodeMCU ESP8266 board and the Telegram app. The system utilizes a PIR (Passive Infrared) motion sensor to detect movement and sends real-time notifications to the user's Telegram account, allowing them to monitor and secure their premises remotely.


## How does the PIR security system work?

When powering this system, First, the Nodemcu board connects to the Internet connection via the local IP address. Then, the system goes into activation mode. After, displayed as “System startup” on the LCD and Telegram app. Next, when a movement occurs, it is captured by the PIR sensor and sent to the Arduino board. Then, the buzzer will activate for a short time. Also, displayed as “Motion detected” in the Telegram app and on the LCD. Then, the system returns to a normal situation. That is, displayed as “No motion” on the LCD.

## Features

- Motion detection using a PIR motion sensor
- Integration with the Telegram app for receiving notifications
- Real-time alerts sent to the user's Telegram account
- Easy setup and customization

## Prerequisites

To set up the NodeMCU security system, you will need the following:

- NodeMCU ESP8266 board
- PIR motion sensor
- Buzzer
- LCD display 
- USB cable for connecting NodeMCU to your computer
- Arduino IDE (Integrated Development Environment)
- Telegram account and the Telegram app installed on your smartphone


## Part's List (Amazon)
==========================================
1.Nodemcu board x 1 -- https://amzn.to/3P2fzr9

2.PIR sensor x 1 --  https://amzn.to/3oVKgU8

3.Jumper wires. -- https://amzn.to/3P1ja8N

4.Breadboard x 1 ---  https://amzn.to/3J2EDKZ

5.LCD display x 1 --  https://amzn.to/3Cooj37

8.Buzzer x 1 --   https://amzn.to/3IXQM3t




## Getting Started

1. Connect the NodeMCU board to your computer using the USB cable.

2. Open the Arduino IDE and install the required libraries for NodeMCU and Telegram integration. You can use the Arduino Library Manager to install the libraries easily.

3. Create a new Arduino sketch and copy the code provided in the <A href="https://github.com/LgcyAlex/ESP8266-security_system/blob/a280195cba1e08d422d9f9473d2523977dc9d405/PIR_security/PIR_security.ino">`PIR_security.ino`</a> file from this repository.

4. Update the Wi-Fi credentials in the code with your network's <A href="https://github.com/LgcyAlex/ESP8266-security_system/blob/e06328504721bd479e5acb2b96674c7bd2fc91b3/PIR_security/PIR_security.ino#L9">SSID (name)</a> and <A href="https://github.com/LgcyAlex/ESP8266-security_system/blob/e06328504721bd479e5acb2b96674c7bd2fc91b3/PIR_security/PIR_security.ino#LL10C1-L10C1"> WiFi Password</a>.

5. Obtain your Telegram Bot Token:
   - Open the Telegram app and search for the <A href="https://telegram.me/BotFather">"BotFather"</a> bot.
   - Create a new bot and obtain the Bot Token.

6. Replace the <A href="https://github.com/LgcyAlex/ESP8266-security_system/blob/f9e9537eecd0c34af6353cfbab3d47520ab83d10/PIR_security/PIR_security.ino#L13">TELEGRAM_BOT_TOKEN</a> placeholder in the code with your Bot Token.

7. Obtain your Telegram CHAT ID:
   - Open the Telegram app and search for the <A href="https://telegram.me/MissRose_bot">"Rose"</a> bot.
   - Press START and send ```/id``` you will get your CHAT_ID.

8. Replace the <A href="https://github.com/LgcyAlex/ESP8266-security_system/blob/f9e9537eecd0c34af6353cfbab3d47520ab83d10/PIR_security/PIR_security.ino#LL14C2-L14C2">CHAT_ID</a> placeholder in the code with your CHAT ID.

9. Upload the code to the NodeMCU board by clicking on the "Upload" button in the Arduino IDE.

10. Once the upload is complete, disconnect the NodeMCU from your computer and connect it to a power source.

11. Connect all the components as shown in the <A href="https://github.com/LgcyAlex/ESP8266-security_system/blob/f9e9537eecd0c34af6353cfbab3d47520ab83d10/circuit%20diagram.png">DIAGRAM</a>.

12. Mount the PIR motion sensor in the desired location, adjusting the sensitivity and range according to your requirements.

13. Boom! Your security system is now ready to use. When the motion sensor detects movement, it will send a notification to your Telegram account.

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
- [Telegram Bot API](https://core.telegram.org/bots/api)
- [PIR Motion Sensor Tutorial](https://www.instructables.com/PIR-Motion-Sensor-Tutorial/)
- [Arduino IDE](https://www.arduino.cc/en/software)

Feel free to contribute to this project by submitting bug reports, feature requests, or pull requests. Happy coding!
