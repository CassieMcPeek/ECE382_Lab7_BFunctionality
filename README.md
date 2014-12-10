ECE382_Lab7_BFunctionality
==========================

# Purpose

The purpose of the library is to create an interface with the three IR sensors on the robot by utilizing ATD.

# Description

The three IR sensors on the robot all return a voltage value between 0 V and 5 V. The value returned is based on the distance from the object to the sensor. The closer the object, the higher the voltage value returned will be. Each IR sensor has a seperate function, declared in the header file, defined in the B_Funct.c file and then utilized in the main2.c file.

# Functions

the three functions are:
      leftSensor()
      rightSensor()
      centerSensor()
      

The left sensor function utilizes the left IR sensor to detect objects on the left side of the robot. The right sensor detects objects on the right side, and the center sensor detects objects in front of the robot. Each IR sensor has a different threshold of where it will detect an object. Therefore, the value that is compared to ADC10MEM in the main2.c file is different for each sensor. Altering this value will alter the distance that the sensor will detect an object. 

The left and center sensors light LED 1 on the MSP430, and the right sensor lights LED 2 on the MSP430. 
