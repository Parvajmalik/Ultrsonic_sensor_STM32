# Ultrsonic sensor control using STM32 

A simple library for HC-SR04 ultrasonic sensor. It uses STM32 HAL library.
Copy the library header and source files to your project folder(Inc and Src folders).

## Usage

Configure STM32CubeMX to use GPIO pins for trigger pin, use TIM input capture mode for echo pin.

In this example, I used PD12 for trigger pin and TIM1 CH1(PD11) for echo pin.

Set timer prescaler to 83, use internal clock source.

Set channel 1 to input capture mode, set polarity to rising edge.

Enable interrupt in NVIC settings.

Include the header file in your main.h file.



