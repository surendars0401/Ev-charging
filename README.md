# Ev-charging
ESP32 I2C LCD Display with IR Sensor

Overview:
This project demonstrates how to use an ESP32 microcontroller to interface with an I2C 16x2 LCD display and an IR sensor. The program reads the state of the IR sensor and displays "charging" or "idle" on the LCD based on the presence of detected objects.

Requirements:
- ESP32 microcontroller
- I2C 16x2 LCD display module
- IR sensor
- Arduino IDE with ESP32 board support package installed

Circuit Diagram:
Please refer to the following circuit diagram for the wiring connections:

    ESP32                LCD Module
    --------------------------------
    SDA (GPIOxx) <----> SDA
    SCL (GPIOxx) <----> SCL
    3.3V        <----> VCC
    GND         <----> GND

Connect the IR sensor to the appropriate GPIO pin as specified in the code.

Installation:

1. Open the Arduino IDE.
2. Install the "LiquidCrystal_I2C" library by going to "Sketch" -> "Include Library" -> "Manage Libraries". Search for "LiquidCrystal_I2C" and click "Install" to install the library.
3. Connect your ESP32 board to your computer.
4. Open the "esp32_i2c_lcd_ir.ino" file in the Arduino IDE.
5. Select the appropriate board and COM port under the "Tools" menu.
6. Click on the "Upload" button to compile and upload the code to the ESP32.

Usage:
1. Upload the code to the ESP32 board as described in the Installation section.
2. Make sure the circuit connections are properly established.
3. Power on the ESP32.
4. The LCD will display "Idle" if no objects are detected by the IR sensor. It will display "Charging" if objects are detected.

Note:
- Modify the GPIO pin number in the code if you have connected the IR sensor to a different pin.
- Adjust the delay in the code (in milliseconds) to change the refresh rate of the sensor readings and LCD updates.

