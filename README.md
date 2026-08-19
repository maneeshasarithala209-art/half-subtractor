# Half Subtractor using Verilog

## Overview

A Half Subtractor is a combinational logic circuit that subtracts one binary digit from another. It has two inputs (A and B) and produces two outputs:

- Difference
- Borrow

## Truth Table

| A | B | Difference | Borrow |
|---|---|------------|--------|
| 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 1 |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 0 |

## Boolean Expressions

Difference = A XOR B

Borrow = A' AND B

## Files

- `half_subtractor.v` – Verilog source code
- `half_subtractor_tb.v` – Testbench
- `waveform.png` – Simulation waveform
- `simulation_output.png` – Console output

## Software Used

- Verilog HDL
- ModelSim / Vivado Simulator / Icarus Verilog
- GTKWave (optional)

## Simulation

Compile:

```bash
iverilog -o hs half_subtractor.v half_subtractor_tb.v
```

Run:

```bash
vvp hs
```

Generate waveform:

```bash
gtkwave waveform.vcd
```

## Result

The simulation verifies that the Half Subtractor correctly generates the Difference and Borrow outputs for all possible input combinations.

## Author

Your Name