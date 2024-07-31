In this project we make a robotic arm with 5 degrees of freedom based on inverse kinematics.
The first thing that comes to mind are the brilliant yellow KUKA BOT arms we see in industrial usage. We draw inspiration from this bot. Self explanatory that our project can also be modified for the same purpose if replaced with heavy motors and subsequent tuning in the code.
Parts used in the project:

NodeMCU-32ES-ESP32 Development board(x1)
![image](https://github.com/user-attachments/assets/5e364cc0-92a3-4b38-b957-13d8ae7f0497)



PCA9685- 16 channel 12-Bit PWM Servo Motor Driver I2C Module ( Compatible with esp32 as slave)(x1)
![download (1)](https://github.com/user-attachments/assets/4f118e1b-9ed8-469f-a4d6-144965aedc60)


MG995 Servo motor (x3)
![image](https://github.com/user-attachments/assets/6d042a5f-e01e-4565-918e-3c97fefef57b)


Jumper Wires
![image](https://github.com/user-attachments/assets/62165969-d499-4239-8e9b-9dee2438bdd4)


6V 2A Power Supply


We are using the NodeMCU-32ES-ESP32 Development board as the thinker board for thus project.

MG995 Servo motor (x3) are used for the rotation of the arm.

PCA9685- 16 channel 12-Bit PWM Servo Motor Driver I2C Module ( Compatible with esp32 as slave)(x1) to be able to control all the servos simultaneously. We have been able to achieve 180 degrees of  base rotation and 3DOF using the above configuration.
We use the standard adruino ide to write, edit and test the code.

The code has been mentioned in the code file of the repository which calculates the joints angles required to reach the given coordinates using Inverse Kinematics.

We use blynk iot cloud for the slider controls to enter the coordinates for controlling the movements of the BOT.

We input the coordinates we need the arm to be at , the thinker board then calculates the joint angles required and the servos work to reach the desired coordinate.


