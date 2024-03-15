# NASSCOM-VSD-SoC-Design-Program
Workshop on Digital VLSI SoC Design and Planning program Using **Openlane **
## About OpenLane 
OpenLANE is an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen, Fault, OpenPhySyn, SPEF-Extractor and custom methodology scripts for design exploration and optimization. It is a tool started for true open source tape-out experience and comes with APACHE version 2.0 . The goal of OpenLANE is to produce clean GDSII without any human intervention. OpenLANE is tuned for Skywater 130nm open-source PDK and can be used to produce hard macros and chips.


### OpenLAne ASIC Flow 

![Screenshot (77)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/9d01e39d-4aa3-4cea-aa5e-fcdf5ad9da0f)

#### RTL to GDSII Description
**1. Synthesis:**
Yosys: Performs RTL synthesis using GTech mapping.
abc: Conducts technology mapping to standard cells defined in the Process Design Kit (PDK). Various synthesis techniques can be adjusted using different integrated abc scripts.
OpenSTA: Executes static timing analysis on the resulting netlist to generate timing reports.
Fault: Implements scan-chain insertion for post-fabrication testing, supporting ATPG (Automatic Test Pattern Generation) and test patterns compaction.
2.Floorplan and PDN
Init_fp - Defines the core area for the macro as well as the rows (used for placement) and the tracks (used for routing)
Ioplacer - Places the macro input and output ports
PDN - Generates the power distribution network
Tapcell - Inserts welltap and decap cells in the floorplan
Placement – Placement is done in two steps, one with global placement in which we place the designs across the chip, but they will not be legal placement with some standard cells overlapping each other, to fix this we perform a detailed placement which legalizes the design and ensures they fit in the standard cell rows
RePLace - Performs global placement
Resizer - Performs optional optimizations on the design
OpenPhySyn - Performs timing optimizations on the design
OpenDP - Perfroms detailed placement to legalize the globally placed components
3. CTS
TritonCTS - Synthesizes the clock distribution network
4.Routing
FastRoute - Performs global routing to generate a guide file for the detailed router
TritonRoute - Performs detailed routing from global routing guides
SPEF-Extractor - Performs SPEF extraction that include parasitic information
GDSII Generation
Magic - Streams out the final GDSII layout file from the routed def
Checks
Magic - Performs DRC Checks & Antenna Checks
Netgen - Performs LVS Checks
