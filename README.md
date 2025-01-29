# 8-bit ALU (Arithmetic and Logic Unit)

This repository contains the design and implementation of an 8-bit ALU (Arithmetic and Logic Unit) using **Proteus** for a Computer Architecture course project. The ALU performs basic arithmetic and logical operations such as addition, subtraction, multiplication, and logical AND, OR, and NOT operations.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [How It Works](#how-it-works)
- [Usage](#usage)
- [Screenshots](#screenshots)
- [Conclusion](#conclusion)

## Project Overview
This ALU project demonstrates a basic implementation of a functional 8-bit ALU, which can perform arithmetic and logical operations based on control inputs. The project was built using **Proteus** simulation software, which allows for hardware-level simulation and testing of digital circuits.

The ALU takes two 8-bit input values and an operation selection signal to output the result of the selected arithmetic or logic operation. It is a key component in many digital systems and microprocessor designs.

## Features
- 8-bit wide input and output for arithmetic operations.
- Supports basic arithmetic operations:
  - **Addition** (A + B)
  - **Subtraction** (A - B)
  - **Multiplication** (A * B)
- Supports basic logic operations:
  - **AND**
  - **OR**
  - **NOT**
- Control signals to select between operations.
- Displays the results on output LEDs.
- Handles both signed and unsigned operations (if extended).
- Designed in a modular way to be easily extensible for more operations.

## Technologies Used
- **Proteus**: Used for hardware simulation and testing of the ALU.
- **VHDL** or **Verilog** (optional, depending on whether you used these for implementing the logic gates or control unit, otherwise Proteus’s own components were used for design).
- **Arduino** (if used for microcontroller integration or control).
  
## How It Works
- **Inputs**: 
  - Two 8-bit data inputs, A and B.
  - A 3-bit control signal to select the desired operation (e.g., `000` for ADD, `001` for SUBTRACT, `010` for AND, etc.).
- **Operations**: 
  - The ALU uses a multiplexer to select the desired operation based on the control signal.
  - Depending on the control signal, the ALU performs the corresponding operation, either arithmetic or logical.
  - The result is displayed on the 8-bit output and optionally can be shown using LEDs or a display on the Proteus simulation.
  
### Example of Control Signal Mapping:
| Control Signal | Operation       |
|----------------|-----------------|
| 000            | Addition (A + B) |
| 001            | Subtraction (A - B) |
| 010            | AND (A AND B) |
| 011            | OR (A OR B) |
| 100            | NOT (A NOT) |
  
## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/USERNAME/8-bit-ALU.git
