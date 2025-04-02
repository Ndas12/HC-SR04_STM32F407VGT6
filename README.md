# STM32F407VGT6 with HC-SR04 Ultrasonic Sensor

This project demonstrates how to interface an STM32F407VGT6 microcontroller with an HC-SR04 ultrasonic distance sensor. The sensor is used to measure distance by emitting a sound pulse and timing how long it takes for the echo to return. This example uses PC4 for the Trigger pin and PC5 for the Echo pin to interact with the HC-SR04 sensor.

# Features:

**Distance Measurement:**

PC4 (configured as an output) is connected to the Trig pin of the HC-SR04 sensor.

PC5 (configured as an input) is connected to the Echo pin of the HC-SR04 sensor.

The STM32F407VGT6 generates a trigger pulse on PC4 to initiate the ultrasonic burst and then measures the time it takes for the Echo signal on PC5 to return.

**Distance Calculation:**

Based on the time taken for the echo to return, the code calculates the distance to the object.

The formula used is:
Distance (cm) = (Time * Speed of Sound) / 2

The speed of sound is approximately 343 meters per second (or 0.0343 cm/μs).

# Pin Connections:

**STM32F407VGT6 Pins:**

PC4 → Trig (HC-SR04)

PC5 → Echo (HC-SR04)

**HC-SR04 Ultrasonic Sensor Pins:**

Trig → PC4 (STM32F407VGT6)

Echo → PC5 (STM32F407VGT6)

VCC → 5V Power Supply

GND → Ground
