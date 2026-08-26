# MyTtiny

My own development board based on the chip **ATtiny3217**.

## Features

One of the biggest features for me is that it is made mainly for myself, but I want to make it good enough so you can use it too.

* **Compact size**

  I tried to make this board as small as possible, and I think I did a really good job with its size: **29.718 × 17.018 mm**.

* **USB-C**

  Yeah, this is a small thing, but it is really useful. With USB-C, you can program and communicate with the board. (Yeah, I added both resistors, so **it works with USB-C to USB-C cables**.)

* **UART**

  I decided to add the **CH340N** on board, so with this, you can upload programs and also use the serial monitor.

* **NeoPixel LED**

  If I want to use this board without any external hardware, I like having something that can provide visual feedback.

* **Pins**

  Every header pin has its name on the top and also on the bottom side.

## Hardware

  ### Microcontroller

  For this board, I decided to use the **ATtiny3217** chip. It's because it's small, easy to use, has low power usage, and for my simple projects, it's a great choice.

  ### USB Interface

  For the port, I decided to use USB-C. It's mainly because it's modern, actually easy to wire, and also small and light. I also added a USB-C protection chip, so there shouldn't be any problems.

  After that, there is the UART chip **CH340N**. This connects the ATtiny and USB together.

  ### Power

  So, on the board, there are 2 voltages:

  * **5V** — This comes from the USB-C port or the 5V pin header. This isn't used in the system; it's just converted to 3.3V using the **AP2112K** chip.

  * **3.3V** — The whole system runs on this voltage.

  I also added a small red LED to show that the power is working.

  ### NeoPixel LED

  On the board, I added an **SK6812MINI**. It's small and easy to use for showing lights.

  ### Button

  There is one small button for classic usage in code.