# 8-bit Computer in VHDL

This project is part of the advance electronics final project. Instruction set and architecture of 8-bit computer are available at Chapter 13 in the book "Introduction to Logic Circuit and Logic Design with VHDL"


## 8 bit Computer Architecture

This is the image of the 8 bit computer architecture from the books.



## Brief Explanation

To create this VHDL program for each element we need creating all entities, connection each of the component.

Structure of program

* Computer.vhdl
  * cpu.vhdl
          * control_unit.vhdl
          * data_path.vhdl
          * ALU.vhdl
  * memory.vhdl
          * rom_128x8_sync.vhdl
          * rw_96x8_sync.vhdl
         




## Run this program using ghdl

To run this program we use ghdl and gtk wave.

```bash
ghdl -a --ieee=synopsys -fexplicit files.vhdl
```

```bash
ghdl -e --ieee=synopsys -fexplicit files
```



## Simulate the program using gtk wave

to make vcd test bench files for simulation

```bash
ghdl -r files

ghdl -r files --vcd = 'filesName.vcd'
```

run the vcd

```bash
gtkwave filename.vcd
```

Part of code is from:

https://www.fpga4student.com/2016/12/a-complete-8-bit-microcontroller-in-vhdl.html
