Download Link: https://assignmentchef.com/product/solved-csc3050-programme-4
<br>
<span style="font-size: 41.8867px; letter-spacing: -1px;">Overvie</span><span style="font-size: 2.61792em; letter-spacing: -1px;">w</span>

You have learnt MIPS instructions and finished a ALU module using verilog in the 3 projects before. In this programme, you will deal with a single-cycle processor which can execute MIPS instructions with verilog.

Compared with programme 3, you should design a whole CPU module, including the clock, instruction memory, registers, ALU, data memory and control unit. You should define the MIPS instruction and build the datapath in a verilog file and test the MIPS instructions in the test file, then display the result like programme 3.

<h1>Block Diagram</h1>

The CPU must support:

1) Data transfer instructions:

– lw, sw

2) Arithmetic instructions:

<ul>

 <li>add, sub, addu, subu</li>

 <li>addi, addiu</li>

</ul>

3) Logical instructions:

<ul>

 <li>and, or, nor, xor</li>

 <li>andi, ori</li>

</ul>

4) Branch/Jump instructions:

<ul>

 <li>beq, bne, slt</li>

 <li>j, jr, jal</li>

</ul>

We can see that, in one clock cycle, the cpu read one instruction in the instruction memory and decode the MIPS instruction with the registers and control unit. The operation code and function code in MIPS instruction are sent to the control unit, which decide how to execute in the next part. For data transfer instructions, you can read and write data between the data memory and registers. For arithmetic or logic instructions, you can use the ALU module to get the answer, and write it to the registers. For conditional branch instructions, you can do comparison in the ALU module and branch to the address in the MIPS instruction. For jump instruction, you can directly jump to your target address.

You should handle two verilog files:

<ul>

 <li>v</li>

 <li>v</li>

</ul>

And your project report.

I will give you example verilog code in my slides and you should implement the whole cpu file and test file by yourself and analyze the final result in your report.

<h1>Grading</h1>

<strong> </strong>

Support the Data transfer instructions – – – – – – – – 10%

Support the Arithmetic/Logic instructions  – – – – – – – – 50%

<ul>

 <li>R-type unsigned arithmetic operations – 10%</li>

 <li>R-type signed arithmetic operations – 10%</li>

 <li>I-type arithmetic operations – 10%</li>

 <li>R-type logical arithmetic operations – 10%</li>

 <li>I-type logical arithmetic operations – 10%</li>

</ul>

Support the Branch/Jump instructions  – – – – – – – – 30%

Project report – – – – – – – – 10%

*You will get a 10% bonus if you implement a pipeline cpu.