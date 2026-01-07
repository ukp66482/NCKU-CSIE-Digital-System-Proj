# Question List

## Overview
After completing the Final Project, please answer all questions listed in this directory.  
Include your answers in the final report and be prepared to present them.

Some of the answers may be found in the official documentation. Students are encouraged to consult the AMD/Xilinx or tul FPGA documents as needed.

## Q1. 
Why is the clock on Pin 16 of the PYNQ-Z2 board 125 MHz?

Where does this clock come from, and why is this specific frequency used?

## Q2. 
What are Byte Addressing and Word Addressing?

Under what circumstances does BRAM use byte addressing, and when does it use word addressing?

In this design, which addressing mode does our BRAM use, and how do we set the BRAM address to match this addressing scheme?

## Q3.
Briefly describe what memory-mapped I/O is, 
and explain what happens if I access (read or write) a GPIO memory-mapped address? 

(please describe the sequence of operations from the hardware’s point of view).

## Q4.
In this design, what is the purpose of the HP port that the CDMA is connected to?

During memory mapping, what address range is assigned to this HP port, and why is it allocated to that specific range?

## Q5.
In this design, we use a CDMA to read/write data from/to DDR memory.
 
From the perspective of computer organization, memory accesses can lead to cache incoherence issues. In our implementation, this problem was resolved at the software level. 

Explain why the software prevents cache incoherence in this case, and additionally discuss what hardware mechanisms could also be used to address this issue.

## Q6.
In FPGA architectures, combinational logic is implemented using LUTs (Look-Up Tables), whereas ASIC design—such as what we learn in the Digital Systems course—relies on cell-based standard logic gates (e.g., NAND, NOR, XOR). In ZYNQ7020 devices, each LUT can implement any 6-input logic function. But it is composed of two 5-input LUTs and a multiplexer.

Explain how a 6-input LUT is constructed using two 5-input LUTs and a multiplexer.

![LUT](./pic/LUT.png)

Explain why we don't use 4-input LUTs nowadays, and what advantages 6-input LUTs provide over 4-input LUTs in FPGA design.


## Q7.
Why do these two blocks use different AXI Interconnect IP cores?

(Why one is AXI Interconnect and the other is AXI SmartConnect)
![HP_GP](./pic/HP_GP.png)