---
layout: default
title: Hardware Levels
prev: options
next: conclusion
audio: levels
image: levels.png
alt: Diagram of the hardware levels from Barkalov, p. 26
---

- Hardware levels (Barkalov, p. 25)
    - System
    - Processor/Register Transfer (RTL)
    - Logic
    - Circuit

<!--
During the design process, designers work at four different levels of detail.

To begin, the design starts at the circuit level, the lowest level of the four. At this level,
designers lay out logic circuits from actual transistors. Gates like AND, OR, and NOT, as well
as simple circuits like the D flip-flop, a single bit of memory. Second, at the logic level
more complex logic is designed using the components designed at the circuit level. Things like
adders, shifters, 32-bit storage elements, and more. Next, in the processor level (also called
the register transfer level or RTL), designers use the more complex circuits of the logic level
and use them to build larger components, like an ALU (Arithmetic Logic Unit) or a multiplier.
Finally, at the system level, the full system is built from components designed in the register 
transfer level.

At each level in the process, the circuits designed in the previous level are used to build up
the circuits of the current level. By this method, designers make sure that when designing the
whole system they don't have to think about the individual logic gates or even transistors all
the way at the bottom. This method saves designers a ton of time and effort.

- levels of abstraction
- system built from processor chunks, etc. etc.
-->