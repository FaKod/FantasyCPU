Fantasy CPU
------------

###Memory And Registers

* RAM : 256 bytes
* A : 16bit general purpose register
* B : 16bit general purpose register
* C : 16bit general purpose register
* Z : Zero Flag (Only modified by CMP Instruction)
* IP : Instruction Pointer Register

###Example Code


```text
LOAD A, 1
SETM 0, A
LOADM A,0
OR A, 8
PRINT A
XOR A, 42
PRINT A
XOR A, 42
PRINT A
LOAD C, 10
PRINT C
DEC C
CMP C, 0
JNE -3
STOP
```

###Execute Example
mvn clean package exec:java