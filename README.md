# SIC-pass-1-assembler-code
pass-1 assembler code of system software
Pass 1 of an assembler is the initial phase of a two-pass assembly process. Its primary function is to perform preliminary processing of the source code and generate essential data structures that are required for the second pass (Pass 2) of assembly. The main functionalities of Pass 1 include:

1. **Line-by-Line Tokenization**: Pass 1 reads the source code file line by line and tokenizes each line into its components. Typically, it breaks down each line into three parts: the label (if present), the operation code (opcode), and the operands. This information is stored for further processing.

2. **Symbol Table Generation**: As Pass 1 processes the source code, it builds a symbol table. This table records all labels and their corresponding memory addresses or values. The symbol table is essential for resolving references to labels, defining symbols, and handling forward references in the code.

3. **Location Counter (LC) Management**: Pass 1 keeps track of the current location counter (LC) as it processes instructions and directives in the code. The LC is incremented as instructions are encountered, and it accounts for the memory space that instructions and data occupy in the final program.

4. **Error Handling**: Pass 1 performs some basic error checking, such as detecting undefined symbols, missing or invalid opcodes, and other syntax errors. These checks help ensure that the source code is well-formed and can be assembled successfully in the second pass.

5. **Generating Intermediate Output**: Pass 1 may also produce intermediate output, often in the form of an assembly listing file. This file includes the original source code, along with the assigned addresses and other information. This listing file assists programmers in debugging and understanding the assembly process.

6. **Handling Special Directives**: Pass 1 interprets and processes assembler directives, such as "START," "END," "EQU," "ORG," and others. These directives control the program's organization, define constants, and set the starting point of the program.

7. **Handling Literal Constants**: Pass 1 identifies and handles literal constants in the source code, often by assigning them unique addresses and recording their values in the symbol table.

8. **Managing Program Length**: Pass 1 calculates and records the length of the program or the amount of memory needed to store the program. This information is essential for allocating memory in the final output and for calculating program size.

9. **Generation of Intermediary Files**: Pass 1 may create intermediary files that store information about the assembly process, such as the symbol table, location counter values, and other data that is used in Pass 2.

10. **Preparing for Pass 2**: Finally, Pass 1 prepares the necessary data structures and information required for the second pass of the assembly process. This includes passing along the symbol table and LC values to Pass 2.

The primary goal of Pass 1 is to create a foundation for the actual assembly process to occur in Pass 2. It gathers essential information, checks for errors, and prepares the groundwork for the generation of machine code and the final object program. Pass 2 will use this data to generate the actual machine code and produce the executable program.
