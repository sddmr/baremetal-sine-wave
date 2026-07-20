# STM32 Sine Wave Generator

This project aims to generate a high-precision, continuous sine wave on microcontrollers (specifically the STM32 series) using C/C++. It leverages Hardware Timers, a Digital-to-Analog Converter (DAC), and Direct Memory Access (DMA) architectures.

## Features

*   **Low-Level & Bare-Metal Approach:** Efficient memory management that minimally occupies CPU cycles.
*   **Look-Up Table (LUT):** Eliminates mathematical processing overhead by using a pre-calculated look-up table for sine wave values.
*   **DMA Integration:** Continuous, non-blocking signal generation by feeding the DAC output directly from memory (memory-to-peripheral).
*   **Configurable Frequency:** Easy adjustment of the wave frequency via Timer settings (Prescaler and ARR).

## Technologies and Tools

*   **Language:** C / C++
*   **Hardware:** STM32 Development Board (e.g., STM32 Nucleo)
*   **Peripherals:** DAC, DMA, Hardware Timers
*   **Development Environment:** STM32CubeIDE / Makefile & GCC-based toolchains

## Hardware Pinout

*   **DAC Output Pin:** (Update according to your specific board, e.g., PA4 or PA5)
*   **GND:** Must be connected to the ground of the oscilloscope or measuring device.

*(Note: You can connect the DAC output pin to an oscilloscope to visualize the signal.)*

## Installation and Usage

1.  Clone this repository to your local machine:
    ```bash
    git clone [https://github.com/YOUR_USERNAME/repo-name.git](https://github.com/YOUR_USERNAME/repo-name.git)
    ```
2.  Open the project via STM32CubeIDE or compile it using your preferred toolchain.
3.  Flash the code onto your development board.
4.  If you want to change the timer frequency or DMA buffer size, you can update the relevant configuration variables within `main.c`.

