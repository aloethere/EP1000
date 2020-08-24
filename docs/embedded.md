---
layout: default
---

# Embedded Programming

## Introduction to Arduino
 Arduino Uno is an open-source microcontroller board based on the Microchip ATmega328P microcontroller. This microcontroller is a good choice as it helps a those getting started with electronics a basic understanding in embedded programming. It is also cheap and widely available. We can make devices work according to our needs and requirements by using this board.

### Using Arduino IDE
Step 1: Write Code
Step 2: Compile
Step 3: Upload to UNO board
Step 4: Observe result
* press reset button to refresh

### Interfacing LCD Panel using I2C
This task is using 16×2 LCD display with HD44780 controller.
Download [LiquidCrystal_PCF8574 Library](https://github.com/johnrickman/LiquidCrystal_I2C)

```
#include <Wire.h> // Library for I2C communication
#include <LiquidCrystal_I2C.h> // Library for LCD
// Wiring: SDA pin is connected to A4 and SCL pin to A5.
// Connect to LCD via I2C, default address 0x27 (A0-A2 not jumpered)
LiquidCrystal_I2C lcd = LiquidCrystal_I2C(0x27, 20, 4); // Change to (0x27,16,2) for 16x2 LCD.
void setup() {
  // Initiate the LCD:
  lcd.init();
  lcd.backlight();
}
void loop() {
  // Print 'Hello World!' on the first line of the LCD:
  lcd.setCursor(0, 0); // Set the cursor on the first column and first row.
  lcd.print("Hello World!"); // Print the string "Hello World!"
  lcd.setCursor(2, 1); //Set the cursor on the third column and the second row (counting starts at 0!).
  lcd.print("Welcome 2 Fablab");
}
```

![]()

### Simple LED control

- connect a LED with a current limiting resistor (220 ohm) to port 6 of the Arduino Uno board.
write a program to blink the LED in a variety of patterns.

![]()

```
const int RED=8;
void setup ()
{ 
  pinMode (RED, OUTPUT);
}

void loop()
{
  digitalWrite(RED, HIGH);
  delay(1000);
  digitalWrite(RED, LOW);
  delay(1000);
  
}
```
