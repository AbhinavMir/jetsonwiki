---
title: "Glossary: Because NVidia couldn't be bothered."
draft: false
---


1. **SPI (Serial Peripheral Interface)**: A synchronous serial communication interface used for short-distance communication, primarily in embedded systems. It enables a master device to communicate with one or several slave devices over short distances at high speeds.

2. **EMMC (Embedded MultiMediaCard)**: A type of solid-state storage typically used in smartphones, tablets, and other consumer electronics. It provides a permanent, non-volatile storage medium for the device.

3. **QSPI (Quad SPI)**: QSPI (Quad Serial Peripheral Interface) is a protocol used for communication between a microcontroller and peripheral devices like flash memory. It uses four lines (quad) for data transmission, allowing for faster data transfer compared to standard SPI that uses a single line. This makes QSPI effective for applications needing high-speed data reading, such as executing code directly from a flash memory (XIP - Execute in Place). It An enhanced version of the standard SPI that allows for faster data transfers. It uses four lines (instead of one, as in standard SPI) for data transmission, which speeds up operations.

Each term relates to different methods and partitions used for the storage and transfer of firmware and data within these computing platforms. The mentioned XML files (`flash_l4t_txxx.xml`) are likely configuration files for the bootloader, specifying how the device's operating system is to be loaded and from which memory partition.