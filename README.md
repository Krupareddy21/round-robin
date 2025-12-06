Implementation of Round Robin and Priority
Based Arbiter Using Verilog HDL

Introduction:
This project presents the design and implementation of two widely used hardware arbitration 
mechanisms—Round Robin Arbiter and Priority-Based Arbiter—using Verilog HDL. Arbiters 
play a crucial role in digital systems where multiple clients compete for shared resources such 
as buses or memory interfaces. The Priority Arbiter allocates access based on fixed priority 
levels, ensuring low-latency service for high-priority clients, while the Round Robin Arbiter 
rotates priority among all requesters to guarantee fairness and eliminate starvation. 
The design is modelled as a Finite State Machine (FSM), simulated using Vivado, and verified 
through behavioural, post-synthesis, and post-implementation timing simulations. 
Performance parameters such as latency, grant duration, resource utilization, and throughput 
are analysed to evaluate the efficiency of both schemes. The results demonstrate that the 
implementation is lightweight, scalable, and suitable for integration into SoC and bus-based 
systems requiring efficient request–grant arbitration. 

Coding in Verilog HDL:
The arbiter logic is developed using synthesizable Verilog. Inputs: req[3:0], priority pointer, 
clock, reset. Output: grant[3:0] (one-hot). Structural and behavior-level descriptions are 
combined to generate clean, modular RTL blocks. 


Simulation Using Vivado:
Testbenches are created to verify functionality under various request patterns. Behavioral 
Simulation validates logic correctness before synthesis. Timing Simulations (post-synthesis 
& post-implementation) check delays, signal transitions, and correctness after hardware 
mapping.  


CONCLUSION: 
The design and implementation of both Round Robin and Priority-Based Arbiters using Verilog HDL 
successfully demonstrate how effective arbitration improves shared resource access in digital systems. 
The Priority Arbiter provides fast and deterministic access for high-priority clients, while the Round 
Robin Arbiter ensures fairness by rotating priority among all requesters and eliminating starvation. 
Through FSM-based RTL design, simulation, synthesis, and post-implementation analysis, the arbiters 
were verified to operate correctly with low latency and minimal resource usage. The timing reports, 
power estimates, and throughput evaluation confirm that the design is lightweight, efficient, and suitable 
for integration into larger SoC or FPGA-based systems requiring reliable request–grant control. Overall, 
the project meets all intended objectives and provides a scalable arbitration solution that balances 
performance, fairness, and hardware cost.
