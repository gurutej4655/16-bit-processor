# 16-bit-processor

**COA Course Activity pattern** 

Design and simulate a **16-bit processor**, which can perform Load/Store, Arithmetic & Logical operations on a set of data. Design for a Harward Architecture, separate code memory & separate data memory to store program instructions and operands respectively. Include all the control & status registers like PC (to hold address of instruction) and IR (to decode the instruction). Include a **Register file of 8 Registers** (R0—R7). Include a data memory of size **512 x 16**. Include code memory of appropriate size. 

- Fetch the instruction using the contents of PC and update PC
- Decode the instruction from IR
- Execute the operation 
- Write the result back in the destination.

**Specifications to be followed for design**

**Instruction Set**

|**Inst.No**|**Opcode**|**Operation**|**Instruction Format**|
| - | :-: | :-: | :-: |
|1|0000|Load|LOAD R<sub>X</sub>, mem loc|
|2|0001|Store|STORE R<sub>X,</sub> mem loc|
|3|0010|Add|ADD R<sub>X</sub>, mem loc|
|4|0011|Subtract|SUB R<sub>X</sub>, mem loc|
|5|0100|Multiply|MUL R<sub>X</sub>, mem loc|
|6|0101|Divide|DIV R<sub>X</sub>, mem loc|
|7|0110|Increment|INC R<sub>X</sub>|
|8|0111|Decrement|DEC R<sub>X</sub>|
|9|1000|And|AND R<sub>X</sub>, mem loc|
|10|1001|Or|OR R<sub>X</sub>, mem loc|
|11|1010|Not|NOT R<sub>X</sub>|
|12|1011|Exchange|XCH R<sub>X</sub>, mem loc|
|13|1100|Shift Right|SHR R<sub>X</sub>, mem loc|
|14|1101|Shift Left|SHL R<sub>X</sub>, mem loc|
|15|1110|Rotate right|ROR R<sub>X</sub>, mem loc|
|16|1111|Rotate left|ROL R<sub>X</sub>, mem loc|


**Instruction Register Format**

|**Opcode(4 bits)**|**Register address (3 bits)**|**Mem loc address (9 bits)**|
| :-: | :-: | :-: |
