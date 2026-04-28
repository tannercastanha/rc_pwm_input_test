This project verifies that a FlySky FS-iA6B receiver is receiving PWM signals from a FlySky FS-i6X transmitter using an STM32-Nucleo-F446RE board.

The program works by receiving a PWM signals from Channels 1 and 2 from the transmitter, measuring the pulse width via TIM2, and prints the pulse length (us) in a serial terminal via UART.

Hardware used:
-STM32-Nucleo-F446RE
-FS-i6X
-FS-iA6B

Config:
PA0 - TIM2_CH1
PA1 - TIM2_CH2
PA2 - USART_TX
PA3 - USART_RX

TIM2:
Clock Source: Internal Clock
Channel 1: Input Capture direct mode
Channel 2: Input Capture direct mode
Prescalre 83
Counter Period: 65535
