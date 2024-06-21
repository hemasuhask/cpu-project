# cpu-project
A fully functioning CPU. Includes circuitry for load-word, store-word, beq, blt, or, and, addi, add, sub, subi, shr (shift-right), shl (shift-left), j, jal, and IO output/input instructions. Only basic components used (Gates, decoders/multiplexers, ROM, RAM, D Flip-Flops, etc.).

## Duke 250/16 Processor Core Design

### Overview
This project involves designing and implementing a 16-bit MIPS-like RISC architecture named Duke 250/16 using Logisim. The processor supports various instructions and includes an automated testing suite for validation. The focus on the software side involves understanding how low-level hardware interacts with software instructions, which can be extremely beneficial for software development projects that require optimization at the hardware level.

### Key Features
- **Architecture:** 16-bit word-addressed RISC
- **Instruction Types:** R-type, I-type, J-type
- **General Purpose Registers:** 8 registers ($r0-$r7)
- **Special Registers:** $r7 (link register), $r6 (stack pointer), $r0 (constant zero)

### Supported Instructions
- **Arithmetic:** add, sub, addi, xor, not
- **Shifts:** sll, srl
- **Memory Access:** lw, sw
- **Control Flow:** beqz, blt, j, jr, jal
- **I/O:** input, output

### Design and Implementation

#### Tools and Components Used
- **Logisim:** Main tool for circuit design
- **Components:**
  - Wiring, Gates, Plexers
  - Memory (D Flip-Flop, RAM, ROM)
  - Input/Output (Keyboard, TTY, Button)

#### Major Subcircuits
- **ALU:** Performs arithmetic and logical operations
- **Register File:** Contains 8 registers, supports read/write operations
- **Control Unit:** Decodes instructions and generates control signals
- **PC Logic:** Handles program counter updates
- **Memory Interface:** Manages instruction and data memory

#### Clocking Scheme
- **Rising Edge:** Register file, TTY
- **Falling Edge:** PC register, data memory, keyboard

#### Memory Layout
- **Instruction Memory:** Separate ROM block
- **Data Memory:** RAM block, word-addressed

### Software Utility
Understanding the design and implementation of the Duke 250/16 processor can provide significant insights for software developers, particularly in the following areas:
- **Optimization:** By understanding how software instructions are executed at the hardware level, developers can write more efficient code.
- **Embedded Systems:** Knowledge of processor design is crucial for developing software for embedded systems.
- **Debugging:** Insight into the interaction between software and hardware can improve debugging skills, especially for low-level software issues.
- **Educational Tool:** The processor serves as a practical example for teaching computer architecture and low-level programming concepts.

### Testing and Debugging
- **Automated Testing:** Provided scripts and tools to validate functionality
- **Manual Testing:** Step-by-step simulation in Logisim for debugging

### Skills and Knowledge Gained
- **Digital Logic Design:** Understanding of basic digital components and their integration
- **RISC Architecture:** Design principles of a reduced instruction set computer
- **Logisim Proficiency:** Circuit design and simulation using Logisim
- **Debugging:** Techniques for identifying and fixing issues in digital circuits

### Submission
**Files:**
- `cpu.circ`: Main Logisim circuit file
- `cpu.pdf` (optional): Description of processor functionality and issues

By completing this project, I gained a deep understanding of processor design, including the creation of an ALU, register file, and control unit, as well as practical experience with digital circuit simulation and debugging. These skills are directly applicable to software projects that require a deep understanding of the underlying hardware.
