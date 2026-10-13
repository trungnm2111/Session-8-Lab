Session 8 - Tuesday, 29 Sep 2026 (4 working days)

Section: Linux Kernel Programming | Topic: Linux OS Overview & Kernel Module/Driver Basics | Duration: 4 working days (8 hours/day)

Purpose: Understand the user-space/kernel-space split, get a conceptual map of the Linux kernel's major components, and write a minimal Loadable Kernel Module and driver. | Expectation: Kernel component-map diagram + working hello.ko module + minimal GPIO driver controlling an LED/button on the target board.

Topics

• Basic concept of an Operating System: what it is and why it is needed

• Linux Operating System concept and its main components

• User space vs. Kernel space: concept, memory, and process differences between the two

• Linux Kernel Components overview: how Memory Management, File System, Process Management, Network, and Device Driver subsystems relate to each other (conceptual survey, not deep-dive)

• Linux Kernel Module (LKM) concept: what it is and why modules exist; built-in vs. loadable modules

• Linux Driver concept: how a driver fits between hardware and the kernel's user-facing interfaces

• Module lifecycle: init/exit functions, insmod/rmmod/modprobe, module parameters, dependencies

• Writing a simple driver to control basic hardware - adapted to whatever GPIO-connected LED/button is available on the trainee's own target board

Readings / Resources • Kernel.org Documentation - Overview • TLPI ch.1-2 - Fundamental Concepts • Linux Kernel Module Programming Guide • LDD3 - Linux Device Drivers, 3rd Ed. (free online)

Studio / Lab

• Draw a one-page diagram of the Linux kernel's major components (Memory Management/File System/Process Management/Network/Device Driver) and how they interact

• Write hello.ko with init/exit functions and a module parameter (module_param); load/unload it and inspect dmesg

• Write a minimal GPIO character driver that turns an LED on/off or reads a button state on your target board, and exercise it with simple read/write calls from userspace