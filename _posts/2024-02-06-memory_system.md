---
layout: default
title: Home
---

# Memory System for efficient memory management in low-level programming

1. Registers
```
Registers are the fastest and smallest storage locations within the CPU, used for temporary data and holding intermediate results during program execution.
Examples include general-purpose registers, instruction pointers, and program counters.
```
2. Stack Memory
```
Stack memory is used for managing function calls, local variables, and function parameters in a Last-In-First-Out (LIFO) manner.
Stack memory is managed automatically by the compiler or runtime system.
```
3. Heap Memory
```
Heap memory is used for dynamic memory allocation, allowing for flexible memory management at runtime.
Memory allocated on the heap must be explicitly managed by the programmer, usually through functions like malloc() and free() in C or new and delete operators in C++.
Heap memory is not organized in a specific order like the stack and is generally slower to access than stack memory.
```
4. Static Memory
```
Static memory, also known as data segment memory, is used for storing global variables and static variables.
Global variables have a lifetime throughout the entire program execution.
Static variables inside functions retain their values across multiple function calls.
Static memory is allocated at compile-time and persists throughout the program's execution.
```
5. Constants Memory
```
Constants memory is used for storing constant data such as string literals and global constants.
String literals and other constant data are typically stored in read-only memory (ROM) or a separate memory segment.
Constants memory is generally immutable and cannot be modified at runtime.
```
6. Program Code Memory:
```
Program code memory, also known as text segment memory, is used for storing executable code instructions.
It contains the compiled machine code instructions of the program.
Program code memory is typically read-only and is shared among multiple processes if the operating system supports it.
```
7. Memory Mapped I/O (MMIO):
```
Memory-mapped I/O is a technique used to access hardware devices by mapping their control registers and data buffers into the address space of the processor.
Hardware devices are accessed by reading from or writing to specific memory addresses.
MMIO allows low-level programming to interact directly with hardware devices, such as network interfaces, storage controllers, and peripheral devices.
```
