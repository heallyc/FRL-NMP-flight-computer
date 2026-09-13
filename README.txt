README
Heally Cruz 10/31/2025
apparently i was supposed to do a 1x4 header for the sensors but then i wouldn't have an AD0 or SDO to attach to ground, so i just used the given components for the MPU6050 and BMP280 in kicad.

pin map
3V3 -> 3V3 pin
5V_USB -> +5V pin
GND -> GND pin
SDA (MPU6050) -> A4
SDI (BMP280) -> A4
SCK (BMP280) -> A5
SCL (MPU6050) -> A5
Servo signal D9 -> PWM_A (D9)
Servo signal D10 -> PWM_B (D10)
TP1(3V3) -> 3V3
TP2(GND) -> GND
TP3(SERVO_5V1) -> SERVO_5V
TP4(SDA1) -> SDA net
TP5(SCL1) -> SCL net
TP6(5V_USB1) -> +5V pin

power domains
5V_USB = 5V from Arduino Nano USB
SERVO_5V = 5V from external source attached to screw terminal
3V3 = 3.3V from Arduino Nano 
all grounds are common

i2c addresses used 
MPU6050 - AD0 (GND) : 0x68 
BMP280 - SDO (GND) : 0x76

servo header pinout
GND (pin 6)         | GND (pin 5)
SERVO_5V (pin 4)    | SERVO_5V (pin 3)
PWM_B (D10) (pin 2) | PWM_A (D9) (pin 1)

