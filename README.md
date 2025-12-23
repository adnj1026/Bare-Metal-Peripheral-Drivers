# STM32F401RE Bare-Metal Peripheral Drivers

This repository contains a bare-metal firmware project for the STM32F401RE
microcontroller. The goal of this project is to design and implement
peripheral drivers from scratch by directly programming MCU registers,
without using HAL, Arduino, or an operating system.

The project focuses on building clean, reusable drivers and documenting
design decisions, assumptions, and failure modes.

## Target Hardware
- STM32F401RE (Nucleo board)

## Project Goals
- Understand STM32 peripheral architecture through register-level programming
- Develop peripheral drivers for GPIO, USART, SPI, and I2C
- Learn proper clock configuration and interrupt handling
- Design clean driver APIs and modular firmware structure
- Document engineering decisions and debugging insights

## Planned Components
- GPIO driver
- USART driver (interrupt-driven)
- SPI or I2C driver
- Basic interrupt and NVIC configuration
- Demo application to validate drivers on real hardware

## Development Approach
- Bare-metal programming (no RTOS, no HAL)
- Incremental development with frequent testing on hardware
- Git used to track design evolution and fixes
- Documentation focused on engineering reasoning, not definitions

## Status
- Project initialized
- Driver development in progress
