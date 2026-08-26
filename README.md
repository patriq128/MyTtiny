# MyTtiny

My own development board based on the **ATtiny3217** chip.

<img src="assets/main.png" alt="main" width="500"/>

## Features

One of the biggest features for me is that it was made mainly for myself, but I want to make it good enough for other people to use too.

- **Compact size**

  I tried to make this board as small as possible, and I think I did a really good job with its size: **29.718 × 17.018 mm**.

- **USB-C**

  Yeah, this is a small thing, but it is really useful. With USB-C, you can program and communicate with the board. (Yeah, I added both resistors, so **it works with USB-C to USB-C cables**.)

- **UART**

  I decided to add the **CH340N** to the board. With this, you can upload programs and also use the serial monitor.

- **NeoPixel LED**

  If I want to use this board without any external hardware, I like having something that can provide visual feedback.

- **Pins**

  Every header pin has its name on both the top and bottom sides.

## Hardware

### Microcontroller

For this board, I decided to use the **ATtiny3217**. It's small, easy to use, has low power consumption, and is a great choice for my simple projects.

### USB Interface

For the port, I decided to use USB-C. It's mainly because it's modern, easy to wire, and also small and lightweight. I also added a USB-C protection chip, so there shouldn't be any problems.

After that, there is the **CH340N** UART chip. This connects the ATtiny to the USB interface.

### Power

There are two voltage levels on the board:

- **5V** — This comes from the USB-C port or the 5V pin header. It isn't used directly by the system; instead, it is converted to 3.3V using the **AP2112K** regulator.

- **3.3V** — The whole system runs on this voltage.

I also added a small red LED to indicate that the board is powered.

### NeoPixel LED

I added an **SK6812MINI** to the board. It's small and easy to use for displaying different colors.

### Button

There is one small button for general use in code.

## Board

### Schematic

I tried to make the schematic as clean as possible.

<img src="assets/schematic.png" alt="schematic" width="500"/>

### PCB

**Top**

<img src="assets/top.png" alt="top" width="500"/>

**Bottom**

<img src="assets/bottom.png" alt="bottom" width="500"/>

## Why I Made This

Actually, I made this because I was bored and didn't want to use some existing development boards that I don't really like. I also decided to use the **ATtiny3217** as my main chip because I didn't want to use classic chips like the RP2040 or ESP32.
