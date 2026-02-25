# Concurrent IPC Processing System (C, pthreads, Linux)

A multi-process concurrent computation system implemented in C on Linux, combining System V shared memory, POSIX semaphores, and pthread-based parallelism.

## Overview

This project implements a producer–consumer architecture where:

- A producer process writes computational tasks into shared memory.
- A consumer process retrieves tasks and executes polynomial operations.
- Synchronization is enforced using named semaphores.
- Thread-level parallelism is achieved using pthreads.

The system focuses on concurrency correctness, inter-process communication, and controlled resource management.

## Architecture

- **IPC Mechanism:** System V shared memory
- **Synchronization:** POSIX named semaphores (`sem_open`)
- **Threading Model:** POSIX threads (`pthread`)
- **Concurrency Pattern:** Bounded buffer (Producer–Consumer)

## Key Concepts Demonstrated

- Inter-Process Communication (IPC)
- Shared memory coordination
- Mutex-based synchronization
- Thread lifecycle management
- Dynamic memory allocation
- Resource cleanup and lifecycle control

## Build

```bash
make
```

## run:
```bash
./producer
```

```bash
./consumer
```
