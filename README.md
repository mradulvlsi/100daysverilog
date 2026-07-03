100 Days of Verilog / SystemVerilog

A daily challenge to master RTL Design & Verification — one module at a time.


About This Repository

This repo documents my 100-day journey of hands-on RTL Design and Verification, where I design, simulate, and verify a new digital hardware module (almost) every day using Verilog and SystemVerilog.

The goal isn't just to write code — it's to build deep, interview-ready fluency in:


Combinational & Sequential Logic Design
Finite State Machines (FSMs)
Clock Domain Crossing (CDC) techniques
Standard Protocols — AXI4-Lite, UART, I2C, SPI
UVM-based Testbench Architecture
SystemVerilog Assertions (SVA) & Functional Coverage
Constrained-Random Verification


Every module here is written, simulated, debugged, and (wherever possible) verified with a proper testbench — not just copy-pasted code.


Why 100 Days?

I'm a 2025 B.Tech ECE graduate actively working toward becoming a strong RTL Design & Verification Engineer. Instead of passively studying theory, this challenge forces consistent, deliberate practice — the same discipline used in real ASIC/VLSI teams: design it, simulate it, break it, fix it, document it.

"Read less, code more, verify everything."






Progress Tracker

DayModuleTypeConcepts CoveredStatus018-bit Barrel ShifterDesignCombinational logic, shift/rotate operationsDone022:1 Multiplexer + TestbenchDesign + TBCombinational logic, basic self-checking TBDone03Bidirectional Shift RegisterDesignSequential logic, direction control, sync resetDone04Coming up...——Pending

This table will be updated daily as new modules are added.


Tools & Environment

CategoryTools UsedSimulationModelSim, EDA PlaygroundSynthesisXilinx VivadoVersion ControlGit & GitHubOSLinuxLanguagesVerilog, SystemVerilogMethodologyUVM (for advanced testbenches, introduced later in the challenge)


What I'm Building Toward

This challenge feeds directly into my larger verification projects, including:


Synchronous FIFO — Full UVM testbench (driver, monitor, scoreboard, sequencer, TLM ports) with 100% functional coverage
Asynchronous FIFO — Gray-code based CDC-safe design
UART TX/RX — Serial communication protocol design
AXI4-Lite Slave Interface — Industry-standard bus protocol implementation


The small daily modules in this repo build the fundamentals that make those larger projects possible.


How to Run

Each module can be simulated using any standard Verilog/SystemVerilog simulator.

Using ModelSim / QuestaSim:

bashvlog design.sv testbench.sv
vsim -c work.testbench_top -do "run -all"

Using EDA Playground:


Upload the design (.v / .sv) file to design.sv
Upload the testbench file to testbench.sv
Select simulator (e.g., Icarus Verilog / ModelSim) and click Run
