---
layout: default
title: Design Options
prev: costs
next: design
audio: options
image: semi-custom.jpg
alt: Image of a semi-custom ASIC design by Antoinebercovici of Wikimedia Commons, licensed under CC BY-SA 3.0
---

- Customizability
    - Full custom
    - Semi custom
    - Standardized

- Programmability
    - Read-only (ROM)
    - Write-once (PROM)
    - Write-many (EEPROM)
    
<!--
The most important variable to think about when designing an ASIC is customization.

Customization is how customized you want the circuit to be. Generally, the more customized
the more efficient the circuit will be, but the more expensive the design process will be 
(often *much* more expensive for the most customized).

The levels of customization can be grouped into three categories, of descending customization:
full custom, semi custom (or gate array), and standardized. Full custom is the most custom
designed, with the circuit being designed from the ground up for it's task. This is a very
expensive and lengthy process, as modern ASICs can have billions of transistors. It takes a lot
of work to design a full custom chip. There are some tools to help with the workload however.
CAD (computer assisted design) tools are quite common for low-level circuits, and can do a lot
of the work. There are also standard designs for low level circuits and logic gates, which are
called standard cells. These standard cells are usually developed by a manufacturer and licensed
out to designers, although there also exist open-source cells.

Semi-custom (aka gate array) designs are ones that use large general components, which are then
"programmed" to accomplish the specific task of the ASIC. To make this work, semi-custom circuits
are usually larger than full custom, because they haven't been optimized from the ground up for
their task. This programming has several variations itself. In some designs, the purpose is built
into the circuit during manufacture. This is called read-only memory, or ROM. Some other designs
build the circuit, and then burn the program into the circuit. This is called write-once memory
or programmable ROM (PROM). The process of burning the program in is destructive, and can only be done
once. These two types of programming are often called firmware, although the terms usage has
expanded to more reusable types of memory. One of those types of memory is called electronically-
erasable PROM, or EEPROM. This type of memory can be written to multiple times, allowing the
circuit to serve different functions throughout its lifetime. However, EEPROM still has a limit
on how many times it can be written to, and is quite slow to write to. A more modern equivalent
is flash memory, which serves the same purpose but solves both these issues by being very fast,
and very reusable.

Finally, there are standardized ASIC designs. These circuits are usually for very common
purposes, like a USB interface which is used in any USB peripheral. These ASICs hardly need
any design at all, and are often available off the shelf as components to be used in a larger
design.

- customizablity
    - full custom
        - designed from the ground up
        - smaller & more efficient (maximize usage)
        - slower design/manufacture
        - higher cost
    - semi-custom
        - work from a base template, build logic onto predefined areas
        - faster/cheaper design, but never maximum efficiency
    - application-specific
        - premade for specific purpose
        - often for applications that are very common
        - e.g. USB controller, Ethernet interface
    
    - standard cells
    - open-source hardware 
    
- programmability
    - read only (ROM, firmware), write once (PROM), write many (EEPROM, flash EEPROM (fast))
-->