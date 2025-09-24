# 8x8 Booth Multiplier

## Overview

This project implements an 8x8 Booth multiplier, a hardware module that multiplies two 8-bit numbers using the Booth algorithm. Booth's algorithm is efficient for signed binary multiplication and optimizes the number of required addition and subtraction operations.

## Features

- **8-bit input**: Multiplies two signed 8-bit numbers.
- **Booth's algorithm**: Reduces the number of arithmetic operations, especially for consecutive 1s in the multiplier.
- **Signed multiplication**: Correctly handles positive and negative inputs.
- **Synthesizable hardware design**: Suitable for FPGA or ASIC implementation.

## Booth Algorithm Summary

Booth's algorithm encodes the multiplier to minimize the number of addition/subtraction operations. It scans pairs of bits and determines whether to:
- Add the multiplicand
- Subtract the multiplicand
- Do nothing (for runs of zeros)

This results in efficient multiplication, especially for numbers with consecutive 1s.

## File Structure

- `booth_multiplier.v` or `booth_multiplier.vhdl`: Main source code for the multiplier.
- `testbench.v` or `testbench.vhdl`: Testbench for simulation and verification.
- `README.md`: This documentation.
- `results/`: May include waveform images or simulation results.

## How to Use

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Agarwal-Pranav/multiplier_booth.git
