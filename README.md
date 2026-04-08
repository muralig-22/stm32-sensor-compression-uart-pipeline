# STM32 Sensor Data Compression and UART Packet Streaming

A mini embedded firmware project built on **STM32F446RE** to simulate high-resolution sensor streams, apply **delta encoding compression**, batch samples into packets, and transmit them over UART in real time.

## Features
- Simulated **24-bit and 16-bit sensor signals**
- **Delta encoding** for efficient 8-bit transmission
- Sample batching into **10 packets per second**
- Custom UART packet framing
- Real-time monitoring using **Tera Term**
- Built and tested on **STM32 Nucleo-F446RE**

## Packet Format
[START][PACKET_ID][DELTA_DATA...][END]

Example:
AA 2B 02 03 FF FE 01 ... 55

## Learnings
- Data compression in embedded systems
- Delta encoding vs uniform quantization
- UART protocol framing
- Real-time packet scheduling
- Firmware debugging and validation
