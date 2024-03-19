
## <a name="Day1---Introduction-to-open-source"></a>DAY1 - Introduction to open-source
### <a name="how-to-talk-to-Computers"></a>How to talk to Computers
The board show here is an **Arduino UNO**.The VLSI industry lies in the processor which is high-lighted in the circle.The entire chip is reffered as 
 ![image](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/84f394cb-0516-4bf2-b30f-c9f28a6c5af5)
 
 **Package**.For any chip we have **pads**.These pads acts as an interface between the external signals and internal signals inside the chip.
The **Core** is the place where our digital logic is placed.The place where the chip is manufactured is called as **Foundary**.
![image](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/18b4d56a-f6ac-4d57-a9e8-fec1bdcd9373)
### <a name="Soc-design-and-OpenLANE"></a>Soc design and OpenLANE
## About OpenLane 
OpenLANE is an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen, Fault, OpenPhySyn, SPEF-Extractor and custom methodology scripts for design exploration and optimization. It is a tool started for true open source tape-out experience and comes with APACHE version 2.0 . The goal of OpenLANE is to produce clean GDSII without any human intervention. OpenLANE is tuned for Skywater 130nm open-source PDK and can be used to produce hard macros and chips.
For Implementation os ASIC design ,we require the following :
       
        i.RTL Designs
       
        ii.PDK DATA
        
        iii.EDA Tools
        ![Screenshot (71)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/a8bff690-f4ee-4607-8898-0b0feabd207f)
## OpenLAne ASIC Flow 
![Screenshot (77)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/9d01e39d-4aa3-4cea-aa5e-fcdf5ad9da0f)

#### RTL to GDSII Description
**1. Synthesis:**
Yosys: Performs RTL synthesis using GTech mapping.
abc: Conducts technology mapping to standard cells defined in the Process Design Kit (PDK). Various synthesis techniques can be adjusted using different integrated abc scripts.
OpenSTA: Executes static timing analysis on the resulting netlist to generate timing reports.
Fault: Implements scan-chain insertion for post-fabrication testing, supporting ATPG (Automatic Test Pattern Generation) and test patterns compaction.

**2.Floorplan and PDN**
Init_fp - Defines the core area for the macro as well as the rows (used for placement) and the tracks (used for routing)
Ioplacer - Places the macro input and output ports
PDN - Generates the power distribution network
Tapcell - Inserts welltap and decap cells in the floorplan.

**3.Placement** – Placement is done in two steps, one with global placement in which we place the designs across the chip, but they will not be legal placement with some standard cells overlapping each other, to fix this we perform a detailed placement which legalizes the design and ensures they fit in the standard cell rows
RePLace - Performs global placement
Resizer - Performs optional optimizations on the design
OpenPhySyn - Performs timing optimizations on the design
OpenDP - Perfroms detailed placement to legalize the globally placed components.

**4. CTS**
TritonCTS - Synthesizes the clock distribution network.

**5.Routing**
FastRoute - Performs global routing to generate a guide file for the detailed router
TritonRoute - Performs detailed routing from global routing guides
SPEF-Extractor - Performs SPEF extraction that include parasitic information.

**GDSII Generation**
Magic - Streams out the final GDSII layout file from the routed def.

**Checks**
Magic - Performs DRC Checks & Antenna Checks
Netgen - Performs LVS Checks.

### <a name="Open-source-EDA-tools"></a>Open-source EDA tools ![1](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/2fddacec-5aab-435b-9aaa-6f83a13635d1)
##### list of  available project   
![3](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/4b0e45f8-09a7-4d64-bc4a-85b8b8d3b7e5)
![4](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/9f659de4-fd2a-437d-8620-9ef84514f737)

###### Selecting  picorv32a Design and list of required files
 The **src** folder contains the verilog description files for the design.In the **run** folder we can find the results and reports of every stage outputs.

 **note : ** To check the contents of the file we can use command **less** or **cat** before the file name i.e < **cat ** filename.extension >
 ![5](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/d4738d5e-6cc1-42ac-8b1b-4d15d234232f)

We Run the synthesis stage using command **run_synthesis** the Results of synthesis are shown below
![r2](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/d0aa6a95-ce9b-48f2-b650-7daa48db934d)
![r3](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/7a46a4b8-b783-456f-bcb2-08debc1580a8)

Flop Ratio : It is the ratio of number of D FF to Total number of cells
1613/14876=0.1084 
.i.e.. 10.84%
