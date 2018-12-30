# miniMIPS-Processor
A single cycle 8-bit processor that can load byte, store byte, add and subtract.

The miniMIPS:
------------
• 8-bit processor

• 4 x 8-bit registers

• 8-bit Data RAM

• 8-bit Program ROM/RAM

• 8-bit ALU

Register Set
---------------
$zero, $t0, $t1, $t2


Instruction Set Architecture
-----------------------------
lb rt, address # load byte from M[address] to R[rt]

sb rt, address # store byte from R[rt] to M[address]

add rd, rs, rt # add R[rd]=R[rs]+R[rt]

sub rd, rs, rt # add R[rd]=R[rs]-R[rt]


Instruction Formats
--------------------

opcode, rt, [rs, rd] / [address]

opcode = 2 bits; rs = 2 bits; rt = 2 bits; rd = 2 bits; address = 4 bits

Opcodes
--------
sub : opcode = 00

add : opcode = 01

sb : opcode = 10

lb : opcode = 11

Organisation
--------
Single cycle MIPS architecture
