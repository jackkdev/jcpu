# Architecture

An instruction is a set of 1-byte operands prefixed with a 1-byte operation code (op code).

Three 1-byte registers exist: r0, r1 and r2.

## Addressing Modes

An instruction may have up to two operands. Thus the max size of an instruction is 3 bytes. How the data is sourced for each operand depends on the op code. Additionally, one operand is typically used as the destination register.

## Instruction Set

```
<op> <a> <b>

MOV <reg8>, <reg8>
MOV <reg8>, <imm8>
MOV <reg8>, <mem8>
MOV <mem8>, <reg8>

ADD <reg8>, <reg8>
ADD <reg8>, <imm8>
```