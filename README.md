# STM32-uart-pwm-led

Simple embedded project using STM32.

## Features
- Control LED via UART commands
- Commands:
  - `on` – turn LED on
  - `off` – turn LED off
  - `0–100` – set brightness (PWM)

## How it works
- UART receives ASCII commands
- Input is parsed into:
  - string commands (`on/off`)
  - numeric values (PWM %)
- Timer generates PWM signal
