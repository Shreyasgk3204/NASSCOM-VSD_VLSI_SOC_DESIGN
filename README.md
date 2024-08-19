# NASSCOM-VSD_VLSI_SOC_DESIGN
This repo walks through the concepts discussed and learnt in 5 days workshop by VLSI SYSTEM DESIGN organisation .
## DAY-1


#### 1.  Microcontroller
This image showcases an Arduino board with the microcontroller circled. This chip is the central processing unit responsible for executing your code and controlling the board's functionalities.

![1](https://github.com/fortunespell/Nasscom-VSD-vlsi/blob/main/vsd/d1/d1_sk1/intro/Screenshot%202024-07-13%20095151.png)
#### 2. Microcontroller Internal Architecture
This diagram illustrates the internal architecture of a typical microcontroller. Key components include:
Processor/SoC (System on a Chip): The "brain" of the microcontroller responsible for executing instructions.
SDRAM (Synchronous Dynamic Random Access Memory): Volatile memory used for temporary data storage while the microcontroller is running.
Direct I2C, SPI, GPIO, PWM: These are communication protocols and input/output pins that allow the microcontroller to interact with external sensors, actuators, and other devices.

![2](https://github.com/fortunespell/Nasscom-VSD-vlsi/blob/main/vsd/d1/d1_sk1/intro/Screenshot%202024-07-13%20095251.png)


#### 3. Zooming in Microcontroller Die
This image provides a magnified view of the silicon die inside the microcontroller. Notable features:
RISC-V SoC: Indicates that the microcontroller utilizes the RISC-V instruction set architecture, known for its efficiency and open-source nature.
GPIO bank: A group of General Purpose Input/Output pins that can be configured as either inputs or outputs for interfacing with external components.
SRAM: Static RAM, a type of memory that retains its contents even when power is off, often used for storing critical program data.
Foundry IP's: Intellectual Property blocks licensed from semiconductor foundries, representing pre-designed and verified circuit modules integrated into the microcontroller.
Macros: Refers to larger functional blocks within the microcontroller's design, encompassing multiple logic gates and components.
![3](https://github.com/fortunespell/Nasscom-VSD-vlsi/blob/main/vsd/d1/d1_sk1/intro/Screenshot%202024-07-13%20095935.png)


#### Visualizing a RISC-V CPU Core: From Code to Silicon Layout
1. RISC-V Assembly Code (Left):
We start with a snippet of assembly code written for the RISC-V architecture.
Each line represents a low-level instruction, demonstrating the fundamental operations the CPU is designed to execute.
2. Implementation in Hardware Description Language (Bottom):
This section displays the implementation of the picorv32 CPU core using a Hardware Description Language (likely Verilog or SystemVerilog).
It demonstrates how the assembly instructions are translated into logical operations and register transfers within the CPU's architecture.
Parameters for configuring the core's features (like enabling counters or cache) are also visible.
3. Physical Layout (Right):
This represents the actual physical layout of the picorv32 CPU core, visualized using a tool like "qflow."
Different colors and labels represent various circuit elements like logic gates (AND2X2, BUFX2), flip-flops (DFFPOSx1), and interconnections.
This layout dictates how the transistors and wires are arranged on the silicon die to implement the CPU's functionality.
Key Takeaways:
The image illustrates the intricate link between software and hardware in CPU design.
Starting from high-level code, we traverse down to the physical realization of a RISC-V core, showcasing the different levels of abstraction involved.
This visual representation helps in understanding how CPU design choices in the hardware description language translate into the physical layout of the silicon chip.
![4](https://github.com/fortunespell/Nasscom-VSD-vlsi/blob/main/vsd/d1/d1_sk1/riscv/Screenshot%202024-07-13%20100329.png)

#### Bridging the Gap: From Software to Silicon
1. Application Software (Top Left):
Our journey begins with the software applications we use daily.
These applications, written in languages like C++, Java, or Python, interact with the underlying system through a defined set of instructions.
2. System Software and Compilation (Top):
The Operating System (OS) acts as an intermediary, managing system resources and providing an interface for applications to interact with the hardware.
Compilers translate high-level code (e.g., C++) into lower-level assembly language instructions specific to the target CPU architecture.
3. Assembly and Machine Code (Middle):
The Assembler further converts assembly code into binary machine code (0s and 1s) that the hardware can directly understand and execute.
The Instruction Set Architecture (ISA) serves as the abstract interface between software and hardware, defining the set of instructions a processor can execute.
4. Hardware Implementation (Bottom):
  Register Transfer Level (RTL):
    This stage describes the hardware behavior using a Hardware Description Language (HDL) like Verilog or VHDL. RTL defines the flow of data between registers and the logical operations         performed.
   
  Netlist Synthesis:
    The RTL description is synthesized into a netlist, a detailed representation of the circuit's interconnected components (gates, flip-flops).
    
  Physical Design:
    Finally, the netlist guides the physical placement and routing of transistors and wires on the silicon die, resulting in the tangible hardware that executes the original software             instructions.
    ![5](https://github.com/fortunespell/Nasscom-VSD-vlsi/blob/main/vsd/d1/d1_sk1/software%20to%20hardware/Screenshot%202024-07-13%20104219.png)
![6](https://github.com/fortunespell/Nasscom-VSD-vlsi/blob/main/vsd/d1/d1_sk1/software%20to%20hardware/Screenshot%202024-07-13%20104157.png)
![7](https://github.com/fortunespell/Nasscom-VSD-vlsi/blob/main/vsd/d1/d1_sk1/software%20to%20hardware/Screenshot%202024-07-13%20100706.png)
Key Takeaways:
This diagram highlights the layered abstraction involved in bridging the gap between software and hardware.
It emphasizes the crucial role of compilers, assemblers, and hardware design tools in translating abstract instructions into physical circuits.
Understanding this flow provides valuable insights into the relationship between software, hardware, and the underlying computer architecture.



