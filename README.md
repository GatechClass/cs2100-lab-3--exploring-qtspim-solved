# cs2100-lab-3--exploring-qtspim-solved
**TO GET THIS SOLUTION VISIT:** [CS2100 Lab #3- Exploring QtSpim Solved](https://mantutor.com/product/cs2100-computer-organisation-solved-8/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;112866&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS2100 Lab #3- Exploring QtSpim Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
Lab #3: Exploring QtSpim

Objective

In this lab, you will explore the QtSpim, a MIPS simulator available on Windows, Mac OS and Linux. This document and its associated files (sample1.asm, sample2.asm and sample3.asm) are all available on Canvas and the course website.

Software and Documentation

The following resources are available on the CS2100 website → “Resources” → “Online”, or https://www.comp.nus.edu.sg/~cs2100/2_resources/online.html directly.

1. QtSpim software: Download the correct QtSpim for your platform (either Windows or MacOS). Follow the installation instructions to install QtSpim in your system. In the lab, QtSpim for Windows has already been installed on the computers.

See https://support.apple.com/en-sg/guide/mac-help/mh40616/mac for how to get around this.

2. Assemblers, Linkers, and the SPIM Simulator documentation: An overview and reference manual for SPIM and MIPS32 instruction set. The sections that you should definitely read are Section A.9 (SPIM) and Section A.10 (MIPS R2000 Assembly Language). This document can also be found in the “Computer Organization and Design” reference book as Appendix A (3rd edition and before) or Appendix B (4th Edition). Note that the SPIM discussion is based on the older version of the simulator. Although there is significant change in the looks (UI) of the simulator, the underlying mechanism and information are largely intact.

Introduction

SPIM, which is just MIPS spelled backwards, is a software that simulates the working of a MIPS processor. It is capable of running MIPS32 assembly language programs and it allows user to inspect the various internal information of a MIPS processor. SPIM is a self-contained system for running MIPS programs. It contains a debugger and provides a few operating system–like services. SPIM is much slower – 100 or more times! – than a real computer. The most current version of SPIM is known as QtSpim which is basically the simulator SPIM with the Qt GUI framework on top. QtSpim is cross-platform and currently available for Windows, Mac OS and Debian Linux.

My First MIPS Program: sample1.asm

BEFORE YOU BEGIN, please read the (very) frequently asked question below.

FAQ: I ran the code and encountered this “Exception occurred at PC = 0x00000000” error, what should I do?

Answer: Your QtSpim is not using address 0x00400000 as the default start address of your

code. Click on “Simulator → Run Parameters” and change the value under “Address or label to start running program” from 0x00000000 to 0x00400000.

Let’s give it a try! Before you start, make sure you have downloaded the 3 assembly programs sample1.asm, sample2.asm and sample3.asm from Canvas or the course website to a working directory of your choice.

Click on the QtSpim shortcut at the desktop to invoke QtSpim. You should see a screen similar to the following:

Let’s check that we have the right simulator configuration for the labs. Click on “Simulator → Settings” (or QtSpim-&gt;Preferences on Macs) on the menu bar. Go to the “MIPS” tab then:

1. Click the “Simple Machine” button to use the simplest setting for the processor simulation.

2. Uncheck the “Load Exception Handler”.

Click “OK” to save your setting. Go to “File → Reinitialize and Load File” and select sample1.asm from your working directory.

With the settings mentioned, your QtSpim window should look exactly the same as follows:

The display is divided into three frames: Registers, Text Segment and Messages.

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> Registers frame: This window shows the values of special and integer registers in the MIPS CPU. There is a tab for FPU (floating point unit) registers, which you can safely ignore.

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> Messages frame: This is where QtSpim writes messages and where error messages appear.

Note that the Text Segment Frame can change to display the Data Segment by clicking on the

“Data” tab. The data segment represents the data your program loaded into the “main memory”, we’ll see more of this later.

Besides the above, there is also a separate Console window for input and output. If the Console window is hidden, you can click “Windows → Console” to enable it.

Let us now take a look at sample1.asm:

# sample1.asm

.text

main: addi $t1, $zero, 97 li $v0, 10

syscall

addi $9, $0, 97 ; 3: addi $t1, $zero, 97 ori $2, $0, 10 ; 4: li $v0, 10 syscall ; 5: syscall

The first line is a comment line, which begins with “#”. The second line .text is the assembler directive that specifies the starting address of the source code. If no starting address is specified, the default value 0x00400000 will be assumed.

The next line contains a MIPS instruction: the add immediate (addi) instruction will place the addition result (0 + 97), i.e. decimal value 97, into register $t1. Numbers are decimal (base 10) by default. If they are preceded by 0x, they are interpreted as hexadecimal (base 16). For example, 256 and 0x100 denote the same value. In QtSpim, the registers $t1 and $zero are translated into their respective numbered registers $9 and $0.

Observe the value of register $t1 (register 9) and the value of PC (program counter) in the Registers window. They are both zero at the moment.

The next two lines li $v0, 10 and syscall constitute a system call to exit. The line li $v0, 10 is a pseudo-instruction (li = load immediate) that is translated into ori $2, $0, 10. This will be explained in the next section and we will ignore them here.

If you want to make any modification to sample1.asm, you can use any text editor such as NotePad, etc. After modification, you need to reload it with “File → Load File”.

Now click on the “Single Step” button to execute one assembly statement.

You should see the changes to the PC and $t1 register in the register frame.

What number base is the value in register $t1? Answer: _________________________.

Text Segment Frame

Now, take a closer look at the text segment frame:

For each line,

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> the first column – [0x00400024] – is the memory location (address) of the instruction; (the default starting address is 0x00400000; some lines of code are inserted before your code by the system, hence your code starts at 0x00400024)

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> the second column – 0x20090061 – is the encoded instruction in hexadecimal;

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> the third column – addi $9, $0, 97 – is the native code; and

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> the fourth column – addi $t1, $zero, 97 – is your source code.

Everything after the semicolon is the actual line from your source code. The number “3:” refers to the line number of the corresponding MIPS instruction in the source code.

Sometimes there is nothing after the semicolon. This means that the instruction was produced by QtSpim as part of translating a pseudo-instruction into more than one real MIPS instruction.

Running and Stepping through Code

You can control the execution by choosing different modes.

“Run/Continue”:

Executes until

(program ends / error occurs / user pause / user stop)

Setting Value into a Register

“Change Register Contents” to assign value directly into that register. Try to change the value of R16 (which is $16 or $s0) to decimal value 100 (or hexadecimal 64).

Writing a message: sample2.asm

Download sample2.asm into your working directory. Click on “File” → “Reinitialize and Load File” to open this file.

The content of sample2.asm is shown below:

# sample2.asm

.data 0x10000100 msg: .asciiz “Hello”

.text main: li $v0, 4 la $a0, msg syscall li $v0, 10 syscall

You will notice that there are a couple of special names starting with a period, e.g. “.data”, “.text” etc. These are assembler directives that tell the assembler how to translate a program but do not produce machine instructions. The second line .data directive specifies the starting address (0x10000100) of the data (in this case, the string “Hello”). The .asciiz directive stores a null-terminated string (a string that ends with a null character) in memory.

For your reference, the set of directives that will be used in the lab exercises is given in the Appendix.

The first two statements are both pseudo-instructions:

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> Load immediate (A-57 in Appendix A): li rdest, imm # load the immediate imm into register rdest. <img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> Load address (A-66 in Appendix A): la rdest, address # load computed address – not the contents of the location – into register rdest.

The syscall instruction makes a system call, and the value in register $v0 indicates the type of call. The value 4 in $v0 indicates a print_string call (A-43 to A-43 in Appendix A: System Calls), and the string to be printed is indicated by $a0.

The value 10 in $v0 indicates an exit call.

We will explore more about system calls in the next lab.

Click on the “Data” tab on the Text Segment frame to display the Data Segment. Take a close look at the content of memory address 0x10000100:

Can you figure out where and how is the string “Hello” stored? Write out the ASCII values, in hexadecimal form, of the characters ‘H’, ‘e’, ‘l’ and ‘o’ below:

‘H’: ____ ‘e’: ____ ‘l’: ____ ‘o’: ____

Now, run the program (press the “Run/Continue” button). What do you see on the Console window? As mentioned before, you can ignore the “Attempt to execute non-instruction ….” error message for now.

Answer: ________________

Modifying a message: sample3.asm

Download sample3.asm into your working directory. Click on “File” → “Reinitialize and Load File” to open this file. The file is the same as sample2.asm at this point except a few comments added near the end of the main routine. We are going to edit the program to perform some simple tasks.

First, take some time to check your understanding of the li (load immediate) and la (load address) pseudo-instructions. Use the “Single Step” button to step through the program. Stop at the line “syscall”. What do you see in the register $v0 and $a0 at this point?

Answer: $v0 = _____________ $a0 = ____________________

Let us now read a single character (i.e. single byte) from the string into a register. Edit the given program sample3.asm as described below:

Add an instruction (lb – load byte) to load the value of ‘o’ (the last character in “Hello”) into register $t0. Add the instruction after the “syscall” instruction. What is the correct memory address to use? (Remember to save your edits, then reload the assembly file in QtSpim).

Answer: lb $t0, ______________

Now, we want to change the ‘o’ into ‘O’ (capital Oh). Let us first change the value in register $t0 by simple arithmetic. What is the difference in ASCII value between ‘o’ and ‘O’?

Answer: _________

Use the (addi – add immediate) instruction to change the value in $t0 to the ASCII value of

‘O’:

Answer: addi ____________________

Finally, let us put this back into the memory. Use the (sb – store byte) instruction to place the changed value of $t0 into the position ‘o’ (i.e. overwriting the value in memory). Take note of the change in data segment when you execute this instruction.

Answer: sb ______________________

Now, just make another syscall to print the string again. Add the instruction syscall at the end of the program as indicated by the comment. What do you see in the output when you run the program?

Answer: _________________________

Appendix
