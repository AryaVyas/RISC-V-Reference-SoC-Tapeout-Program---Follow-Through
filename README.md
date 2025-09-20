	1.	Chip Modelling (O1)
	•	The first step is defining the system’s specifications.
	•	This is often done with a C model, which helps in checking the behavior early using testbenches written in C.
	2.	RTL Architecture (O2)
	•	Once the specs are fixed, the hardware description is created in RTL (Verilog).
	•	The design is split into blocks like processor cores and peripheral/IP modules.
	•	At this stage, the RTL can be simulated to ensure functionality.
	3.	Synthesis & IP Integration
	•	The RTL is synthesized into a gate-level netlist.
	•	Pre-designed macros and analog IPs are also integrated at this stage.
	•	Together, these pieces form the backbone of the SoC.
	4.	SoC Integration (O3)
	•	All components (processor, peripherals, macros, analog IPs) are connected at the top level.
	•	GPIOs and other interfaces are brought together to form a complete SoC.
	5.	Physical Design (RTL to GDS)
	•	Floorplanning, placement, clock tree synthesis (CTS), and routing are carried out.
	•	The final output is the GDSII file, which is used for fabrication.
	•	Before tape-out, checks like DRC (Design Rule Check) and LVS (Layout vs Schematic) are done to verify correctness.
