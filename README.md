# 4bit-abs-val
4-Bit Optimal Absolute-Value Detector

Designed a 4-bit optimal “Absolute-value Detector” focusing on minimizing energy while maintaining specific delay constraints.

Phase 1: Explored different logic architectures and styles, including truth table-based logic minimization and arithmetic functions, and developed a gate-level design sized for minimum delay.

Phase 2: Implemented the design in Cadence, verified functionality in Spectre, performed critical-path delay analysis, and established a simulation delay model.

Phase 3: Developed logical-effort-based sizing and supply voltage-dependent delay and energy models, applied optimization techniques to minimize energy at 1.5x delay, and verified performance through simulation.

Successfully optimized the circuit design for energy efficiency while meeting delay constraints. Achieved a significant reduction in simulation energy from 4240.74 fJ to 542.955 fJ, and analytical energy dropped from 7.8 Eg to 3.82 Eg, all while maintaining consistent simulation time.

# Logic Gate Design

![alt text](https://github.com/mqyeung/4bit-abs-val/blob/main/GATE_LEVEL.png?raw=true)

# Transistor Level Design

![alt text](https://github.com/mqyeung/4bit-abs-val/blob/main/V3_2.png?raw=true)
