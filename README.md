# MIPS Disassembler

This program is a MIPS disassembler designed to interpret 32-bit MIPS instructions. It disassembles MIPS executable files, printing the assembly instructions to the screen.

## Description

The code consists of a C++ program that reads a MIPS executable file and disassembles its instructions, displaying them in human-readable assembly language.

## Instructions

Compilation
To compile the code, use the following command:

```bash
g++ mips_disassembler.cpp -o mips_disassembler
```

## Usage

Run the executable with the MIPS executable file as an argument:

```bash
./mips_disassembler mips_executable
```

Replace mips_executable with the actual MIPS executable file you want to disassemble.

## Functionality

The disassembler performs the following tasks:

- Reads a MIPS executable file in binary format.
- Interprets the 32-bit MIPS instructions present in the file.
- Converts the instructions into human-readable assembly language.
- Displays the disassembled instructions on the screen.
- Understanding the Output
- The disassembler interprets various MIPS instruction types, such as arithmetic, logical, control flow, load/store, etc. It decodes the opcode and relevant fields of each instruction to display the corresponding assembly operation.

The output includes assembly instructions along with their associated registers and immediate values, providing a clear representation of the executable's instructions.

## Note

Ensure that you have a compatible MIPS executable file to disassemble using this program.
