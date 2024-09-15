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
