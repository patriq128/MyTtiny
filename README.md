# MyTtiny

My own development board based on the **ATtiny3217** microcontroller.

<img src="assets/main.png" alt="MyTtiny development board" width="500"/>

## Features

One of the biggest features of this board is that it was originally designed for my own projects. However, I also wanted to make it useful enough for other people to use.

- **Compact size**

  I tried to make this board as small as possible, and I think I did a pretty good job. The board measures only **29.718 × 17.018 mm**.

- **USB-C**

  USB-C makes the board easier to use for programming and communication. I also included the required configuration resistors, so **USB-C to USB-C cables work properly**.

- **UART**

  I decided to add a **CH340N** USB-to-UART chip. This allows you to upload programs and communicate with the board through a serial monitor.

- **NeoPixel LED**

  I wanted the board to provide visual feedback even without any external hardware, so I added a programmable RGB LED.

- **Pins**

  Every header pin is labeled on both the top and bottom sides of the PCB.

## Hardware

### Microcontroller

For this board, I decided to use the **ATtiny3217**. It's small, easy to use, power-efficient, and a great choice for simple projects.

### USB Interface

The board uses a USB-C connector. I chose USB-C because it is modern, compact, and convenient to use.

I also added a USB protection chip to help protect the USB data lines.

The USB interface is connected to a **CH340N** USB-to-UART converter, which provides communication between the computer and the ATtiny3217.

### Power

There are two voltage levels available on the board:

- **5V** — This comes from the USB-C connector or the 5V pin header. It is converted to 3.3V using an **AP2112K** voltage regulator.

- **3.3V** — The entire board operates at this voltage.

I also added a small red LED to indicate that the board is powered.

### NeoPixel LED

The board includes an **SK6812MINI** programmable RGB LED. It can be used to display different colors and provide visual feedback.

### Button

There is also a small button available for general use in your code.

## Pinout

Next to every pin, its name is printed on both the top and bottom sides of the PCB.

> **Note:** On the top side, the pins are labeled without the **"P"** prefix.

### Official Pinout Image

<img src="assets/pinout.png" alt="MyTtiny pinout" width="500"/>


## Board

### Schematic

I tried to make the schematic as clean and easy to understand as possible.

<img src="assets/schematic.png" alt="MyTtiny schematic" width="500"/>

### PCB

#### Top

<img src="assets/top.png" alt="MyTtiny PCB top side" width="500"/>

#### Bottom

<img src="assets/bottom.png" alt="MyTtiny PCB bottom side" width="500"/>

## Why I Made This

Honestly, I originally made this board because I was bored. 

I also didn't really want to use some of the existing development boards available to me, so I decided to design my own.

I chose the **ATtiny3217** as the main microcontroller because I wanted to try something different instead of using more common chips such as the RP2040 or ESP32.