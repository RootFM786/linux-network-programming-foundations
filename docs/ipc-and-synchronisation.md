# Inter-Process Communication and Synchronisation

## Overview

The coursework explored how separate processes communicate and coordinate access to shared resources.

## Semaphores

Semaphores were used to control when processes could access shared resources and to prevent uncontrolled simultaneous access.

## Shared Memory

The producer/consumer exercise used shared memory so two processes could access the same buffer.

One process acted as the producer and wrote items into the buffer, while the other acted as the consumer and read them.

## Producer / Consumer Exercise

The exercise demonstrated:

- creating shared memory
- attaching a process to the shared segment
- signalling with semaphore operations
- controlling producer and consumer timing
- cleaning up the shared-memory segment

## Security Relevance

These concepts matter because real applications frequently rely on IPC.

For an analyst, understanding IPC can help when investigating:

- processes exchanging data locally
- unusual shared-memory activity
- software instability caused by poor synchronisation
- malware using local IPC mechanisms to coordinate components

This coursework was introductory and did not involve malware analysis, but the underlying operating-system concepts are transferable.