 CODETECH-TASK-2
To interface a DHT sensor with an Arduino for measuring temperature and humidity and display the readings on an LCD screen or serial monitor, follow these steps:

 Introduction

A DHT sensor (such as the DHT11 or DHT22) is a commonly used sensor for measuring temperature and humidity. These sensors provide digital output and are easy to interface with microcontrollers like the Arduino. This project involves reading temperature and humidity data from a DHT sensor and displaying the information either on an LCD screen or through the serial monitor of the Arduino IDE.

 Materials Needed

- Arduino board (e.g., Uno)
- DHT sensor (DHT11 or DHT22)
- 16x2 LCD screen (optional, if not using the serial monitor)
- Resistor (10kΩ, if needed for the LCD contrast adjustment)
- Breadboard and jumper wires

 Steps to Interface the DHT Sensor with Arduino

1. *Wiring the DHT Sensor*:
    - Connect the VCC pin of the DHT sensor to the 5V pin on the Arduino.
    - Connect the GND pin of the DHT sensor to the GND pin on the Arduino.
    - Connect the Data pin of the DHT sensor to a digital I/O pin on the Arduino (e.g., pin 2).

2. *Connecting the LCD Screen (Optional)*:
    - Connect the VCC and GND pins of the LCD to the 5V and GND pins on the Arduino.
    - Connect the RS, E, D4, D5, D6, and D7 pins of the LCD to the digital I/O pins on the Arduino (e.g., pins 7, 8, 9, 10, 11, and 12 respectively).
    - Adjust the contrast using a potentiometer connected to the V0 pin of the LCD.

3. *Installing the Libraries*:
    - In the Arduino IDE, go to Sketch -> Include Library -> Manage Libraries.
    - Search for and install the "DHT sensor library" by Adafruit.
    - If using an LCD screen, install the "LiquidCrystal" library.

4. *Arduino Code*:
    - Below is a sample code to read from the DHT sensor and display the readings on the serial monitor or an LCD screw.
