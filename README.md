# 4bit-abs-val
4-Bit Optimal Absolute-Value Detector

Designed a 4-bit optimal “Absolute-value Detector” focusing on minimizing energy while maintaining specific delay constraints.

Successfully optimized the circuit design for energy efficiency while meeting delay constraints. Achieved a significant reduction in simulation energy from 4240.74 fJ to 542.955 fJ, and analytical energy dropped from 7.8 Eg to 3.82 Eg, all while maintaining consistent simulation time.

# Summary:

**Phase 1:** Explored different logic architectures and styles, including truth table-based logic minimization and arithmetic functions, and developed a gate-level design sized for minimum delay.

**Phase 2:** Implemented the design in Cadence, verified functionality in Spectre, performed critical-path delay analysis, and established a simulation delay model.

**Phase 3:** Developed logical-effort-based sizing and supply voltage-dependent delay and energy models, applied optimization techniques to minimize energy at 1.5x delay, and verified performance through simulation.

# Logic Gate Design

![alt text](https://github.com/mqyeung/4bit-abs-val/blob/main/GATE_LEVEL.png?raw=true)

A) Architecture 
3 Bit Half Adder + 3 Bit Mux + 3 Bit Full Adder
Note the lack in subtractor/comparator

B) Logic Circuit Style 
TG Based Half Adder (XOR) + TG Based Mux 
+ TG Based Full Adder (XOR) + CMOS NOR (used in 3 way OR)

C) WHY: about Area, about Delay, other
Removes a whole adder in worst case
If absolute value negates a negative value, it will be negated again (subtractor approach). less gates = less capacitance = less delay
Half adder can be simplified down, reducing worst case
(since only 3 bits are used, and LSB does not change)

# Transistor Level Design

![alt text](https://github.com/mqyeung/4bit-abs-val/blob/main/V3_2.png?raw=true)

# Transistor Level Component Diagram

![alt text](https://github.com/mqyeung/4bit-abs-val/blob/main/LOGIC%20GATE%20BREAKDOWN.png?raw=true)

# Critical Path Delay

![alt text](https://github.com/mqyeung/4bit-abs-val/blob/main/critical%20path%20analysis.png?raw=true)

# Testbench

![alt text](https://github.com/mqyeung/4bit-abs-val/blob/main/testbench.png?raw=true)
