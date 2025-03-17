+++
title = "Real-Time Audio Synthesizer Optimization"
description = "Enhanced the performance of an embedded real-time audio synthesizer by implementing efficient task scheduling and interrupt-driven I/O."
date = 2025-01-18

[extra]
date_start = 2024-11-15
image = "synth.jpeg" # Placeholder image
top_project = true

[taxonomies]
projects = ["CESE Master"]
skills = ["C Programming", "RTOS", "Task Scheduling", "Interrupt Handling"]
+++

As part of the **Real-Time Systems** course at TU Delft, I worked on optimizing an embedded audio synthesizer. The initial codebase operated on a superloop architecture, leading to performance issues such as audio clipping and latency. The project's goal was to refactor the synthesizer to utilize a Real-Time Operating System (RTOS) for efficient task management.

![Synthesizer Hardware](/images/synthesizer_hardware.png)

The synthesizer hardware consisted of a microcontroller development board running the Zephyr RTOS, connected to a peripherals board with switches, encoders, and LEDs for user interaction. The system processed keyboard inputs via a serial console to generate audio signals.

## Responsibilities
- Analyzed the existing superloop-based synthesizer code to identify performance bottlenecks
- Implemented RTOS-based task scheduling to manage peripheral polling, keyboard input processing, sound synthesis, and audio output tasks
- Transitioned from polling to interrupt-driven I/O for peripherals to reduce latency and CPU load
- Measured and optimized task execution times to ensure deadlines were met, preventing audio glitches
- Documented the system architecture and optimization strategies in a detailed report

## What I Learned
This project deepened my understanding of real-time systems and the importance of efficient task scheduling in embedded applications. I gained hands-on experience with RTOS concepts, interrupt handling, and performance optimization techniques critical for developing responsive and reliable embedded systems.
