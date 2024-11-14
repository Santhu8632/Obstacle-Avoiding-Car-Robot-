# Obstacle-Avoiding-Car-Robot-
Obstacle Avoiding Car Robot  using arduino uno 
which is designed for an autonomous obstacle-avoiding robot with a servo-mounted ultrasonic sensor, controlled using an Arduino with an Adafruit Motor Shield.

### Components Needed:
1. **Arduino Uno** (or compatible board)
2. **Adafruit Motor Shield** (to control motors)
3. **DC Motors** - 4
4. **Ultrasonic Sensor (HC-SR04)** (for distance measurement)
5. **Servo Motor** (to rotate the ultrasonic sensor)
6. **Jumper Wires**
7. **Battery Pack** (suitable for motors, e.g., 6V-12V depending on motor specifications)

### Circuit Connections:
1. **Motor Connections**:  
   - Attach the 4 DC motors to the motor terminals on the **Adafruit Motor Shield**:
     - Motor 1 to M1
     - Motor 2 to M2
     - Motor 3 to M3
     - Motor 4 to M4

2. **Ultrasonic Sensor**:
   - Connect the **TRIG_PIN** (`A0`) on the Arduino to the Trig pin of the HC-SR04.
   - Connect the **ECHO_PIN** (`A1`) on the Arduino to the Echo pin of the HC-SR04.
   - Connect **VCC** of the HC-SR04 to the 5V pin on the Arduino.
   - Connect **GND** of the HC-SR04 to the GND pin on the Arduino.

3. **Servo Motor**:
   - Connect the **signal pin** of the servo to **pin 10** on the Arduino (as specified in your code).
   - Connect the **power** and **ground** pins of the servo to 5V and GND on the Arduino.

4. **Power Supply**:
   - Power the **Adafruit Motor Shield** through its external power terminals (using a separate battery pack, e.g., 6-12V, depending on motor specifications).
   - Connect the **Arduino** to either USB or a separate power source (do not power the motors through the Arduino).

### Additional Notes:
- Ensure all **GND** connections are common to maintain a stable reference point.
- Double-check that the **DC motors** and **servo** are compatible with the power source being used to avoid overloading the Arduino or motor shield.
- The code handles forward, backward, left, and right movements based on the distance measured by the ultrasonic sensor.

After setting up the circuit as described, upload the code to the Arduino.
