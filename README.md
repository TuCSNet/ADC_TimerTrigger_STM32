# ADC_TimerTrigger_STM32

## Overview

This project demonstrates ADC-based temperature measurement using a timer-triggered conversion sequence. TIM2 generates an update event every 1 second to trigger ADC conversions via TRGO. DMA transfers the ADC results to memory, and the calculated temperature is displayed on a PC terminal via UART.

## Hardware

- STM32 Nucleo-F446RE development board
- USB connection to PC

## Software and Tools

- STM32CubeIDE
- STM32CubeMX
- STM32 HAL
- C programming language

## Features

- ADC configuration for internal temperature sensor measurement
- TIM2 configuration to generate an update event every 1 second, triggering ADC data acquisition
- UART communication between the STM32 microcontroller and a PC terminal

## Project Structure

- `Core/Inc/` — application header files
- `Core/Src/` — application source files
- `Drivers/` — STM32 HAL and CMSIS dependencies
- `.ioc` — STM32CubeMX configuration file
