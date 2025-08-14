This project is an Jeevani that uses NodeMCU (ESP8266) for
sensor readings and ESP32-S with OV2640 camera module for live streaming. It includes: - Load
Cell + HX711 for saline volume measurement. - IR Flow Sensor for drip rate monitoring. - Servo
motor for flow control. - Buzzer & LEDs for alerts. - SIM800L for SMS notifications. - ESP32-S +
OV2640 for live camera feed. - Supabase for web dashboard integration. - Battery backup system
for uninterrupted operation. The system alerts the nurse when the saline level is low or the flow
stops, and also allows remote flow control via a web dashboard.

Hardware Components: 1. NodeMCU ESP8266 2. ESP32-S Board 3. OV2640 Camera Module 4.
HX711 Load Cell Sensor 5. IR Flow Sensor 6. Servo Motor (SG90 or MG995) 7. Buzzer 8. LEDs
(Red, Green, Yellow) 9. SIM800L GSM Module 10. 16x2 I2C LCD Display 11. Power Supply (5V
Adapter / Battery Backup) 12. Breadboard & Jumper Wires

Setup Instructions: 1. Connect Load Cell to HX711 and to NodeMCU. 2. Connect IR Flow Sensor to
NodeMCU digital pin. 3. Connect Servo Motor to NodeMCU PWM pin. 4. Connect Buzzer & LEDs
to digital pins. 5. Connect SIM800L to NodeMCU UART pins. 6. Connect LCD via I2C to NodeMCU.
7. Connect OV2640 camera module to ESP32-S. 8. Flash NodeMCU.ino to ESP8266 for sensor
control & alerts. 9. Flash ESP32_Camera.ino to ESP32-S for live streaming. 10. Power system via
5V adapter or battery backup.

Battery Backup System: - Use a 12V battery connected to a relay-based inverter circuit. - Step
down voltage to 5V using a buck converter for NodeMCU, ESP32-S, and SIM800L. - Relay will
switch automatically to battery in case of power failure.
