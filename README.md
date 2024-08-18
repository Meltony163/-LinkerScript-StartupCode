# STM32F103C8T6 Linker Script and Startup Code

This repository contains the linker script and startup code specifically designed for the STM32F103C8T6 microcontroller. These files are essential for bare-metal programming, enabling you to correctly set up the memory regions, vector table, and initialize the microcontroller at startup.

## Repository Structure

- **`linker.ld`**: The linker script that defines the memory layout of the STM32F103C8T6, including the flash memory, SRAM, and stack.
- **`startup_stm32f103c8t6.s`**: The assembly startup code that sets up the initial stack pointer, vector table, and handles the reset and default interrupt service routines (ISRs).

## Getting Started

### Prerequisites

To build and run the code in this repository, you will need:

- **ARM GCC Toolchain**: `arm-none-eabi-gcc` and related tools.
- **STM32CubeProgrammer** (optional): Another option for flashing the microcontroller.

### Building the Project

# Memory Layout
The memory layout for STM32F103C8T6 is as follows:

- **Flash**: 64 KB (starting at 0x08000000)
- **SRAM**: 20 KB (starting at 0x20000000)

## Customization

You can modify the linker script (linker.ld) to suit your application's memory requirements. Additionally, you can edit the startup code to add custom ISR handlers or other initialization code.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests if you have improvements or bug fixes.

## References

- STM32F103C8T6 Datasheet
- ARM Cortex-M3 Technical Reference Manual
