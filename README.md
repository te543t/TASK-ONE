# Smart LED Control with Arduino UNO

## Objective
This project demonstrates the basic concept of digital output control using an Arduino UNO to power an LED. It serves as an introductory hands-on experiment for understanding microcontroller-based circuit design and logic control in embedded systems.

## Technical Overview
The circuit connects a red LED to digital pin 13 on the Arduino UNO, with a 220Ω resistor in series to limit current. The Arduino sends a HIGH signal to turn the LED on and a LOW signal to turn it off, controlled through a simple loop in the Arduino sketch. This project illustrates the basics of digital I/O, timing, and hardware interfacing.

##  Circuit Diagram
![LED Arduino Circuit](./TASK%20ONE.png)

> Make sure the image file is named `TASK ONE.png` and stored in the same directory as this README.

##  Tinkercad Project Link  
[Click here to open the Tinkercad project](https://www.tinkercad.com/things/6YT27eC7O6P-funky-bigery-waasa/editel)

---

## Components
- Arduino UNO board  
- Red LED  
- 220Ω resistor (±5%)  
- Breadboard  
- Jumper wires  
- USB cable (for power and programming)

---

## System Behavior
The LED blinks every second based on a timed control loop. The sketch uses `pinMode()` to configure the pin and `digitalWrite()` for output, combined with `delay()` for timing.

---

##  Arduino Code

```cpp
void setup() {
  pinMode(13, OUTPUT); // Set digital pin 13 as output
}

void loop() {
  digitalWrite(13, HIGH); // Turn LED ON
  delay(1000);            // Wait 1 second
  digitalWrite(13, LOW);  // Turn LED OFF
  delay(1000);            // Wait 1 second
}
