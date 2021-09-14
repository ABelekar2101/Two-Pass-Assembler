# Two-Pass-Assembler

**Assembler** is a program for converting instructions written in low-level assembly code into relocatable machine code and generating along information for the loader.

It generates instructions by evaluating the mnemonics (symbols) in operation field and find the value of symbol and literals to produce machine code. Now, if assembler does all this work in one scan then it is called single pass assembler, otherwise if it does in multiple scans then called multiple pass assembler. Here assembler divide these tasks in two passes:

**Pass-1:**
</br> 1. Define symbols and literals and remember them in symbol table and literal table respectively.
</br> 2. Keep track of location counter
</br> 3. Process pseudo-operations

**Pass-2:**
</br> 1. Generate object code by converting symbolic op-code into respective numeric op-code
</br> 2. Generate data for literals and look for values of symbols



### In this repository I have added C++ (.cpp) codes for pass-1 and pass-2 each. </br>The input test case file and output files have also been added.

input.txt - test case
</br>ic.txt - intermediate code output after pass-1
</br>symtable.txt - symbol table output after pass-1
</br>littable.txt - literal table output after pass-1
</br>machine_code.txt - machine code output after pass-2
