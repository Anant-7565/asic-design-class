***RISC-V Instruction Types***

**R-Type (Register):**

Opcode: 0110011
Description: These instructions perform arithmetic and logical operations between registers. Examples include ADD, SUB, AND, OR, and XOR.

**I-Type (Immediate):**

Opcode: 0010011 (for arithmetic operations with immediate values)
Opcode: 0000011 (for load operations)
Description: These instructions include arithmetic operations with an immediate value (e.g., ADDI, SLTI) and memory load instructions (e.g., LB, LW).

**S-Type (Store):**

Opcode: 0100011
Description: These instructions are used for storing data from registers to memory. Examples include SB (store byte), SH (store half-word), and SW (store word).

**B-Type (Branch):**

Opcode: 1100011
Description: These instructions are used for branching based on conditions. Examples include BEQ (branch if equal), BNE (branch if not equal), and BLT (branch if less than).

**U-Type (Upper Immediate):**

Opcode: 0110111 (for LUI - Load Upper Immediate)
Opcode: 0010111 (for AUIPC - Add Upper Immediate to PC)
Description: These instructions are used for handling large immediate values. LUI sets a register to a value with the upper 20 bits set, while AUIPC adds a large immediate value to the program counter.

**J-Type (Jump):**

Opcode: 1101111
Description: These instructions are used for jumps in the code. An example is JAL (jump and link), which jumps to a target address and saves the return address in a register.

For the given instructions, the instruction code and the operation type is as given below:

**1. ADD r5, r6, r7**
Binary: 0000000 00111 00110 000 00101 0110011
32-bit Instruction: 0x00E30533
Opcode: 0110011

**2. SUB r7, r5, r6**
Binary: 0100000 00110 00101 000 00111 0110011
32-bit Instruction: 0x40C283B3
Opcode: 0110011

**3. AND r6, r5, r7**
Binary: 0000000 00111 00101 111 00110 0110011
32-bit Instruction: 0x00F2B333
Opcode: 0110011

**4. OR r8, r6, r5**
Binary: 0000000 00101 00110 110 01000 0110011
32-bit Instruction: 0x005322B3
Opcode: 0110011

**5. XOR r8, r5, r4**
Binary: 0000000 00100 00101 100 01000 0110011
32-bit Instruction: 0x004282B3
Opcode: 0110011

**6. SLT r10, r2, r4**
Binary: 0000000 00100 00010 010 01010 0110011
32-bit Instruction: 0x004112B3
Opcode: 0110011

**7. ADDI r12, r3, 5**
Binary: 000000000101 00011 000 01100 0010011
32-bit Instruction: 0x00518393
Opcode: 0010011

**8. SW r3, r1, 4**
Binary: 0000000 00011 00001 010 00100 0100011
32-bit Instruction: 0x00312023
Opcode: 0100011

**9. SRL r16, r11, r2**
Binary: 0000000 00010 01011 101 10000 0110011
32-bit Instruction: 0x0025A833
Opcode: 0110011

**10. BNE r0, r1, 20**
Binary: 0000000 00001 00000 001 0100 0010 1100011
32-bit Instruction: 0x01408063
Opcode: 1100011

**11. BEQ r0, r0, 15**
Binary: 0000000 00000 00000 000 1111 0000 1100011
32-bit Instruction: 0x00F00063
Opcode: 1100011

**12. LW r13, r11, 2**
Binary: 000000000010 01011 010 01101 0000011
32-bit Instruction: 0x0025A583
Opcode: 0000011

**13. SLL r15, r11, r2**
Binary: 0000000 00010 01011 001 01111 0110011
32-bit Instruction: 0x0025A133
Opcode: 0110011
